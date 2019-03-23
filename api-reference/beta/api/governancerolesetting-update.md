---
title: governanceRoleSetting の更新
description: governanceRoleSetting のプロパティを更新します。
localization_priority: Normal
ms.openlocfilehash: f9c851f95df340693626ff82c960243eb2f85b54
ms.sourcegitcommit: 3615f9475d57bfbb3a8c4402af863897f592dfbd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/23/2019
ms.locfileid: "30789621"
---
# <a name="update-governancerolesetting"></a><span data-ttu-id="f6f6f-103">governanceRoleSetting の更新</span><span class="sxs-lookup"><span data-stu-id="f6f6f-103">Update governanceRoleSetting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6f6f-104">[governanceRoleSetting](../resources/governancerolesetting.md)のプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f6f6f-104">Update the properties of [governanceRoleSetting](../resources/governancerolesetting.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f6f6f-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f6f6f-105">Permissions</span></span>
<span data-ttu-id="f6f6f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f6f6f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="f6f6f-108">**注:** また、この API では、リクエスターがリソースに`Active`対して少なくと`owner`も`user access administrator`1 つの管理者ロールの割り当て (または) を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f6f6f-108">**Note:** This API also requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

|<span data-ttu-id="f6f6f-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f6f6f-109">Permission type</span></span>      | <span data-ttu-id="f6f6f-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f6f6f-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f6f6f-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f6f6f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f6f6f-112">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="f6f6f-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="f6f6f-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f6f6f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f6f6f-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f6f6f-114">Not supported.</span></span>    |
|<span data-ttu-id="f6f6f-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f6f6f-115">Application</span></span> | <span data-ttu-id="f6f6f-116">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="f6f6f-116">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="f6f6f-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f6f6f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /privilegedAccess/azureResources/roleSettings/{id}
```
## <a name="request-headers"></a><span data-ttu-id="f6f6f-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f6f6f-118">Request headers</span></span>
| <span data-ttu-id="f6f6f-119">名前</span><span class="sxs-lookup"><span data-stu-id="f6f6f-119">Name</span></span>       | <span data-ttu-id="f6f6f-120">説明</span><span class="sxs-lookup"><span data-stu-id="f6f6f-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="f6f6f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6f6f-121">Authorization</span></span>  | <span data-ttu-id="f6f6f-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="f6f6f-122">Bearer {code}</span></span>|
| <span data-ttu-id="f6f6f-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="f6f6f-123">Content-type</span></span>  | <span data-ttu-id="f6f6f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f6f6f-124">application/json</span></span>|


## <a name="request-body"></a><span data-ttu-id="f6f6f-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="f6f6f-125">Request body</span></span>
<span data-ttu-id="f6f6f-126">要求本文で、更新する必要がある[governanceRuleSettings](../resources/governancerulesetting.md)の値を指定します。</span><span class="sxs-lookup"><span data-stu-id="f6f6f-126">In the request body, supply the values for [governanceRuleSettings](../resources/governancerulesetting.md) that need to be updated.</span></span> 

| <span data-ttu-id="f6f6f-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f6f6f-127">Property</span></span>     | <span data-ttu-id="f6f6f-128">型</span><span class="sxs-lookup"><span data-stu-id="f6f6f-128">Type</span></span>   |<span data-ttu-id="f6f6f-129">説明</span><span class="sxs-lookup"><span data-stu-id="f6f6f-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f6f6f-130">adminEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="f6f6f-130">adminEligibleSettings</span></span>|<span data-ttu-id="f6f6f-131">[governanceRuleSetting](../resources/governancerulesetting.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f6f6f-131">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="f6f6f-132">管理者が対象となる役割の割り当てを追加しようとしたときに評価されるルールの設定。</span><span class="sxs-lookup"><span data-stu-id="f6f6f-132">The rule settings that are evaluated when an administrator tries to add an eligible role assignment.</span></span>|
|<span data-ttu-id="f6f6f-133">adminmembersettings</span><span class="sxs-lookup"><span data-stu-id="f6f6f-133">adminMemberSettings</span></span>|<span data-ttu-id="f6f6f-134">[governanceRuleSetting](../resources/governancerulesetting.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f6f6f-134">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="f6f6f-135">管理者が直接メンバーの役割の割り当てを追加しようとしたときに評価されるルールの設定。</span><span class="sxs-lookup"><span data-stu-id="f6f6f-135">The rule settings that are evaluated when an administrator tries to add a direct member role assignment.</span></span>|
|<span data-ttu-id="f6f6f-136">userEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="f6f6f-136">userEligibleSettings</span></span>|<span data-ttu-id="f6f6f-137">[governanceRuleSetting](../resources/governancerulesetting.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f6f6f-137">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="f6f6f-138">ユーザーが対象となる役割の割り当てを追加しようとしたときに評価されるルールの設定。</span><span class="sxs-lookup"><span data-stu-id="f6f6f-138">The rule settings that are evaluated when a user tries to add an eligible role assignment.</span></span> <span data-ttu-id="f6f6f-139">これは、現在の`pimforazurerbac`シナリオではサポートされておらず、今後のシナリオで利用できる場合があります。</span><span class="sxs-lookup"><span data-stu-id="f6f6f-139">This is not supported for `pimforazurerbac` scenario for now, and may be available in the future scenarios.</span></span>|
|<span data-ttu-id="f6f6f-140">usermembersettings</span><span class="sxs-lookup"><span data-stu-id="f6f6f-140">userMemberSettings</span></span>|<span data-ttu-id="f6f6f-141">[governanceRuleSetting](../resources/governancerulesetting.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f6f6f-141">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="f6f6f-142">ユーザーが役割の割り当てをアクティブ化しようとしたときに評価されるルールの設定。</span><span class="sxs-lookup"><span data-stu-id="f6f6f-142">The rule settings that are evaluated when a user tries to activate his role assignment.</span></span>|

## <a name="response"></a><span data-ttu-id="f6f6f-143">応答</span><span class="sxs-lookup"><span data-stu-id="f6f6f-143">Response</span></span>
<span data-ttu-id="f6f6f-p103">成功した場合、このメソッドは `204 NoContent` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="f6f6f-p103">If successful, this method returns a `204 NoContent` response code. It does not return anything in the response body.</span></span> 

### <a name="error-codes"></a><span data-ttu-id="f6f6f-146">エラー コード</span><span class="sxs-lookup"><span data-stu-id="f6f6f-146">Error codes</span></span>
<span data-ttu-id="f6f6f-147">この API は、標準の HTTP エラーコードを返します。</span><span class="sxs-lookup"><span data-stu-id="f6f6f-147">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="f6f6f-148">さらに、次のカスタムエラーコードが返されます。</span><span class="sxs-lookup"><span data-stu-id="f6f6f-148">In addition, it returns the following custom error codes.</span></span>

|<span data-ttu-id="f6f6f-149">エラー コード</span><span class="sxs-lookup"><span data-stu-id="f6f6f-149">Error code</span></span>     | <span data-ttu-id="f6f6f-150">エラー メッセージ</span><span class="sxs-lookup"><span data-stu-id="f6f6f-150">Error message</span></span>         | <span data-ttu-id="f6f6f-151">詳細</span><span class="sxs-lookup"><span data-stu-id="f6f6f-151">Details</span></span>             |
|:--------------| :---------------------|:--------------------|
| <span data-ttu-id="f6f6f-152">400 badrequest</span><span class="sxs-lookup"><span data-stu-id="f6f6f-152">400 BadRequest</span></span>| <span data-ttu-id="f6f6f-153">RoleSettingNotFound</span><span class="sxs-lookup"><span data-stu-id="f6f6f-153">RoleSettingNotFound</span></span>   | <span data-ttu-id="f6f6f-154">[governanceRoleSetting](../resources/governancerolesetting.md)は、システムに存在しません。</span><span class="sxs-lookup"><span data-stu-id="f6f6f-154">The [governanceRoleSetting](../resources/governancerolesetting.md) does not exist in system.</span></span>
| <span data-ttu-id="f6f6f-155">400 badrequest</span><span class="sxs-lookup"><span data-stu-id="f6f6f-155">400 BadRequest</span></span>| <span data-ttu-id="f6f6f-156">invalidrolesetting</span><span class="sxs-lookup"><span data-stu-id="f6f6f-156">InvalidRoleSetting</span></span>    | <span data-ttu-id="f6f6f-157">要求本文で指定された[governanceRuleSettings](../resources/governancerulesetting.md)値が無効です。</span><span class="sxs-lookup"><span data-stu-id="f6f6f-157">The [governanceRuleSettings](../resources/governancerulesetting.md) values provided in the request body are not valid.</span></span>

## <a name="example"></a><span data-ttu-id="f6f6f-158">例</span><span class="sxs-lookup"><span data-stu-id="f6f6f-158">Example</span></span> 
<span data-ttu-id="f6f6f-159">この例では、サブスクリプションの Wingtip Toys-製品のカスタムロール3のロール設定を更新します。</span><span class="sxs-lookup"><span data-stu-id="f6f6f-159">This example updates the role setting for Custom Role 3 in the subscription Wingtip Toys - Prod.</span></span>
##### <a name="request"></a><span data-ttu-id="f6f6f-160">要求</span><span class="sxs-lookup"><span data-stu-id="f6f6f-160">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="f6f6f-161">応答</span><span class="sxs-lookup"><span data-stu-id="f6f6f-161">Response</span></span>
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
