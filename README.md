# bugrank.io
BugRank API Specification

## Version: 1.0

### /auth/login

#### POST
##### Summary:

Login

##### Description:

Login

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | OK |

### /account/register-hacker

#### POST
##### Summary:

Register hacker account

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | OK |

### /account/register

#### POST
##### Summary:

Register admin account

##### Description:

Register admin account (test only)

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | OK |

### /account/register-host

#### POST
##### Summary:

Register company

##### Description:

Register host (company) account

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | OK |

### /account/update-avatar

#### POST
##### Summary:

Update avatar (for both host and hacker)

##### Description:

update avatar (for both host and hacker)

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | OK |

##### Security

| Security Schema | Scopes |
| --- | --- |
| Authorization | |

### /account/resend-verification-email/{email}

#### POST
##### Summary:

Resend verification email

##### Description:

Resend verification email

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| email | path |  | Yes | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | OK |

##### Security

| Security Schema | Scopes |
| --- | --- |
| Authorization | |

### /account/forgot-password

#### POST
##### Summary:

Forgot password

##### Description:

Forgot password

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | OK |

### /account/change-password

#### POST
##### Summary:

Change password

##### Description:

Change password

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | OK |

##### Security

| Security Schema | Scopes |
| --- | --- |
| Authorization | |

### /auth/logout

#### POST
##### Summary:

Logout

##### Description:

Logout

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | OK |

##### Security

| Security Schema | Scopes |
| --- | --- |
| Authorization | |

### /account/me

#### GET
##### Summary:

Show current login user

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | OK |

##### Security

| Security Schema | Scopes |
| --- | --- |
| Authorization | |

### /account/update_language

#### POST
##### Summary:

Update language

##### Description:

Update language

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | OK |

##### Security

| Security Schema | Scopes |
| --- | --- |
| Authorization | |

### /host/update-policy

#### POST
##### Summary:

Update policy for company

##### Description:

Update policy for company

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | OK |

##### Security

| Security Schema | Scopes |
| --- | --- |
| Authorization | |

### /host/get-all-policy/{host_id}

#### GET
##### Summary:

Get all policy (todo)

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| host_id | path |  | Yes | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | OK |

##### Security

| Security Schema | Scopes |
| --- | --- |
| Authorization | |

### /host/profile

#### GET
##### Summary:

Get host profile

##### Description:

Get host profile

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | OK |

##### Security

| Security Schema | Scopes |
| --- | --- |
| Authorization | |

### /host/update-profile

#### POST
##### Summary:

Update company profile

##### Description:

Update company profile

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | OK |

##### Security

| Security Schema | Scopes |
| --- | --- |
| Authorization | |

### /host/users

#### GET
##### Summary:

Get all users in company

##### Description:

Get all users in company

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | OK |

##### Security

| Security Schema | Scopes |
| --- | --- |
| Authorization | |

### /host/users/remove/{user_id}

#### GET
##### Summary:

Remove user from company (change to POST)

##### Description:

Remove user from company

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| user_id | path |  | Yes | integer |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | OK |

##### Security

| Security Schema | Scopes |
| --- | --- |
| Authorization | |

### /host/users/invite/{username}

#### GET
##### Summary:

Invite user to join company (change to POST)

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| username | path |  | Yes | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | OK |

##### Security

| Security Schema | Scopes |
| --- | --- |
| Authorization | |

### /host/user/uninvite/{username}

#### GET
##### Summary:

Uninvite user to join company (change to POST)

##### Description:

Uninvite user to join company

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| username | path |  | Yes | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | OK |

##### Security

| Security Schema | Scopes |
| --- | --- |
| Authorization | |

### /hackers/joined-companies

#### GET
##### Summary:

Get all join company invitations of hacker (for hacker)

##### Description:

Get all join company invitations of hacker (for hacker)

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | OK |

##### Security

| Security Schema | Scopes |
| --- | --- |
| Authorization | |

### /hackers/join_company_invitations

#### GET
##### Summary:

Get all join company invitations of hacker (for hacker)

##### Description:

Get all join company invitations of hacker (for hacker)

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | OK |

##### Security

| Security Schema | Scopes |
| --- | --- |
| Authorization | |

### /host/users/invitations

#### GET
##### Summary:

Get all current invitations (for company)

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | OK |

##### Security

| Security Schema | Scopes |
| --- | --- |
| Authorization | |

### /hackers/accept_company_invitation/{host_id}

#### POST
##### Summary:

Accept company invitation

##### Description:

Accept company invitation

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| host_id | path |  | Yes | integer |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | OK |

##### Security

| Security Schema | Scopes |
| --- | --- |
| Authorization | |

### /hackers/decline_company_invitation/{host_id}

#### POST
##### Summary:

Decline join company invitation

##### Description:

Decline join company invitation

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| host_id | path |  | Yes | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | OK |

##### Security

| Security Schema | Scopes |
| --- | --- |
| Authorization | |

### /programs/my-programs

#### GET
##### Summary:

Get my programs (for both company and hacker) todo: udpate filter

##### Description:

