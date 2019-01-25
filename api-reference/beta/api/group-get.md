---
title: グループを取得する
description: グループ オブジェクトのプロパティとリレーションシップを取得します。
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: 18eb80938247d56326620a6ac866073acad6f715
ms.sourcegitcommit: 7d94b581f7c6dc1995efecf6ee21b604c0b80998
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/19/2019
ms.locfileid: "29353077"
---
# <a name="get-group"></a><span data-ttu-id="c915c-103">グループを取得する</span><span class="sxs-lookup"><span data-stu-id="c915c-103">Get group</span></span>

> <span data-ttu-id="c915c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c915c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c915c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c915c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c915c-106">[group](../resources/group.md) オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="c915c-106">Get the properties and relationships of a group object.</span></span>

<span data-ttu-id="c915c-107">「[プロパティ](../resources/group.md#properties)」セクションに記載されているように、この操作は既定ですべての使用できるプロパティのサブセットのみを返します。</span><span class="sxs-lookup"><span data-stu-id="c915c-107">This operation returns by default only a subset of all the available properties, as noted in the [Properties](../resources/group.md#properties) section.</span></span> 

<span data-ttu-id="c915c-108">既定では_返されない_プロパティを取得するには、`$select` OData クエリ オプションでそれらを指定します。</span><span class="sxs-lookup"><span data-stu-id="c915c-108">To get properties that are _not_ returned by default, specify them in a `$select` OData query option.</span></span> <span data-ttu-id="c915c-109">`$select` の[例](#request-2)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c915c-109">See an [example](#request-2) of the `$select` header in use.</span></span> <span data-ttu-id="c915c-110">例外は **hasMembersWithLicenseErrors** プロパティです。</span><span class="sxs-lookup"><span data-stu-id="c915c-110">An exception is the **hasMembersWithLicenseErrors** property.</span></span> <span data-ttu-id="c915c-111">このプロパティの使用方法の[例](group-list.md#request-2)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c915c-111">See an [example](group-list.md#request-2) of how to use this property.</span></span>

<span data-ttu-id="c915c-112">**グループ** リソースは[拡張機能](/graph/extensibility-overview)をサポートしているため、`GET` 操作を使用して、**グループ** インスタンスでカスタム プロパティと拡張機能データを取得することもできます。</span><span class="sxs-lookup"><span data-stu-id="c915c-112">Since the **post** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **post** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="c915c-113">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c915c-113">Permissions</span></span>
<span data-ttu-id="c915c-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c915c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c915c-116">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c915c-116">Permission type</span></span>      | <span data-ttu-id="c915c-117">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c915c-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c915c-118">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c915c-118">Delegated (work or school account)</span></span> | <span data-ttu-id="c915c-119">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c915c-119">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c915c-120">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c915c-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c915c-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c915c-121">Not supported.</span></span>    |
|<span data-ttu-id="c915c-122">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c915c-122">Application</span></span> | <span data-ttu-id="c915c-123">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c915c-123">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c915c-124">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c915c-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c915c-125">省略可能なクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="c915c-125">Optional query parameters</span></span>
<span data-ttu-id="c915c-126">既定では返されないものも含め、特定のグループのプロパティを取得するには `$select` を使用できます。</span><span class="sxs-lookup"><span data-stu-id="c915c-126">You can use `$select` to get specific group properties, including those that are not returned by default.</span></span> <span data-ttu-id="c915c-127">次の[例](#request-2)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c915c-127">See an [example](#request-2).</span></span>

<span data-ttu-id="c915c-128">OData クエリ オプションの詳細については、「[OData クエリ パラメーター](/graph/query-parameters)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c915c-128">For more information on OData query options, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="c915c-129">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c915c-129">Request headers</span></span>
| <span data-ttu-id="c915c-130">名前</span><span class="sxs-lookup"><span data-stu-id="c915c-130">Name</span></span>       | <span data-ttu-id="c915c-131">型</span><span class="sxs-lookup"><span data-stu-id="c915c-131">Type</span></span> | <span data-ttu-id="c915c-132">説明</span><span class="sxs-lookup"><span data-stu-id="c915c-132">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c915c-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="c915c-133">Authorization</span></span>  | <span data-ttu-id="c915c-134">string</span><span class="sxs-lookup"><span data-stu-id="c915c-134">string</span></span>  | <span data-ttu-id="c915c-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c915c-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c915c-137">要求本文</span><span class="sxs-lookup"><span data-stu-id="c915c-137">Request body</span></span>
<span data-ttu-id="c915c-138">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c915c-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c915c-139">応答</span><span class="sxs-lookup"><span data-stu-id="c915c-139">Response</span></span>
<span data-ttu-id="c915c-140">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [group](../resources/group.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c915c-140">If successful, this method returns a `200 OK` response code and [group](../resources/group.md) object in the response body.</span></span> <span data-ttu-id="c915c-141">`$select` を使用して特定のプロパティを指定していない限り、既定のプロパティを返します。</span><span class="sxs-lookup"><span data-stu-id="c915c-141">It returns the default properties unless you use `$select` to specify specific properties.</span></span>

## <a name="example"></a><span data-ttu-id="c915c-142">例</span><span class="sxs-lookup"><span data-stu-id="c915c-142">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="c915c-143">要求 1</span><span class="sxs-lookup"><span data-stu-id="c915c-143">Request 1</span></span>
<span data-ttu-id="c915c-144">GET 要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c915c-144">The following is an example of a request.</span></span> 
<!-- {
  "blockType": "request",
  "sampleKeys": ["45b7d2e7-b882-4a80-ba97-10b7a63b8fa4"],
  "name": "get_group"
}-->
```http
GET https://graph.microsoft.com/beta/groups/45b7d2e7-b882-4a80-ba97-10b7a63b8fa4
```

#### <a name="response-1"></a><span data-ttu-id="c915c-145">応答 1</span><span class="sxs-lookup"><span data-stu-id="c915c-145">Response 1</span></span>
<span data-ttu-id="c915c-146">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c915c-146">The following is an example of the response.</span></span> <span data-ttu-id="c915c-147">既定のプロパティのみが含まれています。</span><span class="sxs-lookup"><span data-stu-id="c915c-147">It includes only the default properties.</span></span>

><span data-ttu-id="c915c-148">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="c915c-148">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c915c-149">実際の呼び出しでは、すべて既定のプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="c915c-149">All the default properties are returned in an actual call.</span></span>
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

#### <a name="request-2"></a><span data-ttu-id="c915c-150">要求 2</span><span class="sxs-lookup"><span data-stu-id="c915c-150">Request 2</span></span>
<span data-ttu-id="c915c-151">`$select` クエリ オプションを使用して、既定では返されないいくつかのプロパティを取得する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c915c-151">The next example uses a `$select` query option to get a few properties that are not returned by default.</span></span> 
<!-- {
  "blockType": "request",
  "sampleKeys": ["b320ee12-b1cd-4cca-b648-a437be61c5cd"],
  "name": "get_group_non_default"
}-->
```http
GET https://graph.microsoft.com/beta/groups/b320ee12-b1cd-4cca-b648-a437be61c5cd?$select=allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount
```

#### <a name="response-2"></a><span data-ttu-id="c915c-152">応答 2</span><span class="sxs-lookup"><span data-stu-id="c915c-152">Response 2</span></span>
<span data-ttu-id="c915c-153">要求された既定以外のプロパティを含む応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c915c-153">The following is an example of the response which includes the requested non-default properties.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="c915c-154">関連項目</span><span class="sxs-lookup"><span data-stu-id="c915c-154">See also</span></span>

- [<span data-ttu-id="c915c-155">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="c915c-155">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="c915c-156">オープン拡張機能を使用してカスタム データをユーザーに追加する</span><span class="sxs-lookup"><span data-stu-id="c915c-156">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="c915c-157">スキーマ拡張機能を使用したグループへのカスタム データの追加</span><span class="sxs-lookup"><span data-stu-id="c915c-157">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
