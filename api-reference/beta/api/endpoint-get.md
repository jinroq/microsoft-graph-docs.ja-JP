---
title: エンドポイントを取得する
description: 特定のエンドポイントオブジェクトのプロパティとリレーションシップを取得します。
localization_priority: Normal
doc_type: apiPageType
author: ''
ms.prod: ''
ms.openlocfilehash: 26cc0d9927cd207e942a6bfd8c386557d61e4b66
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36415814"
---
# <a name="get-endpoint"></a><span data-ttu-id="c3994-103">エンドポイントを取得する</span><span class="sxs-lookup"><span data-stu-id="c3994-103">Get endpoint</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c3994-104">特定の[エンドポイント](../resources/endpoint.md)オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="c3994-104">Retrieve the properties and relationships of a specific [endpoint](../resources/endpoint.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c3994-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c3994-105">Permissions</span></span>
<span data-ttu-id="c3994-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c3994-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c3994-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c3994-108">Permission type</span></span>      | <span data-ttu-id="c3994-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c3994-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c3994-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c3994-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c3994-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3994-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c3994-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c3994-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c3994-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c3994-113">Not supported.</span></span>    |
|<span data-ttu-id="c3994-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c3994-114">Application</span></span> | <span data-ttu-id="c3994-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3994-115">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c3994-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c3994-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/endpoints/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c3994-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="c3994-117">Optional query parameters</span></span>
<span data-ttu-id="c3994-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c3994-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c3994-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c3994-119">Request headers</span></span>
| <span data-ttu-id="c3994-120">名前</span><span class="sxs-lookup"><span data-stu-id="c3994-120">Name</span></span>      |<span data-ttu-id="c3994-121">説明</span><span class="sxs-lookup"><span data-stu-id="c3994-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c3994-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3994-122">Authorization</span></span>  | <span data-ttu-id="c3994-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c3994-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="c3994-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c3994-125">Content-Type</span></span>   | <span data-ttu-id="c3994-126">Application/Json</span><span class="sxs-lookup"><span data-stu-id="c3994-126">Application/Json</span></span> |

## <a name="request-body"></a><span data-ttu-id="c3994-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="c3994-127">Request body</span></span>
<span data-ttu-id="c3994-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c3994-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c3994-129">応答</span><span class="sxs-lookup"><span data-stu-id="c3994-129">Response</span></span>

<span data-ttu-id="c3994-130">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[エンドポイント](../resources/endpoint.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c3994-130">If successful, this method returns a `200 OK` response code and [Endpoint](../resources/endpoint.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c3994-131">例</span><span class="sxs-lookup"><span data-stu-id="c3994-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c3994-132">要求</span><span class="sxs-lookup"><span data-stu-id="c3994-132">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c3994-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="c3994-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_endpoint"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/endpoints/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c3994-134">C#</span><span class="sxs-lookup"><span data-stu-id="c3994-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-endpoint-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c3994-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c3994-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-endpoint-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c3994-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="c3994-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-endpoint-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c3994-137">応答</span><span class="sxs-lookup"><span data-stu-id="c3994-137">Response</span></span>
<span data-ttu-id="c3994-p103">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c3994-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.endpoint"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 208

{
  "capability": "Conversations",
  "providerId": "{Yammer GUID}",
  "providerName": "Yammer",
  "uri": "uri-value",
  "providerResourceId": "Yammer.FeedURL",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get Endpoint",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