Get my programs (for both company and hacker)

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| search | query |  | No | string |
| sort | query |  | No | string |
| filter | query |  | No | string |
| per_page | query |  | No | integer |
| page | query |  | No | integer |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | OK |

##### Security

| Security Schema | Scopes |
| --- | --- |
| Authorization | |

### /programs/new

#### POST
##### Summary:

Create new program (todo: validate host and program parameter)

##### Description:

Create new program

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | OK |

##### Security

| Security Schema | Scopes |
| --- | --- |
| Authorization | |

### /programs/archive

#### POST
##### Summary:

Archive program

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | OK |

##### Security

| Security Schema | Scopes |
| --- | --- |
| Authorization | |

### /programs/update/{program_id}

#### POST
##### Summary:

Update program (todo: define stricter type for field)

##### Description:

Update program

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| program_id | path |  | Yes | integer |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | OK |

##### Security

| Security Schema | Scopes |
| --- | --- |
| Authorization | |

### /programs/{id}

#### GET
##### Summary:

Get program by id

##### Description:

Get program by id

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| id | path |  | Yes | integer |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | OK |

##### Security

| Security Schema | Scopes |
| --- | --- |
| Authorization | |

### /programs/{program_id}/assign/{user_id}

#### POST
##### Summary:

Assign program to user (for company)

##### Description:

Assign program to user (for company)

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| program_id | path |  | Yes | integer |
| user_id | path |  | Yes | integer |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | OK |

##### Security

| Security Schema | Scopes |
| --- | --- |
| Authorization | |

### /programs/{program_id}/unassign/{user_id}

#### POST
##### Summary:

Unassign program from user (for company)

##### Description:

Unassign program from user (for company)

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| program_id | path |  | Yes | string |
| user_id | path |  | Yes | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | OK |

##### Security

| Security Schema | Scopes |
| --- | --- |
| Authorization | |

### /programs/{program_id}/participants

#### GET
##### Summary:

Get all program participants

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| program_id | path |  | Yes | integer |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | OK |

##### Security

| Security Schema | Scopes |
| --- | --- |
| Authorization | |

### /programs/{program_id}/invite/{username}

#### POST
##### Summary:

Invite hacker to program

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| program_id | path | program id | Yes | integer |
| username | path | hacker username | Yes | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | OK |

##### Security

| Security Schema | Scopes |
| --- | --- |
| Authorization | |

### /programs/{program_id}/invitations

#### GET
##### Summary:

Show all invitations of program (for program admin)

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| program_id | path |  | Yes | integer |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | OK |

##### Security

| Security Schema | Scopes |
| --- | --- |
| Authorization | |

### /programs/uninvite/{invitation_id}

#### GET
##### Summary:

Uninvite an invitation (todo: change to POST)

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| invitation_id | path |  | Yes | number |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | OK |

##### Security

| Security Schema | Scopes |
| --- | --- |
| Authorization | |

### /programs/accept/{invitation_id}

#### GET
##### Summary:

Accept program invitation (todo: change to POST)

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| invitation_id | path |  | Yes | string |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | OK |

##### Security

| Security Schema | Scopes |
| --- | --- |
| Authorization | |

### /programs/decline/{invitation_id}

#### GET
##### Summary:

Decline a program invitation (todo: change to POST)

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| invitation_id | path |  | Yes | integer |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | OK |

##### Security

| Security Schema | Scopes |
| --- | --- |
| Authorization | |

### /programs/{program_id}/remove_participant/{user_id}

#### GET
##### Summary:

Remove user from participant list (todo: change to POST)

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| program_id | path |  | Yes | integer |
| user_id | path |  | Yes | integer |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | OK |

##### Security

| Security Schema | Scopes |
| --- | --- |
| Authorization | |

### /hackers/profile

#### GET
##### Summary:

Get hacker profile

##### Description:

Return current user profile (for hacker)

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | OK |

##### Security

| Security Schema | Scopes |
| --- | --- |
| Authorization | |

### /hackers/update-profile

#### POST
##### Summary:

Update hacker profile

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | OK |

##### Security

| Security Schema | Scopes |
| --- | --- |
| Authorization | |

### /hackers/program_invitations

#### GET
##### Summary:

Get all program invitations (for hacker)

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | OK |

##### Security

| Security Schema | Scopes |
| --- | --- |
| Authorization | |

### /hackers/leave-program/{program_id}

#### GET
##### Summary:

Leave program (todo: change to POST)

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| program_id | path |  | Yes | integer |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | OK |

##### Security

| Security Schema | Scopes |
| --- | --- |
| Authorization | |

### /hackers/leave-company/{company_id}

#### GET
##### Summary:

Leave company (todo: change to POST)

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| company_id | path |  | Yes | integer |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | OK |

##### Security

| Security Schema | Scopes |
| --- | --- |
| Authorization | |

### /hackers/top

#### GET
##### Summary:

Get top hackers

##### Parameters

| Name | Located in | Description | Required | Schema |
| ---- | ---------- | ----------- | -------- | ---- |
| limit | query |  | No | integer |

##### Responses

| Code | Description |
| ---- | ----------- |
| 200 | OK |
