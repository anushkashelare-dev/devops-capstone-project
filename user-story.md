# User Story Template

Use this template to capture a user story for the Account Service project.

## Story

**As a** [type of user],

**I need** [an action or capability],

**So that** [the benefit or value].

## Acceptance Criteria

Given [the initial context],

When [the user takes an action],

Then [the expected outcome].

## Additional Notes

- **Priority:** [High / Medium / Low]
- **Estimate:** [Story points]
- **Dependencies:** [Related stories or requirements]
- **Notes:** [Any additional information]

---

## Example: Read an Account

**As a** service user,

**I need** to retrieve an account by its ID,

**So that** I can view the account details.

### Acceptance Criteria

Given an account exists,

When I request the account using its ID,

Then the service returns the account details with an HTTP 200 response.

Given no account exists with the requested ID,

When I request that account,

Then the service returns an HTTP 404 response.
