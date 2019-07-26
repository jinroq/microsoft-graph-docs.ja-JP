---
title: グループを取得する
description: グループ オブジェクトのプロパティとリレーションシップを取得します。
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: 624906f0154045a232d04b5db2cc7556871128a3
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35858620"
---
# <a name="get-group"></a><span data-ttu-id="29c3c-103">グループを取得する</span><span class="sxs-lookup"><span data-stu-id="29c3c-103">Get group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29c3c-104">[group](../resources/group.md) オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="29c3c-104">Get the properties and relationships of a [group](../resources/group.md) object.</span></span> 

<span data-ttu-id="29c3c-105">「[プロパティ](../resources/group.md#properties)」セクションに記載されているように、この操作は既定ですべての使用できるプロパティのサブセットのみを返します。</span><span class="sxs-lookup"><span data-stu-id="29c3c-105">This operation returns by default only a subset of all the available properties, as noted in the [Properties](../resources/group.md#properties) section.</span></span> <span data-ttu-id="29c3c-106">既定では_返されない_プロパティを取得するには、`$select` OData クエリ オプションでそれらを指定します。</span><span class="sxs-lookup"><span data-stu-id="29c3c-106">To get properties that are _not_ returned by default, specify them in a `$select` OData query option.</span></span> <span data-ttu-id="29c3c-107">**hasMembersWithLicenseErrors** プロパティは例外で、`$select` クエリでは返されません。</span><span class="sxs-lookup"><span data-stu-id="29c3c-107">The **hasMembersWithLicenseErrors** property is an exception and is not returned in the `$select` query.</span></span> <span data-ttu-id="29c3c-108">**グループ** リソースは[拡張機能](/graph/extensibility-overview)をサポートしているため、`GET` 操作を使用して、**グループ** インスタンスでカスタム プロパティと拡張機能データを取得することもできます。</span><span class="sxs-lookup"><span data-stu-id="29c3c-108">Since the **group** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **group** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="29c3c-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="29c3c-109">Permissions</span></span>
<span data-ttu-id="29c3c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="29c3c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29c3c-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="29c3c-112">Permission type</span></span>      | <span data-ttu-id="29c3c-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="29c3c-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="29c3c-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="29c3c-114">Delegated (work or school account)</span></span> | <span data-ttu-id="29c3c-115">Group.Read.All、Group.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="29c3c-115">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="29c3c-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="29c3c-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29c3c-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="29c3c-117">Not supported.</span></span>    |
|<span data-ttu-id="29c3c-118">Application</span><span class="sxs-lookup"><span data-stu-id="29c3c-118">Application</span></span> | <span data-ttu-id="29c3c-119">Group.Read.All、Directory.Read.All、Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29c3c-119">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

><span data-ttu-id="29c3c-120">**注:** アクセスするグループの機能によっては、アクセス許可が制限される場合があります。</span><span class="sxs-lookup"><span data-stu-id="29c3c-120">**Note:** Depending on the group features you're trying to access, permissions might be limited.</span></span> <span data-ttu-id="29c3c-121">詳細については、「[Microsoft Graph に関する既知の問題](/graph/known-issues)」の[グループ](/graph/known-issues#groups) セクションを参照してください。</span><span class="sxs-lookup"><span data-stu-id="29c3c-121">For more information, see the [Groups](/graph/known-issues#groups) section in [Known issues with Microsoft Graph](/graph/known-issues).</span></span>

## <a name="http-request"></a><span data-ttu-id="29c3c-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="29c3c-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="29c3c-123">省略可能なクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="29c3c-123">Optional query parameters</span></span>
<span data-ttu-id="29c3c-124">既定では返されないものも含め、特定のグループのプロパティを取得するには `$select` を使用できます。</span><span class="sxs-lookup"><span data-stu-id="29c3c-124">You can use `$select` to get specific group properties, including those that are not returned by default.</span></span>

<span data-ttu-id="29c3c-125">OData クエリ オプションの詳細については、「[OData クエリ パラメーター](/graph/query-parameters)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="29c3c-125">For more information on OData query options, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="29c3c-126">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="29c3c-126">Request headers</span></span>
| <span data-ttu-id="29c3c-127">名前</span><span class="sxs-lookup"><span data-stu-id="29c3c-127">Name</span></span>       | <span data-ttu-id="29c3c-128">型</span><span class="sxs-lookup"><span data-stu-id="29c3c-128">Type</span></span> | <span data-ttu-id="29c3c-129">説明</span><span class="sxs-lookup"><span data-stu-id="29c3c-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="29c3c-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="29c3c-130">Authorization</span></span>  | <span data-ttu-id="29c3c-131">string</span><span class="sxs-lookup"><span data-stu-id="29c3c-131">string</span></span>  | <span data-ttu-id="29c3c-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="29c3c-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="29c3c-134">要求本文</span><span class="sxs-lookup"><span data-stu-id="29c3c-134">Request body</span></span>
<span data-ttu-id="29c3c-135">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="29c3c-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="29c3c-136">応答</span><span class="sxs-lookup"><span data-stu-id="29c3c-136">Response</span></span>
<span data-ttu-id="29c3c-137">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [group](../resources/group.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="29c3c-137">If successful, this method returns a `200 OK` response code and [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="29c3c-138">`$select` を使用して特定のプロパティを指定していない限り、既定のプロパティを返します。</span><span class="sxs-lookup"><span data-stu-id="29c3c-138">It returns the default properties unless you use `$select` to specify specific properties.</span></span>

## <a name="example"></a><span data-ttu-id="29c3c-139">例</span><span class="sxs-lookup"><span data-stu-id="29c3c-139">Example</span></span>

### <a name="example-1-return-all-default-properties"></a><span data-ttu-id="29c3c-140">例 1: すべての既定のプロパティを返す</span><span class="sxs-lookup"><span data-stu-id="29c3c-140">Example 1: Return all default properties</span></span>

#### <a name="request"></a><span data-ttu-id="29c3c-141">要求</span><span class="sxs-lookup"><span data-stu-id="29c3c-141">Request</span></span>

<span data-ttu-id="29c3c-142">GET 要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="29c3c-142">The following is an example of a GET request.</span></span> 

# <a name="httptabhttp"></a>[<span data-ttu-id="29c3c-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="29c3c-143">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["45b7d2e7-b882-4a80-ba97-10b7a63b8fa4"],
  "name": "get_group"
}-->
```http
GET https://graph.microsoft.com/beta/groups/45b7d2e7-b882-4a80-ba97-10b7a63b8fa4
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="29c3c-144">C#</span><span class="sxs-lookup"><span data-stu-id="29c3c-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="29c3c-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="29c3c-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="29c3c-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="29c3c-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="29c3c-147">Java</span><span class="sxs-lookup"><span data-stu-id="29c3c-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="29c3c-148">応答</span><span class="sxs-lookup"><span data-stu-id="29c3c-148">Response</span></span>
<span data-ttu-id="29c3c-149">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="29c3c-149">The following is an example of the response.</span></span> <span data-ttu-id="29c3c-150">既定のプロパティのみが含まれています。</span><span class="sxs-lookup"><span data-stu-id="29c3c-150">It includes only the default properties.</span></span>

><span data-ttu-id="29c3c-151">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="29c3c-151">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="29c3c-152">実際の呼び出しでは、すべて既定のプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="29c3c-152">All the default properties are returned in an actual call.</span></span>
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
  "id": "45b7d2e7-b882-4a80-ba97-10b7a63b8fa4",
  "deletedDateTime": null,
  "classification": null,
  "createdDateTime": "2018-12-22T02:21:05Z",
  "description": "Self help community for golf",
  "displayName": "Golf Assist",
  "expirationDateTime": null,
  "groupTypes": [
      "Unified"
  ],
  "mail": "golfassist@contoso.com",
  "mailEnabled": true,
  "mailNickname": "golfassist",
  "membershipRule": null,
  "membershipRuleProcessingState": null,
  "onPremisesLastSyncDateTime": null,
  "onPremisesSecurityIdentifier": null,
  "onPremisesSyncEnabled": null,
  "preferredDataLocation": "CAN",
  "preferredLanguage": null,
  "proxyAddresses": [
      "smtp:golfassist@contoso.onmicrosoft.com",
      "SMTP:golfassist@contoso.com"
  ],
  "renewedDateTime": "2018-12-22T02:21:05Z",
  "resourceBehaviorOptions": [],
  "resourceProvisioningOptions": [],
  "securityEnabled": false,
  "theme": null,
  "visibility": "Public",
  "onPremisesProvisioningErrors": []
}
```


### <a name="example-2-return-additional-properties-by-using-select"></a><span data-ttu-id="29c3c-153">例 2: $select を使って追加のプロパティを返す</span><span class="sxs-lookup"><span data-stu-id="29c3c-153">Example 2: Return additional properties by using $select</span></span>

#### <a name="request"></a><span data-ttu-id="29c3c-154">要求</span><span class="sxs-lookup"><span data-stu-id="29c3c-154">Request</span></span>

<span data-ttu-id="29c3c-155">GET 要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="29c3c-155">The following is an example of a GET request.</span></span> 


# <a name="httptabhttp"></a>[<span data-ttu-id="29c3c-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="29c3c-156">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["b320ee12-b1cd-4cca-b648-a437be61c5cd"],
  "name": "get_group_non_default"
}-->
```http
GET https://graph.microsoft.com/beta/groups/b320ee12-b1cd-4cca-b648-a437be61c5cd?$select=allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="29c3c-157">C#</span><span class="sxs-lookup"><span data-stu-id="29c3c-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-non-default-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="29c3c-158">Javascript</span><span class="sxs-lookup"><span data-stu-id="29c3c-158">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-non-default-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="29c3c-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="29c3c-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-non-default-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="29c3c-160">Java</span><span class="sxs-lookup"><span data-stu-id="29c3c-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-non-default-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="29c3c-161">応答</span><span class="sxs-lookup"><span data-stu-id="29c3c-161">Response</span></span>

<span data-ttu-id="29c3c-162">要求された既定以外のプロパティを含む応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="29c3c-162">The following is an example of the response which includes the requested non-default properties.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups(allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount)/$entity",
    "id": "b320ee12-b1cd-4cca-b648-a437be61c5cd",
    "allowExternalSenders": false,
    "autoSubscribeNewMembers": false,
    "isSubscribedByMail": false,
    "unseenCount": 0
}
```


## <a name="see-also"></a><span data-ttu-id="29c3c-163">関連項目</span><span class="sxs-lookup"><span data-stu-id="29c3c-163">See also</span></span>

- [<span data-ttu-id="29c3c-164">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="29c3c-164">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="29c3c-165">オープン拡張機能を使用してカスタム データをユーザーに追加する</span><span class="sxs-lookup"><span data-stu-id="29c3c-165">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="29c3c-166">スキーマ拡張機能を使用したグループへのカスタム データの追加</span><span class="sxs-lookup"><span data-stu-id="29c3c-166">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
