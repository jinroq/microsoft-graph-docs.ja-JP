---
title: グループの一覧表示
description: Office 365 のグループを含み、それに限定されない組織で使用可能なすべてのグループを一覧表示します。
ms.openlocfilehash: 2b46891a7570a831cd1b38ae29915e59475e8540
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066700"
---
# <a name="list-groups"></a><span data-ttu-id="76b9f-103">グループを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="76b9f-103">List groups</span></span>

> <span data-ttu-id="76b9f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="76b9f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="76b9f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="76b9f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="76b9f-p102">Office 365 のグループを含み、それに限定されない組織で使用可能なすべてのグループを一覧表示します。各グループの[既定のプロパティ](../api/group-get.md#default-properties)が返されます。</span><span class="sxs-lookup"><span data-stu-id="76b9f-p102">List all the groups available in an organization, including but not limited to Office 365 Groups. The [default properties](../api/group-get.md#default-properties) of each group are returned.</span></span>

<span data-ttu-id="76b9f-108">Office 365 グループ (別名統合グループ) のみを一覧表示するには、**groupTypes** にフィルターを適用します。</span><span class="sxs-lookup"><span data-stu-id="76b9f-108">To list only Office 365 Groups (aka unified groups), apply a filter on **groupTypes**:</span></span>
```
GET https://graph.microsoft.com/beta/groups?$filter=groupTypes/any(c:c+eq+'Unified')
```

<span data-ttu-id="76b9f-109">OData クエリ オプション `$orderby` を使用して、以下の例のように、組織内のグループを **displayName** 値で並べ替えることができます。</span><span class="sxs-lookup"><span data-stu-id="76b9f-109">You can use the OData query option `$orderby` to sort groups in an organization by the **displayName** values, as shown in the following example:</span></span>
```
GET https://graph.microsoft.com/beta/groups?$orderby=displayName
```

<span data-ttu-id="76b9f-110">ライセンス エラーのあるメンバーを含むグループを返すには、 **$filter**クエリ パラメーターを使用します。</span><span class="sxs-lookup"><span data-stu-id="76b9f-110">To return groups containing members with license errors, use the **$filter** query parameter:</span></span> 

```http 
GET https://graph.microsoft.com/beta/groups?$filter=hasMembersWithLicenseErrors+eq+true 
```
## <a name="permissions"></a><span data-ttu-id="76b9f-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="76b9f-111">Permissions</span></span>
<span data-ttu-id="76b9f-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="76b9f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76b9f-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="76b9f-114">Permission type</span></span>      | <span data-ttu-id="76b9f-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="76b9f-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="76b9f-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="76b9f-116">Delegated (work or school account)</span></span> | <span data-ttu-id="76b9f-117">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76b9f-117">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="76b9f-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="76b9f-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="76b9f-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="76b9f-119">Not supported.</span></span>    |
|<span data-ttu-id="76b9f-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="76b9f-120">Application</span></span> | <span data-ttu-id="76b9f-121">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76b9f-121">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="76b9f-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="76b9f-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="76b9f-123">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="76b9f-123">Optional query parameters</span></span>
<span data-ttu-id="76b9f-124">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="76b9f-124">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="76b9f-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="76b9f-125">Request headers</span></span>
| <span data-ttu-id="76b9f-126">名前</span><span class="sxs-lookup"><span data-stu-id="76b9f-126">Name</span></span>       | <span data-ttu-id="76b9f-127">型</span><span class="sxs-lookup"><span data-stu-id="76b9f-127">Type</span></span> | <span data-ttu-id="76b9f-128">説明</span><span class="sxs-lookup"><span data-stu-id="76b9f-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="76b9f-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="76b9f-129">Authorization</span></span>  | <span data-ttu-id="76b9f-130">string</span><span class="sxs-lookup"><span data-stu-id="76b9f-130">string</span></span>  | <span data-ttu-id="76b9f-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="76b9f-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="76b9f-133">要求本文</span><span class="sxs-lookup"><span data-stu-id="76b9f-133">Request body</span></span>
<span data-ttu-id="76b9f-134">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="76b9f-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="76b9f-135">応答</span><span class="sxs-lookup"><span data-stu-id="76b9f-135">Response</span></span>
<span data-ttu-id="76b9f-136">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [group](../resources/group.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="76b9f-136">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76b9f-137">例</span><span class="sxs-lookup"><span data-stu-id="76b9f-137">Example</span></span>
#### <a name="request"></a><span data-ttu-id="76b9f-138">要求</span><span class="sxs-lookup"><span data-stu-id="76b9f-138">Request</span></span>
<span data-ttu-id="76b9f-139">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="76b9f-139">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groups"
}-->
```http
GET https://graph.microsoft.com/beta/groups
```

#### <a name="response"></a><span data-ttu-id="76b9f-140">応答</span><span class="sxs-lookup"><span data-stu-id="76b9f-140">Response</span></span>
<span data-ttu-id="76b9f-141">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="76b9f-141">The following is an example of the response.</span></span>
><span data-ttu-id="76b9f-142">**注:** ここに示す応答オブジェクトは、読みやすさの短縮される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="76b9f-142">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="76b9f-143">実際の呼び出しでは [既定のプロパティ](../api/group-get.md#default-properties)が返されます。</span><span class="sxs-lookup"><span data-stu-id="76b9f-143">The [default properties](../api/group-get.md#default-properties) will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx

 {
  "value": [
    {
      "id": "id-value",
      "description": "description-value",
      "displayName": "displayName-value",
      "groupTypes": [
        "groupTypes-value"
      ],
      "mail": "mail-value",
      "mailEnabled": true,
      "mailNickname": "mailNickname-value",
      "onPremisesLastSyncDateTime": "onPremisesLastSyncDateTime-value",
      "onPremisesSecurityIdentifier": "onPremisesSecurityIdentifier-value",
      "onPremisesSyncEnabled": true,
      "proxyAddresses": [
        "proxyAddresses-value"
      ],
      "securityEnabled": true,
      "visibility": "visibility-value"
    }
  ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
