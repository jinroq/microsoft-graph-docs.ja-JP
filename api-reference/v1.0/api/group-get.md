---
title: グループを取得する
description: グループ オブジェクトのプロパティとリレーションシップを取得します。
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: 27cb6a9c189d158e9e34e26973fc6b2713f718c9
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33615034"
---
# <a name="get-group"></a><span data-ttu-id="e7be2-103">グループを取得する</span><span class="sxs-lookup"><span data-stu-id="e7be2-103">Get group</span></span>
<span data-ttu-id="e7be2-104">グループ オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="e7be2-104">Get the properties and relationships of a group object.</span></span>

<span data-ttu-id="e7be2-105">「[プロパティ](../resources/group.md#properties)」セクションに記載されているように、この操作は既定ですべての使用できるプロパティのサブセットのみを返します。</span><span class="sxs-lookup"><span data-stu-id="e7be2-105">This operation returns by default only a subset of all the available properties, as noted in the [Properties](../resources/group.md#properties) section.</span></span> <span data-ttu-id="e7be2-106">既定では_返されない_プロパティを取得するには、`$select` OData クエリ オプションでそれらを指定します。</span><span class="sxs-lookup"><span data-stu-id="e7be2-106">To get properties that are _not_ returned by default, specify them in a `$select` OData query option.</span></span> <span data-ttu-id="e7be2-107">`$select` の[例](#request-2)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e7be2-107">See an [example](#request-2) of  `$select`.</span></span> <span data-ttu-id="e7be2-108">例外は **hasMembersWithLicenseErrors** プロパティです。</span><span class="sxs-lookup"><span data-stu-id="e7be2-108">An exception is the **hasMembersWithLicenseErrors** property.</span></span> <span data-ttu-id="e7be2-109">このプロパティの使用方法の[例](group-list.md#request-2)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e7be2-109">See an [example](group-list.md#request-2) of how to use this property.</span></span>

## <a name="permissions"></a><span data-ttu-id="e7be2-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e7be2-110">Permissions</span></span>
<span data-ttu-id="e7be2-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e7be2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7be2-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e7be2-113">Permission type</span></span>      | <span data-ttu-id="e7be2-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e7be2-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e7be2-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e7be2-115">Delegated (work or school account)</span></span> | <span data-ttu-id="e7be2-116">Group.Read.All、Group.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7be2-116">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="e7be2-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e7be2-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e7be2-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e7be2-118">Not supported.</span></span>    |
|<span data-ttu-id="e7be2-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e7be2-119">Application</span></span> | <span data-ttu-id="e7be2-120">Group.Read.All、Group.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7be2-120">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e7be2-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e7be2-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e7be2-122">省略可能なクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e7be2-122">Optional query parameters</span></span>
<span data-ttu-id="e7be2-123">既定では返されないものも含め、特定のグループのプロパティを取得するには `$select` を使用できます。</span><span class="sxs-lookup"><span data-stu-id="e7be2-123">You can use `$select` to get specific group properties, including those that are not returned by default.</span></span> <span data-ttu-id="e7be2-124">次の[例](#request-2)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e7be2-124">See an [example](#request-2) below.</span></span>

<span data-ttu-id="e7be2-125">OData クエリ オプションの詳細については、「[OData クエリ パラメーター](/graph/query-parameters)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e7be2-125">For more information on OData query options, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e7be2-126">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e7be2-126">Request headers</span></span>
| <span data-ttu-id="e7be2-127">名前</span><span class="sxs-lookup"><span data-stu-id="e7be2-127">Name</span></span>       | <span data-ttu-id="e7be2-128">型</span><span class="sxs-lookup"><span data-stu-id="e7be2-128">Type</span></span> | <span data-ttu-id="e7be2-129">説明</span><span class="sxs-lookup"><span data-stu-id="e7be2-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e7be2-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7be2-130">Authorization</span></span>  | <span data-ttu-id="e7be2-131">string</span><span class="sxs-lookup"><span data-stu-id="e7be2-131">string</span></span>  | <span data-ttu-id="e7be2-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e7be2-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e7be2-134">要求本文</span><span class="sxs-lookup"><span data-stu-id="e7be2-134">Request body</span></span>
<span data-ttu-id="e7be2-135">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e7be2-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e7be2-136">応答</span><span class="sxs-lookup"><span data-stu-id="e7be2-136">Response</span></span>
<span data-ttu-id="e7be2-137">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [group](../resources/group.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e7be2-137">If successful, this method returns a `200 OK` response code and [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="e7be2-138">`$select` を使用して特定のプロパティを指定していない限り、既定のプロパティを返します。</span><span class="sxs-lookup"><span data-stu-id="e7be2-138">It returns the default properties unless you use `$select` to specify specific properties.</span></span>

## <a name="example"></a><span data-ttu-id="e7be2-139">例</span><span class="sxs-lookup"><span data-stu-id="e7be2-139">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="e7be2-140">要求 1</span><span class="sxs-lookup"><span data-stu-id="e7be2-140">Request 1</span></span>
<span data-ttu-id="e7be2-141">GET 要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e7be2-141">The following is an example of a GET request.</span></span> 
<!-- {
  "blockType": "request",
  "sampleKeys": ["b320ee12-b1cd-4cca-b648-a437be61c5cd"],
  "name": "get_group"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/b320ee12-b1cd-4cca-b648-a437be61c5cd
```

#### <a name="response-1"></a><span data-ttu-id="e7be2-142">応答 1</span><span class="sxs-lookup"><span data-stu-id="e7be2-142">Response 1</span></span>
<span data-ttu-id="e7be2-143">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e7be2-143">The following is an example of the response.</span></span> <span data-ttu-id="e7be2-144">既定のプロパティのみが含まれています。</span><span class="sxs-lookup"><span data-stu-id="e7be2-144">It includes only the default properties.</span></span>

><span data-ttu-id="e7be2-145">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="e7be2-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e7be2-146">実際の呼び出しでは、すべて既定のプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="e7be2-146">All the default properties are returned in an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="e7be2-147">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="e7be2-147">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e7be2-148">C#</span><span class="sxs-lookup"><span data-stu-id="e7be2-148">c</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e7be2-149">Javascript</span><span class="sxs-lookup"><span data-stu-id="e7be2-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_group-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

#### <a name="request-2"></a><span data-ttu-id="e7be2-150">要求 2</span><span class="sxs-lookup"><span data-stu-id="e7be2-150">Request 2</span></span>
<span data-ttu-id="e7be2-151">`$select` クエリ オプションを使用して、既定では返されないいくつかのプロパティを取得する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e7be2-151">The next example uses a `$select` query option to get a few properties that are not returned by default.</span></span> 
<!-- {
  "blockType": "request",
  "sampleKeys": ["b320ee12-b1cd-4cca-b648-a437be61c5cd"],
  "name": "get_group_non_default"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/b320ee12-b1cd-4cca-b648-a437be61c5cd?$select=allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount
```

#### <a name="response-2"></a><span data-ttu-id="e7be2-152">応答 2</span><span class="sxs-lookup"><span data-stu-id="e7be2-152">Response 2</span></span>
<span data-ttu-id="e7be2-153">要求された既定以外のプロパティを含む応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e7be2-153">The following is an example of the response which includes the requested non-default properties.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="e7be2-154">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="e7be2-154">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e7be2-155">C#</span><span class="sxs-lookup"><span data-stu-id="e7be2-155">c</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_group_non_default-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e7be2-156">Javascript</span><span class="sxs-lookup"><span data-stu-id="e7be2-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_group_non_default-Javascript-snippets.md)]

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
    "Error: /api-reference/v1.0/api/group-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/group-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
