---
title: PrivilegedRoleAssignmentRequest を作成します。
description: Privilegedroleassignmentrequest オブジェクトを作成します。
localization_priority: Normal
ms.openlocfilehash: e3158e918d061f09dec9e74c9e3bfd66d95fa48d
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641688"
---
# <a name="create-privilegedroleassignmentrequest"></a><span data-ttu-id="a76ad-103">PrivilegedRoleAssignmentRequest を作成します。</span><span class="sxs-lookup"><span data-stu-id="a76ad-103">Create privilegedRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a76ad-104">[Privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="a76ad-104">Create a [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a76ad-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a76ad-105">Permissions</span></span>
<span data-ttu-id="a76ad-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a76ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a76ad-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a76ad-108">Permission type</span></span>                        | <span data-ttu-id="a76ad-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a76ad-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="a76ad-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a76ad-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a76ad-111">PrivilegedAccess.ReadWrite.AzureAD、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a76ad-111">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a76ad-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a76ad-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a76ad-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a76ad-113">Not supported.</span></span> |
|<span data-ttu-id="a76ad-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a76ad-114">Application</span></span>                            | <span data-ttu-id="a76ad-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a76ad-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a76ad-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a76ad-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="a76ad-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a76ad-117">Request headers</span></span>
| <span data-ttu-id="a76ad-118">名前</span><span class="sxs-lookup"><span data-stu-id="a76ad-118">Name</span></span>      |<span data-ttu-id="a76ad-119">説明</span><span class="sxs-lookup"><span data-stu-id="a76ad-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a76ad-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="a76ad-120">Authorization</span></span>  | <span data-ttu-id="a76ad-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a76ad-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a76ad-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="a76ad-123">Request body</span></span>
<span data-ttu-id="a76ad-124">要求の本文には、 [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="a76ad-124">In the request body, supply a JSON representation of [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) object.</span></span> 

| <span data-ttu-id="a76ad-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a76ad-125">Property</span></span>     | <span data-ttu-id="a76ad-126">型</span><span class="sxs-lookup"><span data-stu-id="a76ad-126">Type</span></span>    |  <span data-ttu-id="a76ad-127">説明</span><span class="sxs-lookup"><span data-stu-id="a76ad-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a76ad-128">roleId</span><span class="sxs-lookup"><span data-stu-id="a76ad-128">roleId</span></span>|<span data-ttu-id="a76ad-129">String</span><span class="sxs-lookup"><span data-stu-id="a76ad-129">String</span></span>|<span data-ttu-id="a76ad-130">ロールの ID です。</span><span class="sxs-lookup"><span data-stu-id="a76ad-130">The ID of the role.</span></span> <span data-ttu-id="a76ad-131">必須。</span><span class="sxs-lookup"><span data-stu-id="a76ad-131">Required.</span></span>|
|<span data-ttu-id="a76ad-132">type</span><span class="sxs-lookup"><span data-stu-id="a76ad-132">type</span></span>|<span data-ttu-id="a76ad-133">String</span><span class="sxs-lookup"><span data-stu-id="a76ad-133">String</span></span>|<span data-ttu-id="a76ad-134">表す、ロールの割り当ての操作の種類です。</span><span class="sxs-lookup"><span data-stu-id="a76ad-134">Represents the the type of the operation on the role assignment.</span></span> <span data-ttu-id="a76ad-135">値は、 `AdminAdd`: 管理者のユーザー ロールを追加します。`UserAdd`: ユーザーは、役割の割り当てを追加します。</span><span class="sxs-lookup"><span data-stu-id="a76ad-135">The value can be `AdminAdd`: Adminstrators add users to roles;`UserAdd`: Users add role assignments.</span></span> <span data-ttu-id="a76ad-136">必須です。</span><span class="sxs-lookup"><span data-stu-id="a76ad-136">Required.</span></span>|
|<span data-ttu-id="a76ad-137">assignmentState</span><span class="sxs-lookup"><span data-stu-id="a76ad-137">assignmentState</span></span>|<span data-ttu-id="a76ad-138">String</span><span class="sxs-lookup"><span data-stu-id="a76ad-138">String</span></span>|<span data-ttu-id="a76ad-139">割り当ての状態です。</span><span class="sxs-lookup"><span data-stu-id="a76ad-139">The state of the assignment.</span></span> <span data-ttu-id="a76ad-140">値は、`Eligible`対象となる割り当ての`Active`が直接割り当てられている場合 -`Active`管理者、またはユーザーが対象となる割り当ての有効化します。</span><span class="sxs-lookup"><span data-stu-id="a76ad-140">The value can be `Eligible` for eligible assignment `Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span> <span data-ttu-id="a76ad-141">可能な値は、``NotStarted``、`Completed`、`RequestedApproval`、`Scheduled`、`Approved`、`ApprovalDenied`、`ApprovalAborted`、`Cancelling`、`Cancelled`、`Revoked`、`RequestExpired` です。</span><span class="sxs-lookup"><span data-stu-id="a76ad-141">Possible values are: ``NotStarted``, `Completed`, `RequestedApproval`, `Scheduled`, `Approved`, `ApprovalDenied`, `ApprovalAborted`, `Cancelling`, `Cancelled`, `Revoked`, `RequestExpired`.</span></span> <span data-ttu-id="a76ad-142">必須です。</span><span class="sxs-lookup"><span data-stu-id="a76ad-142">Required.</span></span>|
|<span data-ttu-id="a76ad-143">理由</span><span class="sxs-lookup"><span data-stu-id="a76ad-143">reason</span></span>|<span data-ttu-id="a76ad-144">String</span><span class="sxs-lookup"><span data-stu-id="a76ad-144">String</span></span>|<span data-ttu-id="a76ad-145">理由は、監査の役割の割り当て要求に指定して目的を確認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a76ad-145">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span>|
|<span data-ttu-id="a76ad-146">スケジュール</span><span class="sxs-lookup"><span data-stu-id="a76ad-146">schedule</span></span>|[<span data-ttu-id="a76ad-147">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="a76ad-147">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="a76ad-148">役割の割り当て要求のスケジュールです。</span><span class="sxs-lookup"><span data-stu-id="a76ad-148">The schedule of the role assignment request.</span></span>|

## <a name="response"></a><span data-ttu-id="a76ad-149">応答</span><span class="sxs-lookup"><span data-stu-id="a76ad-149">Response</span></span>
<span data-ttu-id="a76ad-150">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="a76ad-150">If successful, this method returns a `201 Created` response code and a [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="a76ad-151">エラー コード</span><span class="sxs-lookup"><span data-stu-id="a76ad-151">Error codes</span></span>
<span data-ttu-id="a76ad-152">この API 規格を取得する HTTP エラー コードです。</span><span class="sxs-lookup"><span data-stu-id="a76ad-152">This API returns that standard HTTP error codes.</span></span> <span data-ttu-id="a76ad-153">さらに、次の表に記載されているエラー コードを返すことです。</span><span class="sxs-lookup"><span data-stu-id="a76ad-153">In addition, it can return the error codes listed in the following table.</span></span>

|<span data-ttu-id="a76ad-154">エラー コード</span><span class="sxs-lookup"><span data-stu-id="a76ad-154">Error code</span></span>     | <span data-ttu-id="a76ad-155">エラー メッセージ</span><span class="sxs-lookup"><span data-stu-id="a76ad-155">Error message</span></span>              | 
|:--------------------| :---------------------|
| <span data-ttu-id="a76ad-156">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a76ad-156">400 BadRequest</span></span> | <span data-ttu-id="a76ad-157">RoleAssignmentRequest プロパティが NULL をしました</span><span class="sxs-lookup"><span data-stu-id="a76ad-157">RoleAssignmentRequest property was NULL</span></span> |
| <span data-ttu-id="a76ad-158">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a76ad-158">400 BadRequest</span></span> | <span data-ttu-id="a76ad-159">RoleAssignmentRequest オブジェクトを逆シリアル化できません。</span><span class="sxs-lookup"><span data-stu-id="a76ad-159">Unable to deserialize roleAssignmentRequest Object.</span></span> |
| <span data-ttu-id="a76ad-160">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a76ad-160">400 BadRequest</span></span> | <span data-ttu-id="a76ad-161">RoleId は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="a76ad-161">RoleId is required.</span></span> |
| <span data-ttu-id="a76ad-162">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a76ad-162">400 BadRequest</span></span> | <span data-ttu-id="a76ad-163">スケジュールの開始日は指定する必要があり、今よりも大きい必要があります。</span><span class="sxs-lookup"><span data-stu-id="a76ad-163">Schedule start date must be specified and should be greater than Now.</span></span> |
| <span data-ttu-id="a76ad-164">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a76ad-164">400 BadRequest</span></span> | <span data-ttu-id="a76ad-165">このユーザー、ロール、およびスケジュールの種類のスケジュールが既に存在します。</span><span class="sxs-lookup"><span data-stu-id="a76ad-165">A schedule already exists for this user, role and schedule type.</span></span> |
| <span data-ttu-id="a76ad-166">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a76ad-166">400 BadRequest</span></span> | <span data-ttu-id="a76ad-167">既に保留中の承認は、このユーザー、ロール、および承認の種類に存在します。</span><span class="sxs-lookup"><span data-stu-id="a76ad-167">A pending approval already exists for this user, role and approval type.</span></span> |
| <span data-ttu-id="a76ad-168">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a76ad-168">400 BadRequest</span></span> | <span data-ttu-id="a76ad-169">リクエスターの理由はされていません。</span><span class="sxs-lookup"><span data-stu-id="a76ad-169">Requestor reason is missing.</span></span> |
| <span data-ttu-id="a76ad-170">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a76ad-170">400 BadRequest</span></span> | <span data-ttu-id="a76ad-171">リクエスターの理由は、500 文字未満にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="a76ad-171">Requestor reason should be less than 500 characters.</span></span> |
| <span data-ttu-id="a76ad-172">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a76ad-172">400 BadRequest</span></span> | <span data-ttu-id="a76ad-173">昇格期間は、0.5 の間で、{の設定} からである必要があります。</span><span class="sxs-lookup"><span data-stu-id="a76ad-173">Elevation duration must be between 0.5 and {from setting}.</span></span> |
| <span data-ttu-id="a76ad-174">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a76ad-174">400 BadRequest</span></span> | <span data-ttu-id="a76ad-175">スケジュールのアクティブ化と要求との間の重複があります。</span><span class="sxs-lookup"><span data-stu-id="a76ad-175">There is a overlap between scheduled activation and the request.</span></span> |
| <span data-ttu-id="a76ad-176">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a76ad-176">400 BadRequest</span></span> | <span data-ttu-id="a76ad-177">ロールが既にアクティブになっています。</span><span class="sxs-lookup"><span data-stu-id="a76ad-177">The role is already activated.</span></span> |
| <span data-ttu-id="a76ad-178">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a76ad-178">400 BadRequest</span></span> | <span data-ttu-id="a76ad-179">GenericElevateUserToRoleAssignments: Tickting の情報は必要し、ライセンス認証プロセスで指定されていません。</span><span class="sxs-lookup"><span data-stu-id="a76ad-179">GenericElevateUserToRoleAssignments: Tickting information is required and not supplied in the activation process.</span></span> |
| <span data-ttu-id="a76ad-180">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a76ad-180">400 BadRequest</span></span> | <span data-ttu-id="a76ad-181">スケジュールのアクティブ化と要求との間の重複があります。</span><span class="sxs-lookup"><span data-stu-id="a76ad-181">There is a overlap between scheduled activation and the request.</span></span> |
| <span data-ttu-id="a76ad-182">403 許可されていません。</span><span class="sxs-lookup"><span data-stu-id="a76ad-182">403 UnAuthorized</span></span> | <span data-ttu-id="a76ad-183">昇格時に、複数要素の認証が必要です。</span><span class="sxs-lookup"><span data-stu-id="a76ad-183">Elevation requires Multi-Factor Authentication.</span></span> |
| <span data-ttu-id="a76ad-184">403 許可されていません。</span><span class="sxs-lookup"><span data-stu-id="a76ad-184">403 UnAuthorized</span></span> | <span data-ttu-id="a76ad-185">昇格のため許可されていません。</span><span class="sxs-lookup"><span data-stu-id="a76ad-185">On behalf of elevation is not allowed.</span></span> |

## <a name="example"></a><span data-ttu-id="a76ad-186">例</span><span class="sxs-lookup"><span data-stu-id="a76ad-186">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a76ad-187">要求</span><span class="sxs-lookup"><span data-stu-id="a76ad-187">Request</span></span>
<span data-ttu-id="a76ad-188">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a76ad-188">The following is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="a76ad-189">応答</span><span class="sxs-lookup"><span data-stu-id="a76ad-189">Response</span></span>
<span data-ttu-id="a76ad-190">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a76ad-190">The following is an example of the response.</span></span> <span data-ttu-id="a76ad-191">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="a76ad-191">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="a76ad-192">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="a76ad-192">All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Post privilegedRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedroleassignmentrequest-post.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
