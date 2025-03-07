---
title: Attach and detach permissions for users, roles, and groups for Amazon Web Services (AWS) identities in the Remediation dashboard in CloudKnox Permissions Management
description: How to attach and detach permissions for users, roles, and groups for Amazon Web Services (AWS) identities in the Remediation dashboard in CloudKnox Permissions Management.
services: active-directory
author: mtillman
manager: karenh444
ms.service: active-directory
ms.subservice: ciem
ms.workload: identity
ms.topic: how-to
ms.date: 02/23/2022
ms.author: mtillman
---

# Attach and detach policies for Amazon Web Services (AWS) identities 


> [!IMPORTANT]
> CloudKnox Permissions Management (CloudKnox) is currently in PREVIEW.
> Some information relates to a prerelease product that may be substantially modified before it's released. Microsoft makes no warranties, express or implied, with respect to the information provided here.

This article describes how you can attach and detach permissions for users, roles, and groups for Amazon Web Services (AWS) identities using the **Remediation** dashboard.

> [!NOTE]
> To view the **Remediation** tab, your must have **Viewer**, **Controller**, or **Administrator** permissions. To make changes on this tab, you must have **Controller** or **Administrator** permissions. If you don’t have these permissions, contact your system administrator.

## View permissions

1. On the CloudKnox home page, select the **Remediation** tab, and then select the **Permissions** subtab.
1. From the **Authorization System Type** dropdown, select **AWS**.
1. From the **Authorization System** dropdown, select the accounts you want to access.
1. From the **Search For** dropdown, select **Group**, **User**, or **Role**.
1. To search for more parameters, you can make a selection from the **User States**, **Permission Creep Index**, and **Task Usage** dropdowns.
1. Select **Apply**.
    CloudKnox displays a list of users, roles, or groups that match your criteria.
1. In **Enter a username**, enter or select a user.
1. In **Enter a group name**, enter or select a group, then select **Apply**.
1. Make a selection from the results list.

    The table displays the related **Username** **Domain/Account**, **Source** and **Policy Name**.


## Attach policies

1. On the CloudKnox home page, select the **Remediation** tab, and then select the **Permissions** subtab.
1. From the **Authorization System Type** dropdown, select **AWS**.
1. In **Enter a username**, enter or select a user.
1. In **Enter a Group Name**, enter or select a group, then select **Apply**.
1. Make a selection from the results list.
1. To attach a policy, select **Attach Policies**.
1. In the **Attach Policies** page, from the **Available policies** list, select the plus sign **(+)** to move the policy to the **Selected policies** list. 
1. When you have finished adding policies, select **Submit**.
1. When the following message displays: **Are you sure you want to change permission?**, select: 
    - **Generate Script** to generate a script where you can manually add/remove the permissions you selected.
    - **Execute** to change the permission.
    - **Close** to cancel the action.

## Detach policies

1. On the CloudKnox home page, select the **Remediation** tab, and then select the **Permissions** subtab.
1. From the **Authorization System Type** dropdown, select **AWS**.
1. In **Enter a username**, enter or select a user.
1. In **Enter a Group Name**, enter or select a group, then select **Apply**.
1. Make a selection from the results list.
1. To remove a policy, select **Detach Policies**.
1. In the **Detach Policies** page, from the **Available policies** list, select the plus sign **(+)** to move the policy to the **Selected policies** list. 
1. When you have finished selecting policies, select **Submit**.
1. When the following message displays: **Are you sure you want to change permission?**, select: 
    - **Generate Script** to generate a script where you can manually add/remove the permissions you selected.
    - **Execute** to change the permission.
    - **Close** to cancel the action.

## Next steps


- For information on how to view existing roles/policies, requests, and permissions, see [View roles/policies, requests, and permission in the Remediation dashboard](cloudknox-ui-remediation.md).
- For information on how to create a role/policy, see [Create a role/policy](cloudknox-howto-create-role-policy.md).
- For information on how to clone a role/policy, see [Clone a role/policy](cloudknox-howto-clone-role-policy.md).
- For information on how to delete a role/policy, see [Delete a role/policy](cloudknox-howto-delete-role-policy.md).
- For information on how to modify a role/policy, see Modify a role/policy](cloudknox-howto-modify-role-policy.md).
- To view information about roles/policies, see [View information about roles/policies](cloudknox-howto-view-role-policy.md).
- For information on how to revoke high-risk and unused tasks or assign read-only status for Microsoft Azure and Google Cloud Platform (GCP) identities, see [Revoke high-risk and unused tasks or assign read-only status for Azure and GCP identities](cloudknox-howto-revoke-task-readonly-status.md)
For information on how to create or approve a request for permissions, see [Create or approve a request for permissions](cloudknox-howto-create-approve-privilege-request.md).

