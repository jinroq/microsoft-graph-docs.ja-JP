---
title: グループを取得する
description: グループ オブジェクトのプロパティとリレーションシップを取得します。
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: 92b9c8de30f0070491d84acf9cfc56225c1a7981
ms.sourcegitcommit: 7d94b581f7c6dc1995efecf6ee21b604c0b80998
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/19/2019
ms.locfileid: "29353091"
---
# <a name="get-group"></a><span data-ttu-id="e22b1-103">グループを取得する</span><span class="sxs-lookup"><span data-stu-id="e22b1-103">Get group</span></span>
<span data-ttu-id="e22b1-104">グループ オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="e22b1-104">Get the properties and relationships of a group object.</span></span>

<span data-ttu-id="e22b1-105">「[プロパティ](../resources/group.md#properties)」セクションに記載されているように、この操作は既定ですべての使用できるプロパティのサブセットのみを返します。</span><span class="sxs-lookup"><span data-stu-id="e22b1-105">This operation returns by default only a subset of all the available properties, as noted in the [Properties](../resources/group.md#properties) section.</span></span> <span data-ttu-id="e22b1-106">既定では_返されない_プロパティを取得するには、`$select` OData クエリ オプションでそれらを指定します。</span><span class="sxs-lookup"><span data-stu-id="e22b1-106">To get properties that are _not_ returned by default, specify them in a `$select` OData query option.</span></span> <span data-ttu-id="e22b1-107">[例](#request-2)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e22b1-107">See an [example](#request-2).</span></span>

## <a name="permissions"></a><span data-ttu-id="e22b1-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e22b1-108">Permissions</span></span>
<span data-ttu-id="e22b1-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e22b1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e22b1-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e22b1-111">Permission type</span></span>      | <span data-ttu-id="e22b1-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e22b1-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e22b1-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e22b1-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e22b1-114">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e22b1-114">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e22b1-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e22b1-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e22b1-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e22b1-116">Not supported.</span></span>    |
|<span data-ttu-id="e22b1-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e22b1-117">Application</span></span> | <span data-ttu-id="e22b1-118">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e22b1-118">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e22b1-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e22b1-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e22b1-120">省略可能なクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e22b1-120">Optional query parameters</span></span>
<span data-ttu-id="e22b1-121">既定では返されないものも含め、特定のグループのプロパティを取得するには `$select` を使用できます。</span><span class="sxs-lookup"><span data-stu-id="e22b1-121">You can use `$select` to get specific group properties, including those that are not returned by default.</span></span> <span data-ttu-id="e22b1-122">次の[例](#request-2)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e22b1-122">See an [example](#request-2).</span></span>

<span data-ttu-id="e22b1-123">OData クエリ オプションの詳細については、「[OData クエリ パラメーター](/graph/query-parameters)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e22b1-123">For more information on OData query options, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e22b1-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e22b1-124">Request headers</span></span>
| <span data-ttu-id="e22b1-125">名前</span><span class="sxs-lookup"><span data-stu-id="e22b1-125">Name</span></span>       | <span data-ttu-id="e22b1-126">型</span><span class="sxs-lookup"><span data-stu-id="e22b1-126">Type</span></span> | <span data-ttu-id="e22b1-127">説明</span><span class="sxs-lookup"><span data-stu-id="e22b1-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e22b1-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="e22b1-128">Authorization</span></span>  | <span data-ttu-id="e22b1-129">string</span><span class="sxs-lookup"><span data-stu-id="e22b1-129">string</span></span>  | <span data-ttu-id="e22b1-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e22b1-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e22b1-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="e22b1-132">Request body</span></span>
<span data-ttu-id="e22b1-133">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e22b1-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e22b1-134">応答</span><span class="sxs-lookup"><span data-stu-id="e22b1-134">Response</span></span>
<span data-ttu-id="e22b1-135">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [group](../resources/group.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e22b1-135">If successful, this method returns a `200 OK` response code and [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="e22b1-136">`$select` を使用して特定のプロパティを指定していない限り、既定のプロパティを返します。</span><span class="sxs-lookup"><span data-stu-id="e22b1-136">It returns the default properties unless you use `$select` to specify specific properties.</span></span>

## <a name="example"></a><span data-ttu-id="e22b1-137">例</span><span class="sxs-lookup"><span data-stu-id="e22b1-137">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="e22b1-138">要求 1</span><span class="sxs-lookup"><span data-stu-id="e22b1-138">Request 1</span></span>
<span data-ttu-id="e22b1-139">GET 要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e22b1-139">The following is an example of a request.</span></span> 
<!-- {
  "blockType": "request",
  "sampleKeys": ["b320ee12-b1cd-4cca-b648-a437be61c5cd"],
  "name": "get_group"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/b320ee12-b1cd-4cca-b648-a437be61c5cd
```

#### <a name="response-1"></a><span data-ttu-id="e22b1-140">応答 1</span><span class="sxs-lookup"><span data-stu-id="e22b1-140">Response 1</span></span>
<span data-ttu-id="e22b1-141">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e22b1-141">The following is an example of the response.</span></span> <span data-ttu-id="e22b1-142">既定のプロパティのみが含まれています。</span><span class="sxs-lookup"><span data-stu-id="e22b1-142">It includes only the default properties.</span></span>

><span data-ttu-id="e22b1-143">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="e22b1-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e22b1-144">実際の呼び出しでは、すべて既定のプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="e22b1-144">All the default properties are returned in an actual call.</span></span>
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

#### <a name="request-2"></a><span data-ttu-id="e22b1-145">要求 2</span><span class="sxs-lookup"><span data-stu-id="e22b1-145">Request 2</span></span>
<span data-ttu-id="e22b1-146">`$select` クエリ オプションを使用して、既定では返されないいくつかのプロパティを取得する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e22b1-146">The next example uses a `$select` query option to get a few properties that are not returned by default.</span></span> 
<!-- {
  "blockType": "request",
  "sampleKeys": ["b320ee12-b1cd-4cca-b648-a437be61c5cd"],
  "name": "get_group_non_default"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/b320ee12-b1cd-4cca-b648-a437be61c5cd?$select=allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount
```

#### <a name="response-2"></a><span data-ttu-id="e22b1-147">応答 2</span><span class="sxs-lookup"><span data-stu-id="e22b1-147">Response 2</span></span>
<span data-ttu-id="e22b1-148">要求された既定以外のプロパティを含む応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e22b1-148">The following is an example of the response which includes the requested non-default properties.</span></span>

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
