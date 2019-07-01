---
title: グループを取得する
description: グループ オブジェクトのプロパティとリレーションシップを取得します。
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: bb1078f5d2d15a2c58e39a98dd6794053f8ade76
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35273564"
---
# <a name="get-group"></a><span data-ttu-id="2a2c5-103">グループを取得する</span><span class="sxs-lookup"><span data-stu-id="2a2c5-103">Get group</span></span>

<span data-ttu-id="2a2c5-104">グループ オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="2a2c5-104">Get the properties and relationships of a group object.</span></span>

<span data-ttu-id="2a2c5-105">「[プロパティ](../resources/group.md#properties)」セクションに記載されているように、この操作は既定ですべての使用できるプロパティのサブセットのみを返します。</span><span class="sxs-lookup"><span data-stu-id="2a2c5-105">This operation returns by default only a subset of all the available properties, as noted in the [Properties](../resources/group.md#properties) section.</span></span> <span data-ttu-id="2a2c5-106">既定では_返されない_プロパティを取得するには、`$select` OData クエリ オプションでそれらを指定します。</span><span class="sxs-lookup"><span data-stu-id="2a2c5-106">To get properties that are _not_ returned by default, specify them in a `$select` OData query option.</span></span> <span data-ttu-id="2a2c5-107">**hasMembersWithLicenseErrors** プロパティは例外で、`$select` クエリでは返されません。</span><span class="sxs-lookup"><span data-stu-id="2a2c5-107">The **hasMembersWithLicenseErrors** property is an exception and is not returned in the `$select` query.</span></span>

## <a name="permissions"></a><span data-ttu-id="2a2c5-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2a2c5-108">Permissions</span></span>
<span data-ttu-id="2a2c5-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2a2c5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a2c5-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2a2c5-111">Permission type</span></span>      | <span data-ttu-id="2a2c5-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2a2c5-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2a2c5-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2a2c5-113">Delegated (work or school account)</span></span> | <span data-ttu-id="2a2c5-114">Group.Read.All、Directory.Read.All、Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2a2c5-114">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="2a2c5-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2a2c5-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2a2c5-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2a2c5-116">Not supported.</span></span>    |
|<span data-ttu-id="2a2c5-117">Application</span><span class="sxs-lookup"><span data-stu-id="2a2c5-117">Application</span></span> | <span data-ttu-id="2a2c5-118">Group.Read.All、Directory.Read.All、Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a2c5-118">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

><span data-ttu-id="2a2c5-119">**注:** アクセスするグループの機能によっては、アクセス許可が制限される場合があります。</span><span class="sxs-lookup"><span data-stu-id="2a2c5-119">**Note:** Depending on the group features you're trying to access, permissions might be limited.</span></span> <span data-ttu-id="2a2c5-120">詳細については、「[Microsoft Graph に関する既知の問題](/graph/known-issues)」の[グループ](/graph/known-issues#groups) セクションを参照してください。</span><span class="sxs-lookup"><span data-stu-id="2a2c5-120">For more information, see the [Groups](/graph/known-issues#groups) section in [Known issues with Microsoft Graph](/graph/known-issues).</span></span>

## <a name="http-request"></a><span data-ttu-id="2a2c5-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2a2c5-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2a2c5-122">省略可能なクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="2a2c5-122">Optional query parameters</span></span>
<span data-ttu-id="2a2c5-123">既定では返されないものも含め、特定のグループのプロパティを取得するには `$select` を使用できます。</span><span class="sxs-lookup"><span data-stu-id="2a2c5-123">You can use `$select` to get specific group properties, including those that are not returned by default.</span></span>

<span data-ttu-id="2a2c5-124">OData クエリ オプションの詳細については、「[OData クエリ パラメーター](/graph/query-parameters)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2a2c5-124">For more information on OData query options, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="2a2c5-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2a2c5-125">Request headers</span></span>
| <span data-ttu-id="2a2c5-126">名前</span><span class="sxs-lookup"><span data-stu-id="2a2c5-126">Name</span></span>       | <span data-ttu-id="2a2c5-127">型</span><span class="sxs-lookup"><span data-stu-id="2a2c5-127">Type</span></span> | <span data-ttu-id="2a2c5-128">説明</span><span class="sxs-lookup"><span data-stu-id="2a2c5-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2a2c5-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a2c5-129">Authorization</span></span>  | <span data-ttu-id="2a2c5-130">string</span><span class="sxs-lookup"><span data-stu-id="2a2c5-130">string</span></span>  | <span data-ttu-id="2a2c5-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2a2c5-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2a2c5-133">要求本文</span><span class="sxs-lookup"><span data-stu-id="2a2c5-133">Request body</span></span>
<span data-ttu-id="2a2c5-134">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2a2c5-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2a2c5-135">応答</span><span class="sxs-lookup"><span data-stu-id="2a2c5-135">Response</span></span>
<span data-ttu-id="2a2c5-136">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [group](../resources/group.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2a2c5-136">If successful, this method returns a `200 OK` response code and [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="2a2c5-137">`$select` を使用して特定のプロパティを指定していない限り、既定のプロパティを返します。</span><span class="sxs-lookup"><span data-stu-id="2a2c5-137">It returns the default properties unless you use `$select` to specify specific properties.</span></span>

## <a name="example"></a><span data-ttu-id="2a2c5-138">例</span><span class="sxs-lookup"><span data-stu-id="2a2c5-138">Example</span></span>

### <a name="example-1-return-all-default-properties"></a><span data-ttu-id="2a2c5-139">例 1: すべての既定のプロパティを返す</span><span class="sxs-lookup"><span data-stu-id="2a2c5-139">Example 1: Return all default properties</span></span>

<span data-ttu-id="2a2c5-140">すべての既定のプロパティを返します。</span><span class="sxs-lookup"><span data-stu-id="2a2c5-140">Return all default properties.</span></span>

#### <a name="request"></a><span data-ttu-id="2a2c5-141">要求</span><span class="sxs-lookup"><span data-stu-id="2a2c5-141">Request</span></span> 

<span data-ttu-id="2a2c5-142">GET 要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2a2c5-142">The following is an example of a GET request.</span></span> 
<!-- {
  "blockType": "request",
  "sampleKeys": ["b320ee12-b1cd-4cca-b648-a437be61c5cd"],
  "name": "get_group"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/b320ee12-b1cd-4cca-b648-a437be61c5cd
```

#### <a name="response"></a><span data-ttu-id="2a2c5-143">応答</span><span class="sxs-lookup"><span data-stu-id="2a2c5-143">Response</span></span>
<span data-ttu-id="2a2c5-144">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2a2c5-144">The following is an example of the response.</span></span> <span data-ttu-id="2a2c5-145">既定のプロパティのみが含まれています。</span><span class="sxs-lookup"><span data-stu-id="2a2c5-145">It includes only the default properties.</span></span>

><span data-ttu-id="2a2c5-146">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="2a2c5-146">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="2a2c5-147">実際の呼び出しでは、すべて既定のプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="2a2c5-147">All the default properties are returned in an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "get_group"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "b320ee12-b1cd-4cca-b648-a437be61c5cd",
    "deletedDateTime": null,
    "classification": null,
    "createdDateTime": "2018-12-22T00:51:37Z",
    "creationOptions": [],
    "description": "Self help community for library",
    "displayName": "Library Assist",
    "groupTypes": [
        "Unified"
    ],
    "mail": "library2@contoso.com",
    "mailEnabled": true,
    "mailNickname": "library",
    "onPremisesLastSyncDateTime": null,
    "onPremisesSecurityIdentifier": null,
    "onPremisesSyncEnabled": null,
    "preferredDataLocation": "CAN",
    "proxyAddresses": [
        "smtp:library7423@contoso.com",
        "SMTP:library2@contoso.com"
    ],
    "renewedDateTime": "2018-12-22T00:51:37Z",
    "resourceBehaviorOptions": [],
    "resourceProvisioningOptions": [],
    "securityEnabled": false,
    "visibility": "Public",
    "onPremisesProvisioningErrors": []
}
```

#### <a name="sdk-sample-code"></a><span data-ttu-id="2a2c5-148">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="2a2c5-148">SDK sample code</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="2a2c5-149">C#</span><span class="sxs-lookup"><span data-stu-id="2a2c5-149">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2a2c5-150">Javascript</span><span class="sxs-lookup"><span data-stu-id="2a2c5-150">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_group-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="2a2c5-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2a2c5-151">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_group-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="example-2-return-additional-properties-by-using-select"></a><span data-ttu-id="2a2c5-152">例 2: $select を使って追加のプロパティを返す</span><span class="sxs-lookup"><span data-stu-id="2a2c5-152">Example 2: Return additional properties by using $select</span></span>

<span data-ttu-id="2a2c5-153">`$select` を使って追加のプロパティを返します。</span><span class="sxs-lookup"><span data-stu-id="2a2c5-153">Return additional properties by using `$select`.</span></span>

#### <a name="request"></a><span data-ttu-id="2a2c5-154">要求</span><span class="sxs-lookup"><span data-stu-id="2a2c5-154">Request</span></span>

<span data-ttu-id="2a2c5-155">GET 要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2a2c5-155">The following is an example of a GET request.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["b320ee12-b1cd-4cca-b648-a437be61c5cd"],
  "name": "get_group_non_default"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/b320ee12-b1cd-4cca-b648-a437be61c5cd?$select=allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount
```

#### <a name="response"></a><span data-ttu-id="2a2c5-156">応答</span><span class="sxs-lookup"><span data-stu-id="2a2c5-156">Response</span></span>

<span data-ttu-id="2a2c5-157">要求された既定以外のプロパティを含む応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2a2c5-157">The following is an example of the response which includes the requested non-default properties.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "get_group_non_default"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups(allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount)/$entity",
    "id": "b320ee12-b1cd-4cca-b648-a437be61c5cd",
    "allowExternalSenders": false,
    "autoSubscribeNewMembers": false,
    "isSubscribedByMail": false,
    "unseenCount": 0
}
```

#### <a name="sdk-sample-code"></a><span data-ttu-id="2a2c5-158">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="2a2c5-158">SDK sample code</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="2a2c5-159">C#</span><span class="sxs-lookup"><span data-stu-id="2a2c5-159">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_group_non_default-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2a2c5-160">Javascript</span><span class="sxs-lookup"><span data-stu-id="2a2c5-160">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_group_non_default-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="2a2c5-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2a2c5-161">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_group_non_default-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/group-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/group-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
