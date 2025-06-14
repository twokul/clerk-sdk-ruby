## 4.1.0 - 2025-04-10

- feat: Add support for token v2 org claims [https://github.com/clerk/clerk-sdk-ruby/pull/89]
- feat: Emit `Clerk-Version-API` header [https://github.com/clerk/clerk-sdk-ruby/pull/89]

## 4.0.1 - 2025-01-27

- fix: Ensure that the logger was being correctly passed to the API client  [https://github.com/clerk/clerk-sdk-ruby/pull/87]
- docs: Expand sections within the README [https://github.com/clerk/clerk-sdk-ruby/pull/86]

## 4.0.0 - 2025-01-27

- chore: Relese v4.0.0 based on v4.0.0.beta7 [https://github.com/clerk/clerk-sdk-ruby/pull/85]

## 4.0.0.beta7 - 2025-01-27

- chore: Bump dependency versions [https://github.com/clerk/clerk-sdk-ruby/pull/82]

## 4.0.0.beta6 - 2025-01-27
 
- feat: Allows for users to be able to skip the automatic addition of the Clerk Middleware via Railties. [https://github.com/clerk/clerk-sdk-ruby/pull/81]
- build: Introduces a repeatable release flow. [https://github.com/clerk/clerk-sdk-ruby/pull/81]

## 4.0.0.beta5 - 2025-01-27

[BREAKING] This release introduces our new `clerk-http-client` gem, which is a generated directly from the Clerk API OpenAPI specs. This will help to ensure that the SDK is always in sync with the Clerk API.

- feat: Add support for the `clerk-http-client` gem [https://github.com/clerk/clerk-sdk-ruby/pull/77]
- feat: Add support for Revalidation [https://github.com/clerk/clerk-sdk-ruby/pull/77]
- feat: Add support for Rails API mode [https://github.com/clerk/clerk-sdk-ruby/pull/77]
- feat: Add support for Sinatra [https://github.com/clerk/clerk-sdk-ruby/pull/77]
- feat: Middleware cache defaults to `Rails.cache` -> `ActiveSupport::Cache::MemoryStore` (if available) -> no caching [https://github.com/clerk/clerk-sdk-ruby/pull/77]
- chore: Refactor Clerk helper methods for Rails and Rack [https://github.com/clerk/clerk-sdk-ruby/pull/77]
- fix: Update configuration naming of `api_key` to `secret_key` [https://github.com/clerk/clerk-sdk-ruby/pull/77]
- docs: Add example applications for Rails, Sinatra, and Rack under `apps/` [https://github.com/clerk/clerk-sdk-ruby/pull/77]



## 4.0.0.beta4 - 2025-01-06

[BREAKING] This release introduces our new `clerk-http-client` gem, which is a generated directly from the Clerk API OpenAPI specs. This will help to ensure that the SDK is always in sync with the Clerk API.

- feat: Add support for the `clerk-http-client` gem [https://github.com/clerk/clerk-sdk-ruby/pull/77]
- feat: Add support for Revalidation [https://github.com/clerk/clerk-sdk-ruby/pull/77]
- feat: Add support for Rails API mode [https://github.com/clerk/clerk-sdk-ruby/pull/77]
- feat: Add support for Sinatra [https://github.com/clerk/clerk-sdk-ruby/pull/77]
- feat: Middleware cache defaults to `Rails.cache` -> `ActiveSupport::Cache::MemoryStore` (if available) -> no caching [https://github.com/clerk/clerk-sdk-ruby/pull/77]
- chore: Refactor Clerk helper methods for Rails and Rack [https://github.com/clerk/clerk-sdk-ruby/pull/77]
- fix: Update configuration naming of `api_key` to `secret_key` [https://github.com/clerk/clerk-sdk-ruby/pull/77]
- docs: Add example applications for Rails, Sinatra, and Rack under `apps/` [https://github.com/clerk/clerk-sdk-ruby/pull/77]

## 4.0.0.beta3 - 2024-04-02

- fix: Make publishable_key and secret_key required without making the envs required [https://github.com/clerk/clerk-sdk-ruby/pull/53]

## 4.0.0.beta2 - 2024-02-26

Note: this is identical to 4.0.0.beta1, which was yanked because it was not generated from the main branch.

- feat: replace interstitial with handshake (internal mechanisms) [https://github.com/clerk/clerk-sdk-ruby/pull/45]
- chore: re-organize and refactor internal code to extract functionality of rack middleware [https://github.com/clerk/clerk-sdk-ruby/pull/45]
- changed: `CLERK_PUBLISHABLE_KEY` or `publishable_key` in `Clerk.configure` is **required** [https://github.com/clerk/clerk-sdk-ruby/pull/46]

## [YANKED] 4.0.0.beta1 - 2024-02-26

- feat: replace interstitial with handshake (internal mechanisms) [https://github.com/clerk/clerk-sdk-ruby/pull/45]
- chore: re-organize and refactor internal code to extract functionality of rack middleware [https://github.com/clerk/clerk-sdk-ruby/pull/45]
- changed: `CLERK_PUBLISHABLE_KEY` or `publishable_key` in `Clerk.configure` is **required** [https://github.com/clerk/clerk-sdk-ruby/pull/46]

## 3.2.0 - 2024-04-08

- fix: Infinite redirect loop when client_uat=0 and __session exists [https://github.com/clerk/clerk-sdk-ruby/pull/55]

## 3.1.0 - 2024-03-19

- fix: Incompatible __client_uat & __session should show interstitial [https://github.com/clerk/clerk-sdk-ruby/pull/51]
- fix: Incorrect check that lead to infinite redirect loop introduced by [https://github.com/clerk/clerk-sdk-ruby/pull/51]

## 3.0.0 - 2024-01-09

Note: this is identical to 2.12.0, which was yanked because it contained a
breaking change.

- feat: Add org role/permission helpers [https://github.com/clerk/clerk-sdk-ruby/pull/40]
- changed: drop create sms endpoint [https://github.com/clerk/clerk-sdk-ruby/pull/39]

## [YANKED] 2.12.0 - 2024-01-09

- feat: Add org role/permission helpers [https://github.com/clerk/clerk-sdk-ruby/pull/40]
- changed: drop create sms endpoint [https://github.com/clerk/clerk-sdk-ruby/pull/39]

## 2.11.1 - 2023-10-31

- fix: Properly set Clerk API key (secret) when using Faraday v2 [https://github.com/clerkinc/clerk-sdk-ruby/pull/37]

## 2.11.0 - 2023-10-27

- feat: Added support for Faraday v2 [https://github.com/clerkinc/clerk-sdk-ruby/pull/37]

## 2.10.0 - 2023-04-04

Identical to 2.10.0.beta2

## 2.10.0.beta2 - 2023-03-08

- fix: incorrect usage keyword parameter (fix for 2.10.0.beta1)

## 2.10.0.beta1 - 2023-03-08

- fix: Change signed-out & interstitial request state conditions [https://github.com/clerkinc/clerk-sdk-ruby/pull/30]

## 2.9.0

Identical to 2.9.0.beta3

## 2.9.0.beta3 - 2023-01-17

## Changed

- internal: Change request payloads to `application/json` content type [https://github.com/clerkinc/clerk-sdk-ruby/pull/29]

## 2.9.0.beta2 - 2023-01-05

- feat: Support setting the secret key (previously called Backend API key) using
  the `CLERK_SECRET_KEY` environment variable [https://github.com/clerkinc/clerk-sdk-ruby/pull/28]

## 2.9.0.beta1 - 2022-12-23

- fix: Make JWKS cache work across different SDK instances [https://github.com/clerkinc/clerk-sdk-ruby/pull/27]

## 2.8.0 - 2022-11-29

- feat: Add support for the users.verify_totp endpoint

## 2.7.0 - 2022-11-02

- feat: Add `#clerk_organization` and `#clerk_organization_id` helpers to fetch the current user's active organization [https://github.com/clerkinc/clerk-sdk-ruby/pull/22]
- feat: Implement Organization Metadata update endpoint [https://github.com/clerkinc/clerk-sdk-ruby/pull/21]

## 2.6.0 - 2022-11-01

- feat: Implement Organization endpoints [https://github.com/clerkinc/clerk-sdk-ruby/pull/20]

## 2.5.0 - 2022-09-20

- feat: Add support for disabling the middleware on specific routes [https://github.com/clerkinc/clerk-sdk-ruby/pull/19]

## 2.4.0 - 2022-09-05

- feat: Add support for the users.disable_mfa endpoint

## 2.3.0 - 2022-08-30

- feat: Add support for the users.verify_password endpoint

## 2.2.0 - 2022-08-26

- feat: Add support for the [users.create](https://clerk.com/docs/reference/backend-api/tag/Users#operation/CreateUser) endpoint

## 2.1.2 - 2022-08-26

- fix: Gracefully handle invalid JSON in Authorization header [https://github.com/clerkinc/clerk-sdk-ruby/pull/16]

## 2.1.1 - 2022-02-24

- fix: Make Authv2 middleware thread-safe

## 2.0.0 - 2021-10-21

This release introduces the new networkless middleware which works with the new
authentication scheme, [Auth v2](https://clerk.com/docs/upgrade-guides/auth-v2).

It is backwards-incompatible with applications using Auth v1.

- [BREAKING]: In order to use this version, you must set the authVersion prop
    accordingly in your frontend: `Clerk.load({authVersion: 2})`

For more information on Auth v2, please refer to
https://clerk.com/docs/upgrade-guides/auth-v2.

## 1.0.3 - 2021-07-21

- fix: Proper endpoint for oauth_access_token method

## 1.0.2 - 2021-06-03

- fix: Instantiation of `Clerk::SDK` without prior call to `Clerk.configure`

## 1.0.1 - 2021-06-03

### enhancements

- Middleware now uses a proxy object which lazy loads the Clerk session and user only when needed

## 1.0.0 - 2021-05-27

- initial release
