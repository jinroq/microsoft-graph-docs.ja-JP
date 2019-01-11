---
title: GovernanceRoleSetting を更新します。
description: GovernanceRoleSetting のプロパティを更新します。
localization_priority: Normal
ms.openlocfilehash: e76d7955576d9d514a70b52b31f4d034362aac1f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874908"
---
# <a name="update-governancerolesetting"></a><span data-ttu-id="d6657-103">GovernanceRoleSetting を更新します。</span><span class="sxs-lookup"><span data-stu-id="d6657-103">Update governanceRoleSetting</span></span>

> <span data-ttu-id="d6657-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d6657-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d6657-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d6657-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d6657-106">[GovernanceRoleSetting](../resources/governancerolesetting.md)のプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d6657-106">Update the properties of [governanceRoleSetting](../resources/governancerolesetting.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d6657-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d6657-107">Permissions</span></span>
<span data-ttu-id="d6657-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d6657-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="d6657-110">**注:** この API では、依頼者の少なくとも 1 つある必要があります`Active`管理者の役割の割り当て (`owner`または`user access administrator`)、リソースにします。</span><span class="sxs-lookup"><span data-stu-id="d6657-110">**Note:** This API also requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

|<span data-ttu-id="d6657-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d6657-111">Permission type</span></span>      | <span data-ttu-id="d6657-112">Permissions</span><span class="sxs-lookup"><span data-stu-id="d6657-112">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d6657-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d6657-113">Delegated (work or school account)</span></span> | <span data-ttu-id="d6657-114">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="d6657-114">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="d6657-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d6657-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d6657-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d6657-116">Not supported.</span></span>    |
|<span data-ttu-id="d6657-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d6657-117">Application</span></span> | <span data-ttu-id="d6657-118">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="d6657-118">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="d6657-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d6657-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /privilegedAccess/azureResources/roleSettings/{id}
```
## <a name="request-headers"></a><span data-ttu-id="d6657-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d6657-120">Request headers</span></span>
| <span data-ttu-id="d6657-121">名前</span><span class="sxs-lookup"><span data-stu-id="d6657-121">Name</span></span>       | <span data-ttu-id="d6657-122">説明</span><span class="sxs-lookup"><span data-stu-id="d6657-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="d6657-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6657-123">Authorization</span></span>  | <span data-ttu-id="d6657-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="d6657-124">Bearer {code}</span></span>|
| <span data-ttu-id="d6657-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="d6657-125">Content-type</span></span>  | <span data-ttu-id="d6657-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d6657-126">application/json</span></span>|


## <a name="request-body"></a><span data-ttu-id="d6657-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="d6657-127">Request body</span></span>
<span data-ttu-id="d6657-128">要求の本体を更新する必要がある[governanceRuleSettings](../resources/governancerulesetting.md)の値を指定します。</span><span class="sxs-lookup"><span data-stu-id="d6657-128">In the request body, supply the values for [governanceRuleSettings](../resources/governancerulesetting.md) that need to be updated.</span></span> 

| <span data-ttu-id="d6657-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d6657-129">Property</span></span>     | <span data-ttu-id="d6657-130">種類</span><span class="sxs-lookup"><span data-stu-id="d6657-130">Type</span></span>   |<span data-ttu-id="d6657-131">説明</span><span class="sxs-lookup"><span data-stu-id="d6657-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d6657-132">adminEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="d6657-132">adminEligibleSettings</span></span>|[<span data-ttu-id="d6657-133">governanceRuleSetting</span><span class="sxs-lookup"><span data-stu-id="d6657-133">governanceRuleSetting</span></span>](../resources/governancerulesetting.md)|<span data-ttu-id="d6657-134">管理者対象のロール割り当てを追加しようとするときに評価されるルールの設定。</span><span class="sxs-lookup"><span data-stu-id="d6657-134">The rule settings that are evaluated when an administrator tries to add an eligible role assignment.</span></span>|
|<span data-ttu-id="d6657-135">adminMemberSettings</span><span class="sxs-lookup"><span data-stu-id="d6657-135">adminMemberSettings</span></span>|[<span data-ttu-id="d6657-136">governanceRuleSetting</span><span class="sxs-lookup"><span data-stu-id="d6657-136">governanceRuleSetting</span></span>](../resources/governancerulesetting.md)|<span data-ttu-id="d6657-137">直接的なメンバーの役割の割り当てを追加する際に管理者に評価されるルールの設定。</span><span class="sxs-lookup"><span data-stu-id="d6657-137">The rule settings that are evaluated when an administrator tries to add a direct member role assignment.</span></span>|
|<span data-ttu-id="d6657-138">userEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="d6657-138">userEligibleSettings</span></span>|[<span data-ttu-id="d6657-139">governanceRuleSetting</span><span class="sxs-lookup"><span data-stu-id="d6657-139">governanceRuleSetting</span></span>](../resources/governancerulesetting.md)|<span data-ttu-id="d6657-140">ユーザーが対象のロール割り当てを追加するときに評価されるルールの設定。</span><span class="sxs-lookup"><span data-stu-id="d6657-140">The rule settings that are evaluated when a user tries to add an eligible role assignment.</span></span> <span data-ttu-id="d6657-141">サポートされていない`pimforazurerbac`ここでは、シナリオと、将来のシナリオで使用可能な場合があります。</span><span class="sxs-lookup"><span data-stu-id="d6657-141">This is not supported for `pimforazurerbac` scenario for now, and may be available in the future scenarios.</span></span>|
|<span data-ttu-id="d6657-142">userMemberSettings</span><span class="sxs-lookup"><span data-stu-id="d6657-142">userMemberSettings</span></span>|[<span data-ttu-id="d6657-143">governanceRuleSetting</span><span class="sxs-lookup"><span data-stu-id="d6657-143">governanceRuleSetting</span></span>](../resources/governancerulesetting.md)|<span data-ttu-id="d6657-144">ユーザーが彼の役割の割り当てを有効にしようとした場合に評価されるルールの設定。</span><span class="sxs-lookup"><span data-stu-id="d6657-144">The rule settings that are evaluated when a user tries to activate his role assignment.</span></span>|

## <a name="response"></a><span data-ttu-id="d6657-145">応答</span><span class="sxs-lookup"><span data-stu-id="d6657-145">Response</span></span>
<span data-ttu-id="d6657-p104">成功した場合、このメソッドは `204 NoContent` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="d6657-p104">If successful, this method returns a `204 NoContent` response code. It does not return anything in the response body.</span></span> 

### <a name="error-codes"></a><span data-ttu-id="d6657-148">エラー コード</span><span class="sxs-lookup"><span data-stu-id="d6657-148">Error codes</span></span>
<span data-ttu-id="d6657-149">この API では、標準の HTTP エラー コードを返します。</span><span class="sxs-lookup"><span data-stu-id="d6657-149">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="d6657-150">さらに、次のカスタム エラー コードを返します。</span><span class="sxs-lookup"><span data-stu-id="d6657-150">In addition, it returns the following custom error codes.</span></span>

|<span data-ttu-id="d6657-151">エラー コード</span><span class="sxs-lookup"><span data-stu-id="d6657-151">Error code</span></span>     | <span data-ttu-id="d6657-152">エラー メッセージ</span><span class="sxs-lookup"><span data-stu-id="d6657-152">Error message</span></span>         | <span data-ttu-id="d6657-153">詳細</span><span class="sxs-lookup"><span data-stu-id="d6657-153">Details</span></span>             |
|:--------------| :---------------------|:--------------------|
| <span data-ttu-id="d6657-154">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="d6657-154">400 BadRequest</span></span>| <span data-ttu-id="d6657-155">RoleSettingNotFound</span><span class="sxs-lookup"><span data-stu-id="d6657-155">RoleSettingNotFound</span></span>   | <span data-ttu-id="d6657-156">[GovernanceRoleSetting](../resources/governancerolesetting.md)は、システムに存在しません。</span><span class="sxs-lookup"><span data-stu-id="d6657-156">The [governanceRoleSetting](../resources/governancerolesetting.md) does not exist in system.</span></span>
| <span data-ttu-id="d6657-157">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="d6657-157">400 BadRequest</span></span>| <span data-ttu-id="d6657-158">InvalidRoleSetting</span><span class="sxs-lookup"><span data-stu-id="d6657-158">InvalidRoleSetting</span></span>    | <span data-ttu-id="d6657-159">要求の本文に記載されている[governanceRuleSettings](../resources/governancerulesetting.md)の値が有効ではありません。</span><span class="sxs-lookup"><span data-stu-id="d6657-159">The [governanceRuleSettings](../resources/governancerulesetting.md) values provided in the request body are not valid.</span></span>

## <a name="example"></a><span data-ttu-id="d6657-160">例</span><span class="sxs-lookup"><span data-stu-id="d6657-160">Example</span></span> 
<span data-ttu-id="d6657-161">この例では、サブスクリプション Wingtip toys 社の商品にカスタム ロール 3 のロール設定を更新します。</span><span class="sxs-lookup"><span data-stu-id="d6657-161">This example updates the role setting for Custom Role 3 in the subscription Wingtip Toys - Prod.</span></span>
##### <a name="request"></a><span data-ttu-id="d6657-162">要求</span><span class="sxs-lookup"><span data-stu-id="d6657-162">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="d6657-163">応答</span><span class="sxs-lookup"><span data-stu-id="d6657-163">Response</span></span>
<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update governanceRoleSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
