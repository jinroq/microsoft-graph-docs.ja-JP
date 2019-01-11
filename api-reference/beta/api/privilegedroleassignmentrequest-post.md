---
title: PrivilegedRoleAssignmentRequest を作成します。
description: Privilegedroleassignmentrequest オブジェクトを作成します。
localization_priority: Normal
ms.openlocfilehash: 3f1b88415e5671e38ad557cc28200569a42a9630
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27847770"
---
# <a name="create-privilegedroleassignmentrequest"></a><span data-ttu-id="a4d62-103">PrivilegedRoleAssignmentRequest を作成します。</span><span class="sxs-lookup"><span data-stu-id="a4d62-103">Create privilegedRoleAssignmentRequest</span></span>

> <span data-ttu-id="a4d62-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a4d62-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a4d62-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a4d62-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a4d62-106">[Privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="a4d62-106">Create a [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a4d62-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a4d62-107">Permissions</span></span>
<span data-ttu-id="a4d62-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a4d62-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4d62-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a4d62-110">Permission type</span></span>                        | <span data-ttu-id="a4d62-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a4d62-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="a4d62-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a4d62-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a4d62-113">PrivilegedAccess.ReadWrite.AzureAD、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a4d62-113">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a4d62-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a4d62-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a4d62-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a4d62-115">Not supported.</span></span> |
|<span data-ttu-id="a4d62-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a4d62-116">Application</span></span>                            | <span data-ttu-id="a4d62-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a4d62-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a4d62-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a4d62-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="a4d62-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a4d62-119">Request headers</span></span>
| <span data-ttu-id="a4d62-120">名前</span><span class="sxs-lookup"><span data-stu-id="a4d62-120">Name</span></span>      |<span data-ttu-id="a4d62-121">説明</span><span class="sxs-lookup"><span data-stu-id="a4d62-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a4d62-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4d62-122">Authorization</span></span>  | <span data-ttu-id="a4d62-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a4d62-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a4d62-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="a4d62-125">Request body</span></span>
<span data-ttu-id="a4d62-126">要求の本文には、 [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="a4d62-126">In the request body, supply a JSON representation of [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) object.</span></span> 

| <span data-ttu-id="a4d62-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a4d62-127">Property</span></span>     | <span data-ttu-id="a4d62-128">種類</span><span class="sxs-lookup"><span data-stu-id="a4d62-128">Type</span></span>    |  <span data-ttu-id="a4d62-129">説明</span><span class="sxs-lookup"><span data-stu-id="a4d62-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a4d62-130">roleId</span><span class="sxs-lookup"><span data-stu-id="a4d62-130">roleId</span></span>|<span data-ttu-id="a4d62-131">String</span><span class="sxs-lookup"><span data-stu-id="a4d62-131">String</span></span>|<span data-ttu-id="a4d62-132">ロールの ID です。</span><span class="sxs-lookup"><span data-stu-id="a4d62-132">The ID of the role.</span></span> <span data-ttu-id="a4d62-133">必須。</span><span class="sxs-lookup"><span data-stu-id="a4d62-133">Required.</span></span>|
|<span data-ttu-id="a4d62-134">type</span><span class="sxs-lookup"><span data-stu-id="a4d62-134">type</span></span>|<span data-ttu-id="a4d62-135">String</span><span class="sxs-lookup"><span data-stu-id="a4d62-135">String</span></span>|<span data-ttu-id="a4d62-136">表す、ロールの割り当ての操作の種類です。</span><span class="sxs-lookup"><span data-stu-id="a4d62-136">Represents the the type of the operation on the role assignment.</span></span> <span data-ttu-id="a4d62-137">値は、 `AdminAdd`: 管理者のユーザー ロールを追加します。`UserAdd`: ユーザーは、役割の割り当てを追加します。</span><span class="sxs-lookup"><span data-stu-id="a4d62-137">The value can be `AdminAdd`: Adminstrators add users to roles;`UserAdd`: Users add role assignments.</span></span> <span data-ttu-id="a4d62-138">必須。</span><span class="sxs-lookup"><span data-stu-id="a4d62-138">Required.</span></span>|
|<span data-ttu-id="a4d62-139">assignmentState</span><span class="sxs-lookup"><span data-stu-id="a4d62-139">assignmentState</span></span>|<span data-ttu-id="a4d62-140">String</span><span class="sxs-lookup"><span data-stu-id="a4d62-140">String</span></span>|<span data-ttu-id="a4d62-141">割り当ての状態です。</span><span class="sxs-lookup"><span data-stu-id="a4d62-141">The state of the assignment.</span></span> <span data-ttu-id="a4d62-142">値は、`Eligible`対象となる割り当ての`Active`が直接割り当てられている場合 -`Active`管理者、またはユーザーが対象となる割り当ての有効化します。</span><span class="sxs-lookup"><span data-stu-id="a4d62-142">The value can be `Eligible` for eligible assignment `Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span> <span data-ttu-id="a4d62-143">可能な値は、``NotStarted``、`Completed`、`RequestedApproval`、`Scheduled`、`Approved`、`ApprovalDenied`、`ApprovalAborted`、`Cancelling`、`Cancelled`、`Revoked`、`RequestExpired` です。</span><span class="sxs-lookup"><span data-stu-id="a4d62-143">Possible values are: ``NotStarted``, `Completed`, `RequestedApproval`, `Scheduled`, `Approved`, `ApprovalDenied`, `ApprovalAborted`, `Cancelling`, `Cancelled`, `Revoked`, `RequestExpired`.</span></span> <span data-ttu-id="a4d62-144">必須。</span><span class="sxs-lookup"><span data-stu-id="a4d62-144">Required.</span></span>|
|<span data-ttu-id="a4d62-145">理由</span><span class="sxs-lookup"><span data-stu-id="a4d62-145">reason</span></span>|<span data-ttu-id="a4d62-146">String</span><span class="sxs-lookup"><span data-stu-id="a4d62-146">String</span></span>|<span data-ttu-id="a4d62-147">理由は、監査の役割の割り当て要求に指定して目的を確認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a4d62-147">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span>|
|<span data-ttu-id="a4d62-148">スケジュール</span><span class="sxs-lookup"><span data-stu-id="a4d62-148">schedule</span></span>|[<span data-ttu-id="a4d62-149">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="a4d62-149">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="a4d62-150">役割の割り当て要求のスケジュールです。</span><span class="sxs-lookup"><span data-stu-id="a4d62-150">The schedule of the role assignment request.</span></span>|

## <a name="response"></a><span data-ttu-id="a4d62-151">応答</span><span class="sxs-lookup"><span data-stu-id="a4d62-151">Response</span></span>
<span data-ttu-id="a4d62-152">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="a4d62-152">If successful, this method returns a `201 Created` response code and a [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="a4d62-153">エラー コード</span><span class="sxs-lookup"><span data-stu-id="a4d62-153">Error codes</span></span>
<span data-ttu-id="a4d62-154">この API 規格を取得する HTTP エラー コードです。</span><span class="sxs-lookup"><span data-stu-id="a4d62-154">This API returns that standard HTTP error codes.</span></span> <span data-ttu-id="a4d62-155">さらに、次の表に記載されているエラー コードを返すことです。</span><span class="sxs-lookup"><span data-stu-id="a4d62-155">In addition, it can return the error codes listed in the following table.</span></span>

|<span data-ttu-id="a4d62-156">エラー コード</span><span class="sxs-lookup"><span data-stu-id="a4d62-156">Error code</span></span>     | <span data-ttu-id="a4d62-157">エラー メッセージ</span><span class="sxs-lookup"><span data-stu-id="a4d62-157">Error message</span></span>              | 
|:--------------------| :---------------------|
| <span data-ttu-id="a4d62-158">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a4d62-158">400 BadRequest</span></span> | <span data-ttu-id="a4d62-159">RoleAssignmentRequest プロパティが NULL をしました</span><span class="sxs-lookup"><span data-stu-id="a4d62-159">RoleAssignmentRequest property was NULL</span></span> |
| <span data-ttu-id="a4d62-160">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a4d62-160">400 BadRequest</span></span> | <span data-ttu-id="a4d62-161">RoleAssignmentRequest オブジェクトを逆シリアル化できません。</span><span class="sxs-lookup"><span data-stu-id="a4d62-161">Unable to deserialize roleAssignmentRequest Object.</span></span> |
| <span data-ttu-id="a4d62-162">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a4d62-162">400 BadRequest</span></span> | <span data-ttu-id="a4d62-163">RoleId は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="a4d62-163">RoleId is required.</span></span> |
| <span data-ttu-id="a4d62-164">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a4d62-164">400 BadRequest</span></span> | <span data-ttu-id="a4d62-165">スケジュールの開始日は指定する必要があり、今よりも大きい必要があります。</span><span class="sxs-lookup"><span data-stu-id="a4d62-165">Schedule start date must be specified and should be greater than Now.</span></span> |
| <span data-ttu-id="a4d62-166">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a4d62-166">400 BadRequest</span></span> | <span data-ttu-id="a4d62-167">このユーザー、ロール、およびスケジュールの種類のスケジュールが既に存在します。</span><span class="sxs-lookup"><span data-stu-id="a4d62-167">A schedule already exists for this user, role and schedule type.</span></span> |
| <span data-ttu-id="a4d62-168">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a4d62-168">400 BadRequest</span></span> | <span data-ttu-id="a4d62-169">既に保留中の承認は、このユーザー、ロール、および承認の種類に存在します。</span><span class="sxs-lookup"><span data-stu-id="a4d62-169">A pending approval already exists for this user, role and approval type.</span></span> |
| <span data-ttu-id="a4d62-170">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a4d62-170">400 BadRequest</span></span> | <span data-ttu-id="a4d62-171">リクエスターの理由はされていません。</span><span class="sxs-lookup"><span data-stu-id="a4d62-171">Requestor reason is missing.</span></span> |
| <span data-ttu-id="a4d62-172">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a4d62-172">400 BadRequest</span></span> | <span data-ttu-id="a4d62-173">リクエスターの理由は、500 文字未満にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="a4d62-173">Requestor reason should be less than 500 characters.</span></span> |
| <span data-ttu-id="a4d62-174">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a4d62-174">400 BadRequest</span></span> | <span data-ttu-id="a4d62-175">昇格期間は、0.5 の間で、{の設定} からである必要があります。</span><span class="sxs-lookup"><span data-stu-id="a4d62-175">Elevation duration must be between 0.5 and {from setting}.</span></span> |
| <span data-ttu-id="a4d62-176">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a4d62-176">400 BadRequest</span></span> | <span data-ttu-id="a4d62-177">スケジュールのアクティブ化と要求との間の重複があります。</span><span class="sxs-lookup"><span data-stu-id="a4d62-177">There is a overlap between scheduled activation and the request.</span></span> |
| <span data-ttu-id="a4d62-178">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a4d62-178">400 BadRequest</span></span> | <span data-ttu-id="a4d62-179">ロールが既にアクティブになっています。</span><span class="sxs-lookup"><span data-stu-id="a4d62-179">The role is already activated.</span></span> |
| <span data-ttu-id="a4d62-180">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a4d62-180">400 BadRequest</span></span> | <span data-ttu-id="a4d62-181">GenericElevateUserToRoleAssignments: Tickting の情報は必要し、ライセンス認証プロセスで指定されていません。</span><span class="sxs-lookup"><span data-stu-id="a4d62-181">GenericElevateUserToRoleAssignments: Tickting information is required and not supplied in the activation process.</span></span> |
| <span data-ttu-id="a4d62-182">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a4d62-182">400 BadRequest</span></span> | <span data-ttu-id="a4d62-183">スケジュールのアクティブ化と要求との間の重複があります。</span><span class="sxs-lookup"><span data-stu-id="a4d62-183">There is a overlap between scheduled activation and the request.</span></span> |
| <span data-ttu-id="a4d62-184">403 許可されていません。</span><span class="sxs-lookup"><span data-stu-id="a4d62-184">403 UnAuthorized</span></span> | <span data-ttu-id="a4d62-185">昇格時に、複数要素の認証が必要です。</span><span class="sxs-lookup"><span data-stu-id="a4d62-185">Elevation requires Multi-Factor Authentication.</span></span> |
| <span data-ttu-id="a4d62-186">403 許可されていません。</span><span class="sxs-lookup"><span data-stu-id="a4d62-186">403 UnAuthorized</span></span> | <span data-ttu-id="a4d62-187">昇格のため許可されていません。</span><span class="sxs-lookup"><span data-stu-id="a4d62-187">On behalf of elevation is not allowed.</span></span> |

## <a name="example"></a><span data-ttu-id="a4d62-188">例</span><span class="sxs-lookup"><span data-stu-id="a4d62-188">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a4d62-189">要求</span><span class="sxs-lookup"><span data-stu-id="a4d62-189">Request</span></span>
<span data-ttu-id="a4d62-190">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a4d62-190">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_privilegedroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests
Content-type: application/json

{
    "duration": "2",
    "reason": "Activate the role for business purpose",
    "ticketNumber": "234",
    "ticketSystem": "system",
    "schedule": {
        "startDateTime": "2018-02-08T02:35:17.903Z"
    },
    "evaluateOnly": false,
    "type": "UserAdd",
    "assignmentState": "Active",
    "roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
}
```
##### <a name="response"></a><span data-ttu-id="a4d62-191">応答</span><span class="sxs-lookup"><span data-stu-id="a4d62-191">Response</span></span>
<span data-ttu-id="a4d62-192">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a4d62-192">The following is an example of the response.</span></span> <span data-ttu-id="a4d62-193">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="a4d62-193">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="a4d62-194">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="a4d62-194">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignmentRequest"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 304


{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#privilegedRoleAssignmentRequests/$entity",
    "schedule": {
        "type": "activation",
        "startDateTime": "2018-02-08T02:35:17.903Z",
        "endDateTime": null,
        "duration" : null
    },
    "id": "e13ef8a0-c1cb-4d03-aaae-9cd1c8ede2d1",
    "evaluateOnly": false,
    "type": "UserAdd",
    "assignmentState": "Active",
    "requestedDateTime": "2018-02-08T02:35:42.9137335Z",
    "status": "NotStarted",
    "duration": "2",
    "reason": "Activate the role for business purpose",
    "ticketNumber": "234",
    "ticketSystem": "system",
    "userId": "Self"，
    "roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Post privilegedRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
