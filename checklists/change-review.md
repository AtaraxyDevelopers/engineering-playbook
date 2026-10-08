# Change review

Use the checks that match the change. A small copy edit and a payment flow need different levels of validation.

## Behavior

- Does the change solve the stated problem with an observable outcome?
- Are empty, invalid, duplicate, and unavailable states handled where relevant?
- Could the change affect existing callers, saved data, or integrations?

## Interfaces

- Can the main flow be completed with a keyboard, with a visible focus indicator?
- Do fields have labels and errors that explain how to recover?
- Are layouts usable at narrow widths and with enlarged text?
- Does the interface explain decisions in terms meaningful to its users?

## Data and security

- Is access checked at the boundary where the operation happens?
- Are secrets and private records absent from source, public issues, and logs?
- Are input handling and output encoding appropriate to the context?
- Is collected data necessary for the feature?

## Verification and maintainability

- Do checks exercise meaningful behavior, including relevant failures?
- Are important assumptions and tradeoffs recorded?
- Is the change understandable without knowing the conversation that led to it?
- Are new dependencies justified and operational costs understood?
