---
title: PrivilegedRoleAssignmentRequest を作成する
description: Privilegedroleassignmentrequest オブジェクトを作成します。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: ea9158154aaa528f90be03a153ff1e74c650e14c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35978694"
---
# <a name="create-privilegedroleassignmentrequest"></a><span data-ttu-id="2be67-103">PrivilegedRoleAssignmentRequest を作成する</span><span class="sxs-lookup"><span data-stu-id="2be67-103">Create privilegedRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2be67-104">[Privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="2be67-104">Create a [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2be67-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2be67-105">Permissions</span></span>
<span data-ttu-id="2be67-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2be67-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2be67-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2be67-108">Permission type</span></span>                        | <span data-ttu-id="2be67-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2be67-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="2be67-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2be67-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2be67-111">PrivilegedAccess、AzureAD、および Directory.accessasuser.all。</span><span class="sxs-lookup"><span data-stu-id="2be67-111">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2be67-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2be67-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2be67-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2be67-113">Not supported.</span></span> |
|<span data-ttu-id="2be67-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2be67-114">Application</span></span>                            | <span data-ttu-id="2be67-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2be67-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2be67-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2be67-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="2be67-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2be67-117">Request headers</span></span>
| <span data-ttu-id="2be67-118">名前</span><span class="sxs-lookup"><span data-stu-id="2be67-118">Name</span></span>      |<span data-ttu-id="2be67-119">説明</span><span class="sxs-lookup"><span data-stu-id="2be67-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2be67-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="2be67-120">Authorization</span></span>  | <span data-ttu-id="2be67-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2be67-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2be67-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="2be67-123">Request body</span></span>
<span data-ttu-id="2be67-124">要求本文で、 [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="2be67-124">In the request body, supply a JSON representation of [privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) object.</span></span> 

| <span data-ttu-id="2be67-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2be67-125">Property</span></span>     | <span data-ttu-id="2be67-126">型</span><span class="sxs-lookup"><span data-stu-id="2be67-126">Type</span></span>    |  <span data-ttu-id="2be67-127">説明</span><span class="sxs-lookup"><span data-stu-id="2be67-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2be67-128">roleId</span><span class="sxs-lookup"><span data-stu-id="2be67-128">roleId</span></span>|<span data-ttu-id="2be67-129">String</span><span class="sxs-lookup"><span data-stu-id="2be67-129">String</span></span>|<span data-ttu-id="2be67-130">ロールの ID。</span><span class="sxs-lookup"><span data-stu-id="2be67-130">The ID of the role.</span></span> <span data-ttu-id="2be67-131">必須。</span><span class="sxs-lookup"><span data-stu-id="2be67-131">Required.</span></span>|
|<span data-ttu-id="2be67-132">type</span><span class="sxs-lookup"><span data-stu-id="2be67-132">type</span></span>|<span data-ttu-id="2be67-133">String</span><span class="sxs-lookup"><span data-stu-id="2be67-133">String</span></span>|<span data-ttu-id="2be67-134">役割の割り当てに対する操作の種類を表します。</span><span class="sxs-lookup"><span data-stu-id="2be67-134">Represents the type of the operation on the role assignment.</span></span> <span data-ttu-id="2be67-135">値は次の`AdminAdd`ようになります。管理者が役割にユーザーを追加します。`UserAdd`: ユーザーが役割の割り当てを追加します。</span><span class="sxs-lookup"><span data-stu-id="2be67-135">The value can be `AdminAdd`: Administrators add users to roles;`UserAdd`: Users add role assignments.</span></span> <span data-ttu-id="2be67-136">必須です。</span><span class="sxs-lookup"><span data-stu-id="2be67-136">Required.</span></span>|
|<span data-ttu-id="2be67-137">割り当ての状態</span><span class="sxs-lookup"><span data-stu-id="2be67-137">assignmentState</span></span>|<span data-ttu-id="2be67-138">String</span><span class="sxs-lookup"><span data-stu-id="2be67-138">String</span></span>|<span data-ttu-id="2be67-139">割り当ての状態を指定します。</span><span class="sxs-lookup"><span data-stu-id="2be67-139">The state of the assignment.</span></span> <span data-ttu-id="2be67-140">この値は、 `Eligible`管理者に`Active`よって直接割り当てら`Active`れている場合、またはユーザーによる資格のある割り当てに対してアクティブ化されている場合に、対象となる割り当てに使用できます。</span><span class="sxs-lookup"><span data-stu-id="2be67-140">The value can be `Eligible` for eligible assignment `Active` - if it is directly assigned `Active` by administrators, or activated on an eligible assignment by the users.</span></span> <span data-ttu-id="2be67-141">使用可能な値は、``NotStarted``、`Completed`、`RequestedApproval`、`Scheduled`、`Approved`、`ApprovalDenied`、`ApprovalAborted`、`Cancelling`、`Cancelled`、`Revoked`、`RequestExpired` です。</span><span class="sxs-lookup"><span data-stu-id="2be67-141">Possible values are: ``NotStarted``, `Completed`, `RequestedApproval`, `Scheduled`, `Approved`, `ApprovalDenied`, `ApprovalAborted`, `Cancelling`, `Cancelled`, `Revoked`, `RequestExpired`.</span></span> <span data-ttu-id="2be67-142">必須です。</span><span class="sxs-lookup"><span data-stu-id="2be67-142">Required.</span></span>|
|<span data-ttu-id="2be67-143">したがっ</span><span class="sxs-lookup"><span data-stu-id="2be67-143">reason</span></span>|<span data-ttu-id="2be67-144">String</span><span class="sxs-lookup"><span data-stu-id="2be67-144">String</span></span>|<span data-ttu-id="2be67-145">監査およびレビューの目的で、役割の割り当て要求に対して理由を提供する必要があります。</span><span class="sxs-lookup"><span data-stu-id="2be67-145">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span>|
|<span data-ttu-id="2be67-146">schedule</span><span class="sxs-lookup"><span data-stu-id="2be67-146">schedule</span></span>|[<span data-ttu-id="2be67-147">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="2be67-147">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="2be67-148">役割の割り当て要求のスケジュール。</span><span class="sxs-lookup"><span data-stu-id="2be67-148">The schedule of the role assignment request.</span></span>|

## <a name="response"></a><span data-ttu-id="2be67-149">応答</span><span class="sxs-lookup"><span data-stu-id="2be67-149">Response</span></span>
<span data-ttu-id="2be67-150">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2be67-150">If successful, this method returns a `201 Created` response code and a [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="2be67-151">エラー コード</span><span class="sxs-lookup"><span data-stu-id="2be67-151">Error codes</span></span>
<span data-ttu-id="2be67-152">この API は、その標準の HTTP エラーコードを返します。</span><span class="sxs-lookup"><span data-stu-id="2be67-152">This API returns that standard HTTP error codes.</span></span> <span data-ttu-id="2be67-153">また、次の表に示されているエラーコードを返すこともできます。</span><span class="sxs-lookup"><span data-stu-id="2be67-153">In addition, it can return the error codes listed in the following table.</span></span>

|<span data-ttu-id="2be67-154">エラー コード</span><span class="sxs-lookup"><span data-stu-id="2be67-154">Error code</span></span>     | <span data-ttu-id="2be67-155">エラー メッセージ</span><span class="sxs-lookup"><span data-stu-id="2be67-155">Error message</span></span>              | 
|:--------------------| :---------------------|
| <span data-ttu-id="2be67-156">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="2be67-156">400 BadRequest</span></span> | <span data-ttu-id="2be67-157">Role割り当て要求プロパティが NULL でした</span><span class="sxs-lookup"><span data-stu-id="2be67-157">RoleAssignmentRequest property was NULL</span></span> |
| <span data-ttu-id="2be67-158">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="2be67-158">400 BadRequest</span></span> | <span data-ttu-id="2be67-159">Role割り当て要求オブジェクトをシリアル化解除できません。</span><span class="sxs-lookup"><span data-stu-id="2be67-159">Unable to deserialize roleAssignmentRequest Object.</span></span> |
| <span data-ttu-id="2be67-160">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="2be67-160">400 BadRequest</span></span> | <span data-ttu-id="2be67-161">RoleId が必要です。</span><span class="sxs-lookup"><span data-stu-id="2be67-161">RoleId is required.</span></span> |
| <span data-ttu-id="2be67-162">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="2be67-162">400 BadRequest</span></span> | <span data-ttu-id="2be67-163">スケジュールの開始日を指定する必要があります。これより大きい値を指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="2be67-163">Schedule start date must be specified and should be greater than Now.</span></span> |
| <span data-ttu-id="2be67-164">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="2be67-164">400 BadRequest</span></span> | <span data-ttu-id="2be67-165">このユーザー、役割、およびスケジュールの種類に対するスケジュールが既に存在します。</span><span class="sxs-lookup"><span data-stu-id="2be67-165">A schedule already exists for this user, role and schedule type.</span></span> |
| <span data-ttu-id="2be67-166">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="2be67-166">400 BadRequest</span></span> | <span data-ttu-id="2be67-167">このユーザー、ロール、承認の種類に対して、保留中の承認が既に存在します。</span><span class="sxs-lookup"><span data-stu-id="2be67-167">A pending approval already exists for this user, role and approval type.</span></span> |
| <span data-ttu-id="2be67-168">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="2be67-168">400 BadRequest</span></span> | <span data-ttu-id="2be67-169">要求者の理由がありません。</span><span class="sxs-lookup"><span data-stu-id="2be67-169">Requestor reason is missing.</span></span> |
| <span data-ttu-id="2be67-170">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="2be67-170">400 BadRequest</span></span> | <span data-ttu-id="2be67-171">要求者の理由は、500文字未満である必要があります。</span><span class="sxs-lookup"><span data-stu-id="2be67-171">Requestor reason should be less than 500 characters.</span></span> |
| <span data-ttu-id="2be67-172">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="2be67-172">400 BadRequest</span></span> | <span data-ttu-id="2be67-173">昇格期間は0.5 と {from 設定} の間である必要があります。</span><span class="sxs-lookup"><span data-stu-id="2be67-173">Elevation duration must be between 0.5 and {from setting}.</span></span> |
| <span data-ttu-id="2be67-174">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="2be67-174">400 BadRequest</span></span> | <span data-ttu-id="2be67-175">スケジュールされたライセンス認証と要求の間に重複があります。</span><span class="sxs-lookup"><span data-stu-id="2be67-175">There is a overlap between scheduled activation and the request.</span></span> |
| <span data-ttu-id="2be67-176">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="2be67-176">400 BadRequest</span></span> | <span data-ttu-id="2be67-177">このロールは、あらかじめアクティブ化されています。</span><span class="sxs-lookup"><span data-stu-id="2be67-177">The role is already activated.</span></span> |
| <span data-ttu-id="2be67-178">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="2be67-178">400 BadRequest</span></span> | <span data-ttu-id="2be67-179">GenericElevateUserToRoleAssignments: Tickting 情報は必須であり、アクティブ化プロセスでは提供されていません。</span><span class="sxs-lookup"><span data-stu-id="2be67-179">GenericElevateUserToRoleAssignments: Tickting information is required and not supplied in the activation process.</span></span> |
| <span data-ttu-id="2be67-180">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="2be67-180">400 BadRequest</span></span> | <span data-ttu-id="2be67-181">スケジュールされたライセンス認証と要求の間に重複があります。</span><span class="sxs-lookup"><span data-stu-id="2be67-181">There is a overlap between scheduled activation and the request.</span></span> |
| <span data-ttu-id="2be67-182">403権限がありません</span><span class="sxs-lookup"><span data-stu-id="2be67-182">403 UnAuthorized</span></span> | <span data-ttu-id="2be67-183">昇格には多要素認証が必要です。</span><span class="sxs-lookup"><span data-stu-id="2be67-183">Elevation requires Multi-Factor Authentication.</span></span> |
| <span data-ttu-id="2be67-184">403権限がありません</span><span class="sxs-lookup"><span data-stu-id="2be67-184">403 UnAuthorized</span></span> | <span data-ttu-id="2be67-185">昇格の代理人は許可されていません。</span><span class="sxs-lookup"><span data-stu-id="2be67-185">On behalf of elevation is not allowed.</span></span> |

## <a name="example"></a><span data-ttu-id="2be67-186">例</span><span class="sxs-lookup"><span data-stu-id="2be67-186">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2be67-187">要求</span><span class="sxs-lookup"><span data-stu-id="2be67-187">Request</span></span>
<span data-ttu-id="2be67-188">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2be67-188">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2be67-189">プロトコル</span><span class="sxs-lookup"><span data-stu-id="2be67-189">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="2be67-190">C#</span><span class="sxs-lookup"><span data-stu-id="2be67-190">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-privilegedroleassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2be67-191">Javascript</span><span class="sxs-lookup"><span data-stu-id="2be67-191">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-privilegedroleassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2be67-192">目的-C</span><span class="sxs-lookup"><span data-stu-id="2be67-192">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-privilegedroleassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="2be67-193">Java</span><span class="sxs-lookup"><span data-stu-id="2be67-193">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-privilegedroleassignmentrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2be67-194">応答</span><span class="sxs-lookup"><span data-stu-id="2be67-194">Response</span></span>
<span data-ttu-id="2be67-195">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2be67-195">The following is an example of the response.</span></span> <span data-ttu-id="2be67-196">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="2be67-196">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="2be67-197">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="2be67-197">All of the properties will be returned from an actual call.</span></span>
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
    "userId": "Self",
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
  ]
}
-->
