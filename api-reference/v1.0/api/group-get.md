---
title: グループを取得する
description: グループ オブジェクトのプロパティとリレーションシップを取得します。
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: edf1b53beaf519e86669e7ea8a472ea1562766af
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572676"
---
# <a name="get-group"></a><span data-ttu-id="4f314-103">グループを取得する</span><span class="sxs-lookup"><span data-stu-id="4f314-103">Get group</span></span>
<span data-ttu-id="4f314-104">グループ オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="4f314-104">Get the properties and relationships of a group object.</span></span>

<span data-ttu-id="4f314-105">「[プロパティ](../resources/group.md#properties)」セクションに記載されているように、この操作は既定ですべての使用できるプロパティのサブセットのみを返します。</span><span class="sxs-lookup"><span data-stu-id="4f314-105">This operation returns by default only a subset of all the available properties, as noted in the [Properties](../resources/group.md#properties) section.</span></span> <span data-ttu-id="4f314-106">既定では_返されない_プロパティを取得するには、`$select` OData クエリ オプションでそれらを指定します。</span><span class="sxs-lookup"><span data-stu-id="4f314-106">To get properties that are _not_ returned by default, specify them in a `$select` OData query option.</span></span> <span data-ttu-id="4f314-107">`$select` の[例](#request-2)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4f314-107">See an [example](#request-2) of  `$select`.</span></span> <span data-ttu-id="4f314-108">例外は **hasMembersWithLicenseErrors** プロパティです。</span><span class="sxs-lookup"><span data-stu-id="4f314-108">An exception is the **hasMembersWithLicenseErrors** property.</span></span> <span data-ttu-id="4f314-109">このプロパティの使用方法の[例](group-list.md#request-2)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4f314-109">See an [example](group-list.md#request-2) of how to use this property.</span></span>

## <a name="permissions"></a><span data-ttu-id="4f314-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4f314-110">Permissions</span></span>
<span data-ttu-id="4f314-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4f314-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f314-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4f314-113">Permission type</span></span>      | <span data-ttu-id="4f314-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4f314-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4f314-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4f314-115">Delegated (work or school account)</span></span> | <span data-ttu-id="4f314-116">Group.Read.All、Group.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f314-116">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="4f314-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4f314-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f314-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4f314-118">Not supported.</span></span>    |
|<span data-ttu-id="4f314-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4f314-119">Application</span></span> | <span data-ttu-id="4f314-120">Group.Read.All、Group.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f314-120">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4f314-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4f314-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4f314-122">省略可能なクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="4f314-122">Optional query parameters</span></span>
<span data-ttu-id="4f314-123">既定では返されないものも含め、特定のグループのプロパティを取得するには `$select` を使用できます。</span><span class="sxs-lookup"><span data-stu-id="4f314-123">You can use `$select` to get specific group properties, including those that are not returned by default.</span></span> <span data-ttu-id="4f314-124">次の[例](#request-2)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4f314-124">See an [example](#request-2) below.</span></span>

<span data-ttu-id="4f314-125">OData クエリ オプションの詳細については、「[OData クエリ パラメーター](/graph/query-parameters)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4f314-125">For more information on OData query options, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="4f314-126">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4f314-126">Request headers</span></span>
| <span data-ttu-id="4f314-127">名前</span><span class="sxs-lookup"><span data-stu-id="4f314-127">Name</span></span>       | <span data-ttu-id="4f314-128">型</span><span class="sxs-lookup"><span data-stu-id="4f314-128">Type</span></span> | <span data-ttu-id="4f314-129">説明</span><span class="sxs-lookup"><span data-stu-id="4f314-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4f314-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="4f314-130">Authorization</span></span>  | <span data-ttu-id="4f314-131">string</span><span class="sxs-lookup"><span data-stu-id="4f314-131">string</span></span>  | <span data-ttu-id="4f314-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4f314-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4f314-134">要求本文</span><span class="sxs-lookup"><span data-stu-id="4f314-134">Request body</span></span>
<span data-ttu-id="4f314-135">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="4f314-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4f314-136">応答</span><span class="sxs-lookup"><span data-stu-id="4f314-136">Response</span></span>
<span data-ttu-id="4f314-137">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [group](../resources/group.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4f314-137">If successful, this method returns a `200 OK` response code and [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="4f314-138">`$select` を使用して特定のプロパティを指定していない限り、既定のプロパティを返します。</span><span class="sxs-lookup"><span data-stu-id="4f314-138">It returns the default properties unless you use `$select` to specify specific properties.</span></span>

## <a name="example"></a><span data-ttu-id="4f314-139">例</span><span class="sxs-lookup"><span data-stu-id="4f314-139">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="4f314-140">要求 1</span><span class="sxs-lookup"><span data-stu-id="4f314-140">Request 1</span></span>
<span data-ttu-id="4f314-141">GET 要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4f314-141">The following is an example of a GET request.</span></span> 
<!-- {
  "blockType": "request",
  "sampleKeys": ["b320ee12-b1cd-4cca-b648-a437be61c5cd"],
  "name": "get_group"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/b320ee12-b1cd-4cca-b648-a437be61c5cd
```

#### <a name="response-1"></a><span data-ttu-id="4f314-142">応答 1</span><span class="sxs-lookup"><span data-stu-id="4f314-142">Response 1</span></span>
<span data-ttu-id="4f314-143">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4f314-143">The following is an example of the response.</span></span> <span data-ttu-id="4f314-144">既定のプロパティのみが含まれています。</span><span class="sxs-lookup"><span data-stu-id="4f314-144">It includes only the default properties.</span></span>

><span data-ttu-id="4f314-145">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="4f314-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4f314-146">実際の呼び出しでは、すべて既定のプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="4f314-146">All the default properties are returned in an actual call.</span></span>
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

#### <a name="request-2"></a><span data-ttu-id="4f314-147">要求 2</span><span class="sxs-lookup"><span data-stu-id="4f314-147">Request 2</span></span>
<span data-ttu-id="4f314-148">`$select` クエリ オプションを使用して、既定では返されないいくつかのプロパティを取得する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4f314-148">The next example uses a `$select` query option to get a few properties that are not returned by default.</span></span> 
<!-- {
  "blockType": "request",
  "sampleKeys": ["b320ee12-b1cd-4cca-b648-a437be61c5cd"],
  "name": "get_group_non_default"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/b320ee12-b1cd-4cca-b648-a437be61c5cd?$select=allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount
```

#### <a name="response-2"></a><span data-ttu-id="4f314-149">応答 2</span><span class="sxs-lookup"><span data-stu-id="4f314-149">Response 2</span></span>
<span data-ttu-id="4f314-150">要求された既定以外のプロパティを含む応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4f314-150">The following is an example of the response which includes the requested non-default properties.</span></span>

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
  "tocPath": ""
}-->
