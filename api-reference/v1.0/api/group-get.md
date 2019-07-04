---
title: グループを取得する
description: グループ オブジェクトのプロパティとリレーションシップを取得します。
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: ef0a798833f00188cb92310ee4f56e5749320a2a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35460869"
---
# <a name="get-group"></a><span data-ttu-id="825b4-103">グループを取得する</span><span class="sxs-lookup"><span data-stu-id="825b4-103">Get group</span></span>

<span data-ttu-id="825b4-104">グループ オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="825b4-104">Get the properties and relationships of a group object.</span></span>

<span data-ttu-id="825b4-105">「[プロパティ](../resources/group.md#properties)」セクションに記載されているように、この操作は既定ですべての使用できるプロパティのサブセットのみを返します。</span><span class="sxs-lookup"><span data-stu-id="825b4-105">This operation returns by default only a subset of all the available properties, as noted in the [Properties](../resources/group.md#properties) section.</span></span> <span data-ttu-id="825b4-106">既定では_返されない_プロパティを取得するには、`$select` OData クエリ オプションでそれらを指定します。</span><span class="sxs-lookup"><span data-stu-id="825b4-106">To get properties that are _not_ returned by default, specify them in a `$select` OData query option.</span></span> <span data-ttu-id="825b4-107">**hasMembersWithLicenseErrors** プロパティは例外で、`$select` クエリでは返されません。</span><span class="sxs-lookup"><span data-stu-id="825b4-107">The **hasMembersWithLicenseErrors** property is an exception and is not returned in the `$select` query.</span></span>

## <a name="permissions"></a><span data-ttu-id="825b4-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="825b4-108">Permissions</span></span>
<span data-ttu-id="825b4-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="825b4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="825b4-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="825b4-111">Permission type</span></span>      | <span data-ttu-id="825b4-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="825b4-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="825b4-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="825b4-113">Delegated (work or school account)</span></span> | <span data-ttu-id="825b4-114">Group.Read.All、Directory.Read.All、Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="825b4-114">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="825b4-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="825b4-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="825b4-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="825b4-116">Not supported.</span></span>    |
|<span data-ttu-id="825b4-117">Application</span><span class="sxs-lookup"><span data-stu-id="825b4-117">Application</span></span> | <span data-ttu-id="825b4-118">Group.Read.All、Directory.Read.All、Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="825b4-118">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

><span data-ttu-id="825b4-119">**注:** アクセスするグループの機能によっては、アクセス許可が制限される場合があります。</span><span class="sxs-lookup"><span data-stu-id="825b4-119">**Note:** Depending on the group features you're trying to access, permissions might be limited.</span></span> <span data-ttu-id="825b4-120">詳細については、「[Microsoft Graph に関する既知の問題](/graph/known-issues)」の[グループ](/graph/known-issues#groups) セクションを参照してください。</span><span class="sxs-lookup"><span data-stu-id="825b4-120">For more information, see the [Groups](/graph/known-issues#groups) section in [Known issues with Microsoft Graph](/graph/known-issues).</span></span>

## <a name="http-request"></a><span data-ttu-id="825b4-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="825b4-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="825b4-122">省略可能なクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="825b4-122">Optional query parameters</span></span>
<span data-ttu-id="825b4-123">既定では返されないものも含め、特定のグループのプロパティを取得するには `$select` を使用できます。</span><span class="sxs-lookup"><span data-stu-id="825b4-123">You can use `$select` to get specific group properties, including those that are not returned by default.</span></span>

<span data-ttu-id="825b4-124">OData クエリ オプションの詳細については、「[OData クエリ パラメーター](/graph/query-parameters)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="825b4-124">For more information on OData query options, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="825b4-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="825b4-125">Request headers</span></span>
| <span data-ttu-id="825b4-126">名前</span><span class="sxs-lookup"><span data-stu-id="825b4-126">Name</span></span>       | <span data-ttu-id="825b4-127">型</span><span class="sxs-lookup"><span data-stu-id="825b4-127">Type</span></span> | <span data-ttu-id="825b4-128">説明</span><span class="sxs-lookup"><span data-stu-id="825b4-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="825b4-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="825b4-129">Authorization</span></span>  | <span data-ttu-id="825b4-130">string</span><span class="sxs-lookup"><span data-stu-id="825b4-130">string</span></span>  | <span data-ttu-id="825b4-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="825b4-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="825b4-133">要求本文</span><span class="sxs-lookup"><span data-stu-id="825b4-133">Request body</span></span>
<span data-ttu-id="825b4-134">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="825b4-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="825b4-135">応答</span><span class="sxs-lookup"><span data-stu-id="825b4-135">Response</span></span>
<span data-ttu-id="825b4-136">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [group](../resources/group.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="825b4-136">If successful, this method returns a `200 OK` response code and [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="825b4-137">`$select` を使用して特定のプロパティを指定していない限り、既定のプロパティを返します。</span><span class="sxs-lookup"><span data-stu-id="825b4-137">It returns the default properties unless you use `$select` to specify specific properties.</span></span>

## <a name="example"></a><span data-ttu-id="825b4-138">例</span><span class="sxs-lookup"><span data-stu-id="825b4-138">Example</span></span>

### <a name="example-1-return-all-default-properties"></a><span data-ttu-id="825b4-139">例 1: すべての既定のプロパティを返す</span><span class="sxs-lookup"><span data-stu-id="825b4-139">Example 1: Return all default properties</span></span>

<span data-ttu-id="825b4-140">すべての既定のプロパティを返します。</span><span class="sxs-lookup"><span data-stu-id="825b4-140">Return all default properties.</span></span>

#### <a name="request"></a><span data-ttu-id="825b4-141">要求</span><span class="sxs-lookup"><span data-stu-id="825b4-141">Request</span></span> 

<span data-ttu-id="825b4-142">GET 要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="825b4-142">The following is an example of a GET request.</span></span> 

# <a name="httptabhttp"></a>[<span data-ttu-id="825b4-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="825b4-143">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["b320ee12-b1cd-4cca-b648-a437be61c5cd"],
  "name": "get_group"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/b320ee12-b1cd-4cca-b648-a437be61c5cd
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="825b4-144">C#</span><span class="sxs-lookup"><span data-stu-id="825b4-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="825b4-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="825b4-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="825b4-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="825b4-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="825b4-147">応答</span><span class="sxs-lookup"><span data-stu-id="825b4-147">Response</span></span>
<span data-ttu-id="825b4-148">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="825b4-148">The following is an example of the response.</span></span> <span data-ttu-id="825b4-149">既定のプロパティのみが含まれています。</span><span class="sxs-lookup"><span data-stu-id="825b4-149">It includes only the default properties.</span></span>

><span data-ttu-id="825b4-150">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="825b4-150">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="825b4-151">実際の呼び出しでは、すべて既定のプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="825b4-151">All the default properties are returned in an actual call.</span></span>

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


### <a name="example-2-return-additional-properties-by-using-select"></a><span data-ttu-id="825b4-152">例 2: $select を使って追加のプロパティを返す</span><span class="sxs-lookup"><span data-stu-id="825b4-152">Example 2: Return additional properties by using $select</span></span>

<span data-ttu-id="825b4-153">`$select` を使って追加のプロパティを返します。</span><span class="sxs-lookup"><span data-stu-id="825b4-153">Return additional properties by using `$select`.</span></span>

#### <a name="request"></a><span data-ttu-id="825b4-154">要求</span><span class="sxs-lookup"><span data-stu-id="825b4-154">Request</span></span>

<span data-ttu-id="825b4-155">GET 要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="825b4-155">The following is an example of a GET request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="825b4-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="825b4-156">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["b320ee12-b1cd-4cca-b648-a437be61c5cd"],
  "name": "get_group_non_default"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/b320ee12-b1cd-4cca-b648-a437be61c5cd?$select=allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="825b4-157">C#</span><span class="sxs-lookup"><span data-stu-id="825b4-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-non-default-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="825b4-158">Javascript</span><span class="sxs-lookup"><span data-stu-id="825b4-158">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-non-default-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="825b4-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="825b4-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-non-default-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="825b4-160">応答</span><span class="sxs-lookup"><span data-stu-id="825b4-160">Response</span></span>

<span data-ttu-id="825b4-161">要求された既定以外のプロパティを含む応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="825b4-161">The following is an example of the response which includes the requested non-default properties.</span></span>

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


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
