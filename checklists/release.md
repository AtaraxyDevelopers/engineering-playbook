# Release checklist

## Before release

- Identify the exact revision and intended environment.
- Complete checks appropriate to the change and record their results.
- Confirm that necessary configuration exists without printing secret values.
- Check relevant database migration and backward compatibility implications.
- Verify a recoverable backup or rollback method when the change affects stored data.
- Define the signal that would trigger rollback and who can perform it.

## During release

- Use the established deployment route with the required approvals.
- Confirm that the intended revision is running.
- Check the critical user flow and relevant integration responses.
- Observe error rates, job failures, and other applicable operational signals.

## After release

- Record the outcome and any follow-up work.
- Confirm scheduled jobs still run when the release changes their dependencies.
- Update user-facing documentation when behavior has changed.
- Investigate unexpected results before widening the rollout.

## Recovery note

A backup file alone is not evidence of recoverability. Verify the integrity and restore process at a level appropriate to the data and service. Keep production data out of public test artifacts.
