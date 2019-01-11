---
title: グループの一覧表示
description: Office 365 のグループを含み、それに限定されない組織で使用可能なすべてのグループを一覧表示します。
localization_priority: Priority
ms.openlocfilehash: 1122685cfbd4f1a1f2ff0ca3367e913c983866a0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867719"
---
# <a name="list-groups"></a><span data-ttu-id="acc9f-103">グループを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="acc9f-103">List groups</span></span>
<span data-ttu-id="acc9f-p101">Office 365 のグループを含み、それに限定されない組織で使用可能なすべてのグループを一覧表示します。各グループの[既定のプロパティ](../api/group-get.md#default-properties)が返されます。</span><span class="sxs-lookup"><span data-stu-id="acc9f-p101">List all the groups available in an organization, including but not limited to Office 365 Groups. The [default properties](../api/group-get.md#default-properties) of each group are returned.</span></span>

<span data-ttu-id="acc9f-106">Office 365 グループ (別名統合グループ) のみを一覧表示するには、**groupTypes** にフィルターを適用します。</span><span class="sxs-lookup"><span data-stu-id="acc9f-106">To list only Office 365 Groups (aka unified groups), apply a filter on **groupTypes**:</span></span>
```
GET https://graph.microsoft.com/v1.0/groups?$filter=groupTypes/any(c:c+eq+'Unified')
```

<span data-ttu-id="acc9f-107">OData クエリ オプション `$orderby` を使用して、以下の例のように、組織内のグループを **displayName** 値で並べ替えることができます。</span><span class="sxs-lookup"><span data-stu-id="acc9f-107">You can use the OData query option `$orderby` to sort groups in an organization by the **displayName** values, as shown in the following example:</span></span>
```
GET https://graph.microsoft.com/v1.0/groups?$orderby=displayName
```

## <a name="permissions"></a><span data-ttu-id="acc9f-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="acc9f-108">Permissions</span></span>
<span data-ttu-id="acc9f-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="acc9f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="acc9f-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="acc9f-111">Permission type</span></span>      | <span data-ttu-id="acc9f-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="acc9f-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="acc9f-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="acc9f-113">Delegated (work or school account)</span></span> | <span data-ttu-id="acc9f-114">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="acc9f-114">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="acc9f-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="acc9f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="acc9f-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="acc9f-116">Not supported.</span></span>    |
|<span data-ttu-id="acc9f-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="acc9f-117">Application</span></span> | <span data-ttu-id="acc9f-118">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="acc9f-118">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="acc9f-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="acc9f-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="acc9f-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="acc9f-120">Optional query parameters</span></span>
<span data-ttu-id="acc9f-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="acc9f-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="acc9f-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="acc9f-122">Request headers</span></span>
| <span data-ttu-id="acc9f-123">名前</span><span class="sxs-lookup"><span data-stu-id="acc9f-123">Name</span></span>       | <span data-ttu-id="acc9f-124">種類</span><span class="sxs-lookup"><span data-stu-id="acc9f-124">Type</span></span> | <span data-ttu-id="acc9f-125">説明</span><span class="sxs-lookup"><span data-stu-id="acc9f-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="acc9f-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="acc9f-126">Authorization</span></span>  | <span data-ttu-id="acc9f-127">string</span><span class="sxs-lookup"><span data-stu-id="acc9f-127">string</span></span>  | <span data-ttu-id="acc9f-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="acc9f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="acc9f-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="acc9f-130">Request body</span></span>
<span data-ttu-id="acc9f-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="acc9f-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="acc9f-132">応答</span><span class="sxs-lookup"><span data-stu-id="acc9f-132">Response</span></span>
<span data-ttu-id="acc9f-133">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [group](../resources/group.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="acc9f-133">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="acc9f-134">例</span><span class="sxs-lookup"><span data-stu-id="acc9f-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="acc9f-135">要求</span><span class="sxs-lookup"><span data-stu-id="acc9f-135">Request</span></span>
<span data-ttu-id="acc9f-136">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="acc9f-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groups"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups
```

#### <a name="response"></a><span data-ttu-id="acc9f-137">応答</span><span class="sxs-lookup"><span data-stu-id="acc9f-137">Response</span></span>
<span data-ttu-id="acc9f-138">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="acc9f-138">The following is an example of the response.</span></span>

><span data-ttu-id="acc9f-139">**注:** ここに示す応答オブジェクトは、読みやすさの短縮される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="acc9f-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="acc9f-140">実際の呼び出しでは [既定のプロパティ](../api/group-get.md#default-properties)が返されます。</span><span class="sxs-lookup"><span data-stu-id="acc9f-140">The [default properties](../api/group-get.md#default-properties) will be returned from an actual call.</span></span>

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
