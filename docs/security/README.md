# Security Module

## Overview

The security module in `src/security` implements authentication and authorization using Supabase for JWT token validation. It ensures users can only access their own threads and assistants.

Key components:
- `auth.py`: Defines authentication functions and handlers for threads and assistants.

## Authentication Logic

- `get_current_user`: Verifies JWT tokens via Supabase.
- Handlers for create/read/update/delete operations on threads and assistants, setting ownership metadata and filters.
- Store authorization based on user identity in namespaces.

## Connections

Integrates with LangGraph SDK for auth middleware. Requires SUPABASE_URL and SUPABASE_KEY environment variables.

This module secures the application by enforcing user-specific access controls.