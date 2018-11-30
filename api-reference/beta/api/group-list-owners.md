---
title: 所有者を一覧表示する
description: グループの所有者の一覧を取得します。所有者は、グループ オブジェクトの変更を許可されている管理者以外のユーザーです。
ms.openlocfilehash: 2b3584e5037c9ac36ac4bff97ef64af21643eb31
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073749"
---
# <a name="list-owners"></a><span data-ttu-id="383be-104">所有者を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="383be-104">List owners</span></span>

> <span data-ttu-id="383be-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="383be-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="383be-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="383be-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="383be-p103">グループの所有者の一覧を取得します。所有者は、グループ オブジェクトの変更を許可されている管理者以外のユーザーです。</span><span class="sxs-lookup"><span data-stu-id="383be-p103">Retrieve a list of the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span>

## <a name="permissions"></a><span data-ttu-id="383be-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="383be-109">Permissions</span></span>
<span data-ttu-id="383be-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="383be-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="383be-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="383be-112">Permission type</span></span>      | <span data-ttu-id="383be-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="383be-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="383be-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="383be-114">Delegated (work or school account)</span></span> | <span data-ttu-id="383be-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="383be-115">Not supported.</span></span>    |
|<span data-ttu-id="383be-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="383be-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="383be-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="383be-117">Not supported.</span></span>    |
|<span data-ttu-id="383be-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="383be-118">Application</span></span> | <span data-ttu-id="383be-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="383be-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="383be-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="383be-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/owners
```

## <a name="optional-query-parameters"></a><span data-ttu-id="383be-121">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="383be-121">Optional query parameters</span></span>
<span data-ttu-id="383be-122">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="383be-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="383be-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="383be-123">Request headers</span></span>
| <span data-ttu-id="383be-124">名前</span><span class="sxs-lookup"><span data-stu-id="383be-124">Name</span></span>       | <span data-ttu-id="383be-125">型</span><span class="sxs-lookup"><span data-stu-id="383be-125">Type</span></span> | <span data-ttu-id="383be-126">説明</span><span class="sxs-lookup"><span data-stu-id="383be-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="383be-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="383be-127">Authorization</span></span>  | <span data-ttu-id="383be-128">string</span><span class="sxs-lookup"><span data-stu-id="383be-128">string</span></span>  | <span data-ttu-id="383be-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="383be-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="383be-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="383be-131">Request body</span></span>
<span data-ttu-id="383be-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="383be-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="383be-133">応答</span><span class="sxs-lookup"><span data-stu-id="383be-133">Response</span></span>
<span data-ttu-id="383be-134">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="383be-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="383be-135">例</span><span class="sxs-lookup"><span data-stu-id="383be-135">Example</span></span>
#### <a name="request"></a><span data-ttu-id="383be-136">要求</span><span class="sxs-lookup"><span data-stu-id="383be-136">Request</span></span>
<span data-ttu-id="383be-137">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="383be-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/owners
```

#### <a name="response"></a><span data-ttu-id="383be-138">応答</span><span class="sxs-lookup"><span data-stu-id="383be-138">Response</span></span>
<span data-ttu-id="383be-139">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="383be-139">The following is an example of the response.</span></span>
><span data-ttu-id="383be-140">**注:** ここに示す応答オブジェクトは、読みやすさの短縮される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="383be-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="383be-141">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="383be-141">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->