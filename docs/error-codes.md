<!--
- SPDX-FileCopyrightText: 2021 TQ Tezos

- SPDX-License-Identifier: LicenseRef-MIT-TQ
-->

<!--
NOTE: This file should not be modified directly.
Use `stack scripts/generate_error_code.hs` instead.
-->

## Error Codes

Here is a summary of all the error codes thrown by the contract.


 #### Invalid Input Error Codes

| Error Code       | Error Label      | Description                                           |
|------------------|------------------|-------------------------------------------------------|
| 100 | `not_admin` | The sender is not the administrator. |
| 101 | `not_pending_admin` | The sender is not the current pending administrator. |
| 102 | `fail_proposal_check` | Thrown paired with a `string` error message when the proposal does not pass the `proposal_check`. |
| 103 | `proposal_not_exist` | The proposal does not exist or is no longer ongoing. |
| 104 | `voting_stage_over` | The proposal voting stage has already ended. |
| 105 | `max_proposals_reached` | The maximum amount of ongoing proposals has been reached. |
| 106 | `max_voters_reached` | The maximum amount of voters has been reached for the proposal. |
| 107 | `forbidden_xtz` | Transfer of XTZ is forbidden on this entrypoint. |
| 108 | `proposal_not_unique` | The submitted proposal already exist. |
| 109 | `missigned` | Parameter signature does not match the expected one - for permits. |
| 110 | `unpacking_failed` | The unpacking of a submitted value failed. |
| 111 | `unpacking_proposal_metadata_failed` | The unpacking of a proposal metadata failed. |
| 112 | `missing_value` | A required field value was not found. |
| 113 | `not_proposing_stage` | Proposals cannot be submitted in non-proposing stages. |
| 114 | `not_enough_frozen_tokens` | There aren't enough frozen tokens for the operation. |
| 115 | `bad_token_contract` | The governance token contract does not have the expected entrypoints. |
| 116 | `bad_view_contract` | The type of a contract for a view entrypoint is not of the expected type. |
| 117 | `drop_proposal_condition_not_met` | The conditions to drop this proposal are not met. |
| 118 | `expired_proposal` | The proposal has expired and can no longer be flushed. |
| 119 | `empty_flush` | There are no available proposals to flush. |
| 120 | `not_delegate` | The sender has not been delegated the control of the required tokens. |
| 121 | `fail_decision_lambda` | Executing the proposal's decision lambda results in failure. |
| 122 | `entrypoint_not_found` | The chosen custom entrypoint does not exist. |





 #### Internal Error Codes

| Error Code       | Error Label      | Description                                           |
|------------------|------------------|-------------------------------------------------------|
| 300 | `bad_state` | Throw when storage is in an unexpected state, indicating a contract error. |


