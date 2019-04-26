---
title: エンドポイントを一覧表示する
description: エンドポイントオブジェクトのリストを取得します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: a5e65bdfc2daa39424c3e6f0c90a3717f91d4e0b
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33324329"
---
# <a name="list-endpoints"></a><span data-ttu-id="acda0-103">エンドポイントを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="acda0-103">List endpoints</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="acda0-104">[エンドポイント](../resources/endpoint.md)オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="acda0-104">Retrieve a list of [endpoint](../resources/endpoint.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="acda0-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="acda0-105">Permissions</span></span>
<span data-ttu-id="acda0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="acda0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="acda0-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="acda0-108">Permission type</span></span>      | <span data-ttu-id="acda0-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="acda0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="acda0-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="acda0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="acda0-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="acda0-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="acda0-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="acda0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="acda0-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="acda0-113">Not supported.</span></span>    |
|<span data-ttu-id="acda0-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="acda0-114">Application</span></span> | <span data-ttu-id="acda0-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="acda0-115">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="acda0-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="acda0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/endpoints
```
## <a name="optional-query-parameters"></a><span data-ttu-id="acda0-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="acda0-117">Optional query parameters</span></span>
<span data-ttu-id="acda0-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="acda0-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="acda0-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="acda0-119">Request headers</span></span>
| <span data-ttu-id="acda0-120">名前</span><span class="sxs-lookup"><span data-stu-id="acda0-120">Name</span></span>      |<span data-ttu-id="acda0-121">説明</span><span class="sxs-lookup"><span data-stu-id="acda0-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="acda0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="acda0-122">Authorization</span></span>  | <span data-ttu-id="acda0-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="acda0-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="acda0-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="acda0-125">Content-Type</span></span>   | <span data-ttu-id="acda0-126">Application/Json</span><span class="sxs-lookup"><span data-stu-id="acda0-126">Application/Json</span></span> |

## <a name="request-body"></a><span data-ttu-id="acda0-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="acda0-127">Request body</span></span>
<span data-ttu-id="acda0-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="acda0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="acda0-129">応答</span><span class="sxs-lookup"><span data-stu-id="acda0-129">Response</span></span>

<span data-ttu-id="acda0-130">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[エンドポイント](../resources/endpoint.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="acda0-130">If successful, this method returns a `200 OK` response code and collection of [Endpoint](../resources/endpoint.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="acda0-131">例</span><span class="sxs-lookup"><span data-stu-id="acda0-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="acda0-132">要求</span><span class="sxs-lookup"><span data-stu-id="acda0-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_endpoints"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/endpoints
```
##### <a name="response"></a><span data-ttu-id="acda0-133">応答</span><span class="sxs-lookup"><span data-stu-id="acda0-133">Response</span></span>
<span data-ttu-id="acda0-p103">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="acda0-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.endpoint",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 261

{
  "value": [
    {
      "capability": "Conversations",
      "providerId": "{Yammer GUID}",
      "providerName": "Yammer",
      "uri": "uri-value",
      "providerResourceId": "Yammer.FeedURL",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List endpoints",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
