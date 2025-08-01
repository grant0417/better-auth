# @better-auth/stripe

## 1.3.5

### Patch Changes

- 2ec8cad: should fallback to subscription id when it's present in the body
- a536de9: Fix an issue where updating Stripe customer ID wasn't properly syncing with secondary storage during user creation
- Updated dependencies [e4af253]
- Updated dependencies [b27221b]
- Updated dependencies [d1d593f]
- Updated dependencies [29c0df5]
- Updated dependencies [978b285]
  - better-auth@1.3.5

## 1.3.4

### Patch Changes

- ac6baba: chore: fix typo on `freeTrial`
- c2fb1aa: Fix duplicate trials when switching plans
- 2bd2fa9: Added support for listing organization members with pagination, sorting, and filtering, and improved client inference for additional organization fields. Also fixed date handling in rate limits and tokens, improved Notion OAuth user extraction, and ensured session is always set in context.

  Organization

  - Added listMembers API with pagination, sorting, and filtering.
  - Added membersLimit param to getFullOrganization.
  - Improved client inference for additional fields in organization schemas.
  - Bug Fixes
  - Fixed date handling by casting DB values to Date objects before using date methods.
  - Fixed Notion OAuth to extract user info correctly.
  - Ensured session is set in context when reading from cookie cach

- Updated dependencies [2bd2fa9]
  - better-auth@1.3.4
