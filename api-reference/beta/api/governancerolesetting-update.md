---
title: GovernanceRoleSetting を更新します。
description: GovernanceRoleSetting のプロパティを更新します。
localization_priority: Normal
ms.openlocfilehash: e5fc297690816227e1031af363ea7d4d38199e25
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509330"
---
# <a name="update-governancerolesetting"></a><span data-ttu-id="bb29e-103">GovernanceRoleSetting を更新します。</span><span class="sxs-lookup"><span data-stu-id="bb29e-103">Update governanceRoleSetting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb29e-104">[GovernanceRoleSetting](../resources/governancerolesetting.md)のプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="bb29e-104">Update the properties of [governanceRoleSetting](../resources/governancerolesetting.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bb29e-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="bb29e-105">Permissions</span></span>
<span data-ttu-id="bb29e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bb29e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="bb29e-108">**注:** この API では、依頼者の少なくとも 1 つある必要があります`Active`管理者の役割の割り当て (`owner`または`user access administrator`)、リソースにします。</span><span class="sxs-lookup"><span data-stu-id="bb29e-108">**Note:** This API also requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

|<span data-ttu-id="bb29e-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bb29e-109">Permission type</span></span>      | <span data-ttu-id="bb29e-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="bb29e-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bb29e-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bb29e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bb29e-112">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="bb29e-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="bb29e-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bb29e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb29e-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bb29e-114">Not supported.</span></span>    |
|<span data-ttu-id="bb29e-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bb29e-115">Application</span></span> | <span data-ttu-id="bb29e-116">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="bb29e-116">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="bb29e-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bb29e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /privilegedAccess/azureResources/roleSettings/{id}
```
## <a name="request-headers"></a><span data-ttu-id="bb29e-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bb29e-118">Request headers</span></span>
| <span data-ttu-id="bb29e-119">名前</span><span class="sxs-lookup"><span data-stu-id="bb29e-119">Name</span></span>       | <span data-ttu-id="bb29e-120">説明</span><span class="sxs-lookup"><span data-stu-id="bb29e-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="bb29e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb29e-121">Authorization</span></span>  | <span data-ttu-id="bb29e-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="bb29e-122">Bearer {code}</span></span>|
| <span data-ttu-id="bb29e-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="bb29e-123">Content-type</span></span>  | <span data-ttu-id="bb29e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="bb29e-124">application/json</span></span>|


## <a name="request-body"></a><span data-ttu-id="bb29e-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="bb29e-125">Request body</span></span>
<span data-ttu-id="bb29e-126">要求の本体を更新する必要がある[governanceRuleSettings](../resources/governancerulesetting.md)の値を指定します。</span><span class="sxs-lookup"><span data-stu-id="bb29e-126">In the request body, supply the values for [governanceRuleSettings](../resources/governancerulesetting.md) that need to be updated.</span></span> 

| <span data-ttu-id="bb29e-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bb29e-127">Property</span></span>     | <span data-ttu-id="bb29e-128">型</span><span class="sxs-lookup"><span data-stu-id="bb29e-128">Type</span></span>   |<span data-ttu-id="bb29e-129">説明</span><span class="sxs-lookup"><span data-stu-id="bb29e-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bb29e-130">adminEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="bb29e-130">adminEligibleSettings</span></span>|[<span data-ttu-id="bb29e-131">governanceRuleSetting</span><span class="sxs-lookup"><span data-stu-id="bb29e-131">governanceRuleSetting</span></span>](../resources/governancerulesetting.md)|<span data-ttu-id="bb29e-132">管理者対象のロール割り当てを追加しようとするときに評価されるルールの設定。</span><span class="sxs-lookup"><span data-stu-id="bb29e-132">The rule settings that are evaluated when an administrator tries to add an eligible role assignment.</span></span>|
|<span data-ttu-id="bb29e-133">adminMemberSettings</span><span class="sxs-lookup"><span data-stu-id="bb29e-133">adminMemberSettings</span></span>|[<span data-ttu-id="bb29e-134">governanceRuleSetting</span><span class="sxs-lookup"><span data-stu-id="bb29e-134">governanceRuleSetting</span></span>](../resources/governancerulesetting.md)|<span data-ttu-id="bb29e-135">直接的なメンバーの役割の割り当てを追加する際に管理者に評価されるルールの設定。</span><span class="sxs-lookup"><span data-stu-id="bb29e-135">The rule settings that are evaluated when an administrator tries to add a direct member role assignment.</span></span>|
|<span data-ttu-id="bb29e-136">userEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="bb29e-136">userEligibleSettings</span></span>|[<span data-ttu-id="bb29e-137">governanceRuleSetting</span><span class="sxs-lookup"><span data-stu-id="bb29e-137">governanceRuleSetting</span></span>](../resources/governancerulesetting.md)|<span data-ttu-id="bb29e-138">ユーザーが対象のロール割り当てを追加するときに評価されるルールの設定。</span><span class="sxs-lookup"><span data-stu-id="bb29e-138">The rule settings that are evaluated when a user tries to add an eligible role assignment.</span></span> <span data-ttu-id="bb29e-139">サポートされていない`pimforazurerbac`ここでは、シナリオと、将来のシナリオで使用可能な場合があります。</span><span class="sxs-lookup"><span data-stu-id="bb29e-139">This is not supported for `pimforazurerbac` scenario for now, and may be available in the future scenarios.</span></span>|
|<span data-ttu-id="bb29e-140">userMemberSettings</span><span class="sxs-lookup"><span data-stu-id="bb29e-140">userMemberSettings</span></span>|[<span data-ttu-id="bb29e-141">governanceRuleSetting</span><span class="sxs-lookup"><span data-stu-id="bb29e-141">governanceRuleSetting</span></span>](../resources/governancerulesetting.md)|<span data-ttu-id="bb29e-142">ユーザーが彼の役割の割り当てを有効にしようとした場合に評価されるルールの設定。</span><span class="sxs-lookup"><span data-stu-id="bb29e-142">The rule settings that are evaluated when a user tries to activate his role assignment.</span></span>|

## <a name="response"></a><span data-ttu-id="bb29e-143">応答</span><span class="sxs-lookup"><span data-stu-id="bb29e-143">Response</span></span>
<span data-ttu-id="bb29e-p103">成功した場合、このメソッドは `204 NoContent` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="bb29e-p103">If successful, this method returns a `204 NoContent` response code. It does not return anything in the response body.</span></span> 

### <a name="error-codes"></a><span data-ttu-id="bb29e-146">エラー コード</span><span class="sxs-lookup"><span data-stu-id="bb29e-146">Error codes</span></span>
<span data-ttu-id="bb29e-147">この API では、標準の HTTP エラー コードを返します。</span><span class="sxs-lookup"><span data-stu-id="bb29e-147">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="bb29e-148">さらに、次のカスタム エラー コードを返します。</span><span class="sxs-lookup"><span data-stu-id="bb29e-148">In addition, it returns the following custom error codes.</span></span>

|<span data-ttu-id="bb29e-149">エラー コード</span><span class="sxs-lookup"><span data-stu-id="bb29e-149">Error code</span></span>     | <span data-ttu-id="bb29e-150">エラー メッセージ</span><span class="sxs-lookup"><span data-stu-id="bb29e-150">Error message</span></span>         | <span data-ttu-id="bb29e-151">詳細</span><span class="sxs-lookup"><span data-stu-id="bb29e-151">Details</span></span>             |
|:--------------| :---------------------|:--------------------|
| <span data-ttu-id="bb29e-152">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="bb29e-152">400 BadRequest</span></span>| <span data-ttu-id="bb29e-153">RoleSettingNotFound</span><span class="sxs-lookup"><span data-stu-id="bb29e-153">RoleSettingNotFound</span></span>   | <span data-ttu-id="bb29e-154">[GovernanceRoleSetting](../resources/governancerolesetting.md)は、システムに存在しません。</span><span class="sxs-lookup"><span data-stu-id="bb29e-154">The [governanceRoleSetting](../resources/governancerolesetting.md) does not exist in system.</span></span>
| <span data-ttu-id="bb29e-155">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="bb29e-155">400 BadRequest</span></span>| <span data-ttu-id="bb29e-156">InvalidRoleSetting</span><span class="sxs-lookup"><span data-stu-id="bb29e-156">InvalidRoleSetting</span></span>    | <span data-ttu-id="bb29e-157">要求の本文に記載されている[governanceRuleSettings](../resources/governancerulesetting.md)の値が有効ではありません。</span><span class="sxs-lookup"><span data-stu-id="bb29e-157">The [governanceRuleSettings](../resources/governancerulesetting.md) values provided in the request body are not valid.</span></span>

## <a name="example"></a><span data-ttu-id="bb29e-158">例</span><span class="sxs-lookup"><span data-stu-id="bb29e-158">Example</span></span> 
<span data-ttu-id="bb29e-159">この例では、サブスクリプション Wingtip toys 社の商品にカスタム ロール 3 のロール設定を更新します。</span><span class="sxs-lookup"><span data-stu-id="bb29e-159">This example updates the role setting for Custom Role 3 in the subscription Wingtip Toys - Prod.</span></span>
##### <a name="request"></a><span data-ttu-id="bb29e-160">要求</span><span class="sxs-lookup"><span data-stu-id="bb29e-160">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_governancerolesetting"
}-->
```http
PATCH https://graph.microsoft.com/beta/privilegedAccess/pimforazurerbac/roleSettings/5fb5aef8-1081-4b8e-bb16-9d5d0385bab5
Content-type: application/json
Content-length: 350

{
  "adminEligibleSettings":[{"ruleIdentifier":"ExpirationRule","setting":"{\"permanentAssignment\":false,\"maximumGrantPeriodInMinutes\":129600}"}]
}
```
##### <a name="response"></a><span data-ttu-id="bb29e-161">応答</span><span class="sxs-lookup"><span data-stu-id="bb29e-161">Response</span></span>
<!-- {
  "blockType": "response",
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
  "description": "Update governanceRoleSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/governancerolesetting-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
