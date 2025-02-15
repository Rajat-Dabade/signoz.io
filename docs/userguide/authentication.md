---
id: authentication
title: Authentication and Login
sidebar_label: Authentication
---

Authentication is available in SigNoz from `v0.8.0` If you are on an earlier version, please upgrade to see this.

## Supported Roles
SigNoz currently supports 3 roles:
- Admin
- Editor
- Viewer

The person who installs SigNoz and registers for the first time is by default assigned the role of an admin.

- If you are logging in SigNoz for the first time, just create an account. This will make you an admin.
- If you would like to invite more members, they would need an invite link from admin. You can create invite link from `Settings-> Org Settings` tab

Admins can add new users by creating invites for them and sending them invite link to create an account.

![user-invite](../../static/img/docs/user-invite.png)


:::note

As of `version 0.8.0`, news users can only be invited by Admins to a SigNoz instance. New users will get an invite link from admin which they can use to signup to SigNoz.

When new user is invited by an admin, he can be assigned a role of Admin, Editor or Viewer 

:::

## How to Edit Member Details?

You can edit permission levels of members by going to `Settings-> Org Settings` tab and then Members table. 
You can also generate password reset link if they have forgotten their password and it needs to be reset.

![edit-member](../../static/img/docs/edit-member.png)


## Permission Matrix for Admin, Editor and Viewer:

| Features                                        | Admin | Editor | Viewer |
| ----------------------------------------------- | ----- | ------ | ------ |
| View Application List                           | ✅    | ✅     | ✅     |
| Search/Filter Application List                  | ✅    | ✅     | ✅     |
| View Metrics Detail Page                        | ✅    | ✅     | ✅     |
| View Dashboards                                 | ✅    | ✅     | ✅     |
| Create New Dashboards                           | ✅    | ✅     | ❌     |
| Import Dashboards                               | ✅    | ✅     | ❌     |
| Export Dashboards                               | ✅    | ✅     | ✅     |
| View Trace Filter Page & do Filtering           | ✅    | ✅     | ✅     |
| View Trace Detail Page                          | ✅    | ✅     | ✅     |
| View Alerts                                     | ✅    | ✅     | ✅     |
| Search / Filter Alerts                          | ✅    | ✅     | ✅     |
| Add New Alerts                                  | ✅    | ✅     | ❌     |
| View Settings Page                              | ✅    | ❌     | ❌     |
| View Service Map                                | ✅    | ✅     | ✅     |
| Invite New Members                              | ✅    | ❌     | ❌     |
| Revoke Invite of Members                        | ✅    | ❌     | ❌     |
| Create New Alert Channels                       | ✅    | ❌     | ❌     |
| Set Retention Period                            | ✅    | ❌     | ❌     |
| Set own Password and Name                       | ✅    | ✅     | ✅     |
| Change Org Name                                 | ✅    | ❌     | ❌     |
| Edit / Delete Member Details                    | ✅    | ❌     | ❌     |
| View Version Information Page (from left panel) | ✅    | ✅     | ✅     |
| Change Theme (dark/light)                       | ✅    | ✅     | ✅     |

