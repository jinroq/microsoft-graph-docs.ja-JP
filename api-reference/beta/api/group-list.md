---
title: グループの一覧表示
description: Office 365 グループを含み、それに限定されない組織で使用可能なすべてのグループを一覧表示します。
localization_priority: Priority
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 11faba0b03b2e82c3086481dab617cd34ffa0d64
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35953627"
---
# <a name="list-groups"></a><span data-ttu-id="19e9f-103">グループの一覧表示</span><span class="sxs-lookup"><span data-stu-id="19e9f-103">List groups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="19e9f-104">Office 365 グループを含み、それに限定されない組織のすべてのグループを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="19e9f-104">List all the groups available in an organization, including but not limited to Office 365 Groups.</span></span> 

<span data-ttu-id="19e9f-105">この操作は既定で各グループで頻繁に使用されるプロパティのサブセットのみを返します。</span><span class="sxs-lookup"><span data-stu-id="19e9f-105">This operation returns by default only a subset of the more commonly used properties for each group.</span></span> <span data-ttu-id="19e9f-106">これらの_既定_のプロパティは、「[プロパティ](../resources/group.md#properties)」セクションに記載されています。</span><span class="sxs-lookup"><span data-stu-id="19e9f-106">These _default_ properties are noted in the [Properties](../resources/group.md#properties) section.</span></span> <span data-ttu-id="19e9f-107">既定で_返されない_プロパティを取得するには、グループに対して [GET 操作](group-get.md)を実行し、`$select` OData クエリ オプションでプロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="19e9f-107">To get properties that are _not_ returned by default, do a [GET](group-get.md) operation for the group and specify the properties in a `$select` OData query option.</span></span> <span data-ttu-id="19e9f-108">**hasMembersWithLicenseErrors** プロパティは例外で、`$select` クエリでは返されません。</span><span class="sxs-lookup"><span data-stu-id="19e9f-108">The **hasMembersWithLicenseErrors** property is an exception and is not returned in the `$select` query.</span></span>

## <a name="permissions"></a><span data-ttu-id="19e9f-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="19e9f-109">Permissions</span></span>
<span data-ttu-id="19e9f-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="19e9f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19e9f-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="19e9f-112">Permission type</span></span>      | <span data-ttu-id="19e9f-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="19e9f-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="19e9f-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="19e9f-114">Delegated (work or school account)</span></span> | <span data-ttu-id="19e9f-115">Group.Read.All、Directory.Read.All、Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="19e9f-115">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="19e9f-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="19e9f-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19e9f-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="19e9f-117">Not supported.</span></span>    |
|<span data-ttu-id="19e9f-118">Application</span><span class="sxs-lookup"><span data-stu-id="19e9f-118">Application</span></span> | <span data-ttu-id="19e9f-119">Group.Read.All、Directory.Read.All、Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19e9f-119">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="19e9f-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="19e9f-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="19e9f-121">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="19e9f-121">Optional query parameters</span></span>

<span data-ttu-id="19e9f-122">Office 365 グループ (別名統合グループ) のみを一覧表示するには、**groupTypes** にフィルターを適用します。</span><span class="sxs-lookup"><span data-stu-id="19e9f-122">To list only Office 365 Groups (aka unified groups), apply a filter on **groupTypes**:</span></span>
<!-- { "blockType": "ignored" } -->
```
GET https://graph.microsoft.com/beta/groups?$filter=groupTypes/any(c:c+eq+'Unified')
```

<span data-ttu-id="19e9f-123">OData クエリ オプション `$orderby` を使用して、以下の例のように、組織内のグループを **displayName** 値で並べ替えることができます。</span><span class="sxs-lookup"><span data-stu-id="19e9f-123">You can use the OData query option `$orderby` to sort groups in an organization by the **displayName** values, as shown in the following example:</span></span>
<!-- { "blockType": "ignored" } -->
```
GET https://graph.microsoft.com/beta/groups?$orderby=displayName
```

<span data-ttu-id="19e9f-124">OData クエリ オプションの詳細については、「[OData クエリ パラメーター](/graph/query-parameters)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="19e9f-124">For more information on OData query options, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="19e9f-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="19e9f-125">Request headers</span></span>
| <span data-ttu-id="19e9f-126">名前</span><span class="sxs-lookup"><span data-stu-id="19e9f-126">Name</span></span>       | <span data-ttu-id="19e9f-127">種類</span><span class="sxs-lookup"><span data-stu-id="19e9f-127">Type</span></span> | <span data-ttu-id="19e9f-128">説明</span><span class="sxs-lookup"><span data-stu-id="19e9f-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="19e9f-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="19e9f-129">Authorization</span></span>  | <span data-ttu-id="19e9f-130">string</span><span class="sxs-lookup"><span data-stu-id="19e9f-130">string</span></span>  | <span data-ttu-id="19e9f-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="19e9f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="19e9f-133">要求本文</span><span class="sxs-lookup"><span data-stu-id="19e9f-133">Request body</span></span>
<span data-ttu-id="19e9f-134">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="19e9f-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="19e9f-135">応答</span><span class="sxs-lookup"><span data-stu-id="19e9f-135">Response</span></span>
<span data-ttu-id="19e9f-136">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [group](../resources/group.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="19e9f-136">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span> <span data-ttu-id="19e9f-137">応答には、各グループの既定のプロパティのみが含まれています。</span><span class="sxs-lookup"><span data-stu-id="19e9f-137">The response includes only the default properties of each group.</span></span>

## <a name="example"></a><span data-ttu-id="19e9f-138">例</span><span class="sxs-lookup"><span data-stu-id="19e9f-138">Example</span></span>

### <a name="example-1-return-a-list-of-group-objects"></a><span data-ttu-id="19e9f-139">例 1: グループ オブジェクトのリストを取得する</span><span class="sxs-lookup"><span data-stu-id="19e9f-139">Example 1: Return a list of group objects</span></span>

#### <a name="request"></a><span data-ttu-id="19e9f-140">要求</span><span class="sxs-lookup"><span data-stu-id="19e9f-140">Request</span></span>

<span data-ttu-id="19e9f-141">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="19e9f-141">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="19e9f-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="19e9f-142">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_groups"
}-->
```http
GET https://graph.microsoft.com/beta/groups
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="19e9f-143">C#</span><span class="sxs-lookup"><span data-stu-id="19e9f-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="19e9f-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="19e9f-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="19e9f-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="19e9f-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="19e9f-146">Java</span><span class="sxs-lookup"><span data-stu-id="19e9f-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-groups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="19e9f-147">応答</span><span class="sxs-lookup"><span data-stu-id="19e9f-147">Response</span></span>

<span data-ttu-id="19e9f-148">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="19e9f-148">The following is an example of the response.</span></span>
><span data-ttu-id="19e9f-149">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="19e9f-149">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="19e9f-150">実際の呼び出しでは、各グループのすべての既定のプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="19e9f-150">All the default properties are returned for each group in an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true,
  "name": "get_groups"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups",
    "value": [
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
        },
        {
            "id": "d7797254-3084-44d0-99c9-a3b5ab149538",
            "deletedDateTime": null,
            "classification": null,
            "createdDateTime": "2018-11-19T20:29:40Z",
            "description": "Talk about golf",
            "displayName": "Golf Discussion",
            "expirationDateTime": null,
            "groupTypes": [],
            "mail": "golftalk@contoso.com",
            "mailEnabled": true,
            "mailNickname": "golftalk",
            "membershipRule": null,
            "membershipRuleProcessingState": null,
            "onPremisesLastSyncDateTime": null,
            "onPremisesSecurityIdentifier": null,
            "onPremisesSyncEnabled": null,
            "preferredDataLocation": "CAN",
            "preferredLanguage": null,
            "proxyAddresses": [
                "smtp:golftalk@contoso.onmicrosoft.com",
                "SMTP:golftalk@contoso.com"
            ],
            "renewedDateTime": "2018-11-19T20:29:40Z",
            "resourceBehaviorOptions": [],
            "resourceProvisioningOptions": [],
            "securityEnabled": false,
            "theme": null,
            "visibility": null,
            "onPremisesProvisioningErrors": []
        }
    ]
}

```


### <a name="example-2-return-a-filtered-list-of-group-objects"></a><span data-ttu-id="19e9f-151">例 2: フィルター処理されたグループ オブジェクトのリストを返す</span><span class="sxs-lookup"><span data-stu-id="19e9f-151">Example 2: Return a filtered list of group objects</span></span> 

#### <a name="request"></a><span data-ttu-id="19e9f-152">要求</span><span class="sxs-lookup"><span data-stu-id="19e9f-152">Request</span></span>

<span data-ttu-id="19e9f-153">この例では、`$filter` クエリ オプションを使用して、グループ ベースのライセンス割り当てによるライセンス エラーが発生したメンバーが含まれているグループを取得します。</span><span class="sxs-lookup"><span data-stu-id="19e9f-153">This example uses a `$filter` query option to get those groups that have members with license errors from their group-based license assignments.</span></span> <span data-ttu-id="19e9f-154">また、`$select` クエリ オプションも使用して、各グループの **id** プロパティと **displayName** プロパティのみを応答で取得します (その他の既定または既定以外のプロパティは取得しません)。</span><span class="sxs-lookup"><span data-stu-id="19e9f-154">It also uses a `$select` query option to get only the **id** and **displayName** properties of each group in the response, and not other default or non-default properties.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="19e9f-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="19e9f-155">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_groups_withlicenseerrors"
}-->
```http
GET https://graph.microsoft.com/beta/groups?$filter=hasMembersWithLicenseErrors+eq+true&$select=id,displayName
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="19e9f-156">C#</span><span class="sxs-lookup"><span data-stu-id="19e9f-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-groups-withlicenseerrors-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="19e9f-157">Javascript</span><span class="sxs-lookup"><span data-stu-id="19e9f-157">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-groups-withlicenseerrors-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="19e9f-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="19e9f-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-groups-withlicenseerrors-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="19e9f-159">Java</span><span class="sxs-lookup"><span data-stu-id="19e9f-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-groups-withlicenseerrors-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="19e9f-160">応答</span><span class="sxs-lookup"><span data-stu-id="19e9f-160">Response</span></span>

<span data-ttu-id="19e9f-161">要求したプロパティのみを含む応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="19e9f-161">The following is an example of the response which includes only the requested properties.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true,
  "name": "get_groups_withlicenseerrors"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups(id,displayName)",
    "value": [
        {
            "id": "b320ee12-b1cd-4cca-b648-a437be61c5cd",
            "displayName": "Library Assist"
        },
        {
            "id": "45b7d2e7-b882-4a80-ba97-10b7a63b8fa4",
            "displayName": "Golf Assist"
        }
    ]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List groups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
