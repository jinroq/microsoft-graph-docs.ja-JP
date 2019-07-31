---
title: GovernanceRoleSetting の更新
description: GovernanceRoleSetting のプロパティを更新します。
localization_priority: Normal
doc_type: apiPageType
author: ''
ms.prod: ''
ms.openlocfilehash: 8dadb8669a3569b971586e04a9d84c5dff93da06
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35954150"
---
# <a name="update-governancerolesetting"></a><span data-ttu-id="307cd-103">GovernanceRoleSetting の更新</span><span class="sxs-lookup"><span data-stu-id="307cd-103">Update governanceRoleSetting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="307cd-104">[GovernanceRoleSetting](../resources/governancerolesetting.md)のプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="307cd-104">Update the properties of [governanceRoleSetting](../resources/governancerolesetting.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="307cd-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="307cd-105">Permissions</span></span>
<span data-ttu-id="307cd-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="307cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="307cd-108">**注:** また、この API では、リクエスターがリソースに`Active`対して少なくと`owner`も`user access administrator`1 つの管理者ロールの割り当て (または) を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="307cd-108">**Note:** This API also requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

|<span data-ttu-id="307cd-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="307cd-109">Permission type</span></span>      | <span data-ttu-id="307cd-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="307cd-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="307cd-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="307cd-111">Delegated (work or school account)</span></span> | <span data-ttu-id="307cd-112">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="307cd-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="307cd-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="307cd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="307cd-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="307cd-114">Not supported.</span></span>    |
|<span data-ttu-id="307cd-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="307cd-115">Application</span></span> | <span data-ttu-id="307cd-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="307cd-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="307cd-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="307cd-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /privilegedAccess/azureResources/roleSettings/{id}
```
## <a name="request-headers"></a><span data-ttu-id="307cd-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="307cd-118">Request headers</span></span>
| <span data-ttu-id="307cd-119">名前</span><span class="sxs-lookup"><span data-stu-id="307cd-119">Name</span></span>       | <span data-ttu-id="307cd-120">説明</span><span class="sxs-lookup"><span data-stu-id="307cd-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="307cd-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="307cd-121">Authorization</span></span>  | <span data-ttu-id="307cd-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="307cd-122">Bearer {code}</span></span>|
| <span data-ttu-id="307cd-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="307cd-123">Content-type</span></span>  | <span data-ttu-id="307cd-124">application/json</span><span class="sxs-lookup"><span data-stu-id="307cd-124">application/json</span></span>|


## <a name="request-body"></a><span data-ttu-id="307cd-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="307cd-125">Request body</span></span>
<span data-ttu-id="307cd-126">要求本文で、更新する必要がある[governanceRuleSettings](../resources/governancerulesetting.md)の値を指定します。</span><span class="sxs-lookup"><span data-stu-id="307cd-126">In the request body, supply the values for [governanceRuleSettings](../resources/governancerulesetting.md) that need to be updated.</span></span> 

| <span data-ttu-id="307cd-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="307cd-127">Property</span></span>     | <span data-ttu-id="307cd-128">型</span><span class="sxs-lookup"><span data-stu-id="307cd-128">Type</span></span>   |<span data-ttu-id="307cd-129">説明</span><span class="sxs-lookup"><span data-stu-id="307cd-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="307cd-130">adminEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="307cd-130">adminEligibleSettings</span></span>|<span data-ttu-id="307cd-131">[governanceRuleSetting](../resources/governancerulesetting.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="307cd-131">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="307cd-132">管理者が対象となる役割の割り当てを追加しようとしたときに評価されるルールの設定。</span><span class="sxs-lookup"><span data-stu-id="307cd-132">The rule settings that are evaluated when an administrator tries to add an eligible role assignment.</span></span>|
|<span data-ttu-id="307cd-133">adminMemberSettings</span><span class="sxs-lookup"><span data-stu-id="307cd-133">adminMemberSettings</span></span>|<span data-ttu-id="307cd-134">[governanceRuleSetting](../resources/governancerulesetting.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="307cd-134">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="307cd-135">管理者が直接メンバーの役割の割り当てを追加しようとしたときに評価されるルールの設定。</span><span class="sxs-lookup"><span data-stu-id="307cd-135">The rule settings that are evaluated when an administrator tries to add a direct member role assignment.</span></span>|
|<span data-ttu-id="307cd-136">userEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="307cd-136">userEligibleSettings</span></span>|<span data-ttu-id="307cd-137">[governanceRuleSetting](../resources/governancerulesetting.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="307cd-137">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="307cd-138">ユーザーが対象となる役割の割り当てを追加しようとしたときに評価されるルールの設定。</span><span class="sxs-lookup"><span data-stu-id="307cd-138">The rule settings that are evaluated when a user tries to add an eligible role assignment.</span></span> <span data-ttu-id="307cd-139">これは、現在の`pimforazurerbac`シナリオではサポートされておらず、今後のシナリオで利用できる場合があります。</span><span class="sxs-lookup"><span data-stu-id="307cd-139">This is not supported for `pimforazurerbac` scenario for now, and may be available in the future scenarios.</span></span>|
|<span data-ttu-id="307cd-140">userMemberSettings</span><span class="sxs-lookup"><span data-stu-id="307cd-140">userMemberSettings</span></span>|<span data-ttu-id="307cd-141">[governanceRuleSetting](../resources/governancerulesetting.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="307cd-141">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="307cd-142">ユーザーが役割の割り当てをアクティブ化しようとしたときに評価されるルールの設定。</span><span class="sxs-lookup"><span data-stu-id="307cd-142">The rule settings that are evaluated when a user tries to activate his role assignment.</span></span>|

## <a name="response"></a><span data-ttu-id="307cd-143">応答</span><span class="sxs-lookup"><span data-stu-id="307cd-143">Response</span></span>
<span data-ttu-id="307cd-p103">成功した場合、このメソッドは `204 NoContent` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="307cd-p103">If successful, this method returns a `204 NoContent` response code. It does not return anything in the response body.</span></span> 

### <a name="error-codes"></a><span data-ttu-id="307cd-146">エラー コード</span><span class="sxs-lookup"><span data-stu-id="307cd-146">Error codes</span></span>
<span data-ttu-id="307cd-147">この API は、標準の HTTP エラーコードを返します。</span><span class="sxs-lookup"><span data-stu-id="307cd-147">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="307cd-148">さらに、次のカスタムエラーコードが返されます。</span><span class="sxs-lookup"><span data-stu-id="307cd-148">In addition, it returns the following custom error codes.</span></span>

|<span data-ttu-id="307cd-149">エラー コード</span><span class="sxs-lookup"><span data-stu-id="307cd-149">Error code</span></span>     | <span data-ttu-id="307cd-150">エラー メッセージ</span><span class="sxs-lookup"><span data-stu-id="307cd-150">Error message</span></span>         | <span data-ttu-id="307cd-151">詳細</span><span class="sxs-lookup"><span data-stu-id="307cd-151">Details</span></span>             |
|:--------------| :---------------------|:--------------------|
| <span data-ttu-id="307cd-152">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="307cd-152">400 BadRequest</span></span>| <span data-ttu-id="307cd-153">RoleSettingNotFound</span><span class="sxs-lookup"><span data-stu-id="307cd-153">RoleSettingNotFound</span></span>   | <span data-ttu-id="307cd-154">[GovernanceRoleSetting](../resources/governancerolesetting.md)は、システムに存在しません。</span><span class="sxs-lookup"><span data-stu-id="307cd-154">The [governanceRoleSetting](../resources/governancerolesetting.md) does not exist in system.</span></span>
| <span data-ttu-id="307cd-155">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="307cd-155">400 BadRequest</span></span>| <span data-ttu-id="307cd-156">InvalidRoleSetting</span><span class="sxs-lookup"><span data-stu-id="307cd-156">InvalidRoleSetting</span></span>    | <span data-ttu-id="307cd-157">要求本文で指定された[governanceRuleSettings](../resources/governancerulesetting.md)値が無効です。</span><span class="sxs-lookup"><span data-stu-id="307cd-157">The [governanceRuleSettings](../resources/governancerulesetting.md) values provided in the request body are not valid.</span></span>

## <a name="example"></a><span data-ttu-id="307cd-158">例</span><span class="sxs-lookup"><span data-stu-id="307cd-158">Example</span></span> 
<span data-ttu-id="307cd-159">この例では、サブスクリプションの Wingtip Toys-製品のカスタムロール3のロール設定を更新します。</span><span class="sxs-lookup"><span data-stu-id="307cd-159">This example updates the role setting for Custom Role 3 in the subscription Wingtip Toys - Prod.</span></span>
##### <a name="request"></a><span data-ttu-id="307cd-160">要求</span><span class="sxs-lookup"><span data-stu-id="307cd-160">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="307cd-161">プロトコル</span><span class="sxs-lookup"><span data-stu-id="307cd-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_governancerolesetting"
}-->
```http
PATCH https://graph.microsoft.com/beta/privilegedAccess/pimforazurerbac/roleSettings/5fb5aef8-1081-4b8e-bb16-9d5d0385bab5
Content-type: application/json
Content-length: 350

{
   "adminEligibleSettings":[
      {
         "ruleIdentifier":"ExpirationRule",
         "setting":"{\"permanentAssignment\":false,\"maximumGrantPeriodInMinutes\":129600}"
      }
   ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="307cd-162">C#</span><span class="sxs-lookup"><span data-stu-id="307cd-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-governancerolesetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="307cd-163">Javascript</span><span class="sxs-lookup"><span data-stu-id="307cd-163">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-governancerolesetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="307cd-164">目的-C</span><span class="sxs-lookup"><span data-stu-id="307cd-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-governancerolesetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="307cd-165">Java</span><span class="sxs-lookup"><span data-stu-id="307cd-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-governancerolesetting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="307cd-166">応答</span><span class="sxs-lookup"><span data-stu-id="307cd-166">Response</span></span>
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
  ]
}
-->
