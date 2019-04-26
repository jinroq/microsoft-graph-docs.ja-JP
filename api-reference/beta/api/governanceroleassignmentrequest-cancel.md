---
title: governanceRoleAssignmentRequest のキャンセル
description: governanceRoleAssignmentRequest を取り消します。
localization_priority: Normal
ms.openlocfilehash: d4573af27def33f11c4c20e11ce99a8b309581fb
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33329667"
---
# <a name="cancel-governanceroleassignmentrequest"></a><span data-ttu-id="13fc5-103">governanceRoleAssignmentRequest のキャンセル</span><span class="sxs-lookup"><span data-stu-id="13fc5-103">Cancel governanceRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="13fc5-104">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)を取り消します。</span><span class="sxs-lookup"><span data-stu-id="13fc5-104">Cancel a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="13fc5-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="13fc5-105">Permissions</span></span>
<span data-ttu-id="13fc5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="13fc5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13fc5-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="13fc5-108">Permission type</span></span>      | <span data-ttu-id="13fc5-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="13fc5-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="13fc5-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="13fc5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="13fc5-111">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="13fc5-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="13fc5-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="13fc5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="13fc5-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="13fc5-113">Not supported.</span></span>    |
|<span data-ttu-id="13fc5-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="13fc5-114">Application</span></span> | <span data-ttu-id="13fc5-115">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="13fc5-115">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="13fc5-116">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="13fc5-116">Optional query parameters</span></span>
<span data-ttu-id="13fc5-117">このメソッドは、 [OData クエリパラメーター](/graph/query-parameters)をサポートし**ていません**。</span><span class="sxs-lookup"><span data-stu-id="13fc5-117">This method does **not** support [OData Query Parameters](/graph/query-parameters).</span></span>

### <a name="http-request"></a><span data-ttu-id="13fc5-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="13fc5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/cancel
```

## <a name="request-headers"></a><span data-ttu-id="13fc5-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="13fc5-119">Request headers</span></span>
| <span data-ttu-id="13fc5-120">名前</span><span class="sxs-lookup"><span data-stu-id="13fc5-120">Name</span></span>       | <span data-ttu-id="13fc5-121">説明</span><span class="sxs-lookup"><span data-stu-id="13fc5-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="13fc5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="13fc5-122">Authorization</span></span>  | <span data-ttu-id="13fc5-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="13fc5-123">Bearer {code}</span></span>|
| <span data-ttu-id="13fc5-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="13fc5-124">Content-type</span></span>  | <span data-ttu-id="13fc5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="13fc5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="13fc5-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="13fc5-126">Request body</span></span>
<span data-ttu-id="13fc5-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="13fc5-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="13fc5-128">応答</span><span class="sxs-lookup"><span data-stu-id="13fc5-128">Response</span></span>
<span data-ttu-id="13fc5-p102">成功した場合、このメソッドは `204 NoContent` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="13fc5-p102">If successful, this method returns `204 NoContent` response code. It does not return anything in the response body.</span></span> 

## <a name="error-codes"></a><span data-ttu-id="13fc5-131">エラー コード</span><span class="sxs-lookup"><span data-stu-id="13fc5-131">Error codes</span></span>
<span data-ttu-id="13fc5-132">この API は、HTTP コードの標準に従います。</span><span class="sxs-lookup"><span data-stu-id="13fc5-132">This API follows the standard of HTTP codes.</span></span> <span data-ttu-id="13fc5-133">それに加えて、カスタムエラーコードは以下のとおりです。</span><span class="sxs-lookup"><span data-stu-id="13fc5-133">Besides, the custom error codes are shown below.</span></span>
|<span data-ttu-id="13fc5-134">エラー コード</span><span class="sxs-lookup"><span data-stu-id="13fc5-134">Error code</span></span>     | <span data-ttu-id="13fc5-135">エラー メッセージ</span><span class="sxs-lookup"><span data-stu-id="13fc5-135">Error message</span></span>              | <span data-ttu-id="13fc5-136">詳細</span><span class="sxs-lookup"><span data-stu-id="13fc5-136">Details</span></span> |
|:--------------------| :---------------------|:--------------------|
| <span data-ttu-id="13fc5-137">400 badrequest</span><span class="sxs-lookup"><span data-stu-id="13fc5-137">400 BadRequest</span></span> | <span data-ttu-id="13fc5-138">RoleAssignmentRequestNotFound</span><span class="sxs-lookup"><span data-stu-id="13fc5-138">RoleAssignmentRequestNotFound</span></span> | <span data-ttu-id="13fc5-139">governanceRoleAssignmentRequest は、システムに存在しません。</span><span class="sxs-lookup"><span data-stu-id="13fc5-139">The governanceRoleAssignmentRequest does not exist in system.</span></span>
| <span data-ttu-id="13fc5-140">400 badrequest</span><span class="sxs-lookup"><span data-stu-id="13fc5-140">400 BadRequest</span></span> | <span data-ttu-id="13fc5-141">RequestCannotBeCancelled</span><span class="sxs-lookup"><span data-stu-id="13fc5-141">RequestCannotBeCancelled</span></span>    | <span data-ttu-id="13fc5-142">、 `Granted` `PendingApproval`、、の状態の要求のみ`PendingAdminDecision`を取り消すことができます。 `PendingApprovalProvisioning`</span><span class="sxs-lookup"><span data-stu-id="13fc5-142">Only requests in status of `Granted`, `PendingApproval`, `PendingApprovalProvisioning` and `PendingAdminDecision` can be cancelled.</span></span>

## <a name="example"></a><span data-ttu-id="13fc5-143">例</span><span class="sxs-lookup"><span data-stu-id="13fc5-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="13fc5-144">要求</span><span class="sxs-lookup"><span data-stu-id="13fc5-144">Request</span></span>
<span data-ttu-id="13fc5-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="13fc5-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "cancel_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/cancel
```

##### <a name="response"></a><span data-ttu-id="13fc5-146">応答</span><span class="sxs-lookup"><span data-stu-id="13fc5-146">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Cancel governanceRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
