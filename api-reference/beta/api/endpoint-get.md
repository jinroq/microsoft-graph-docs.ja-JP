---
title: エンドポイントを取得します。
description: プロパティと、特定のエンドポイント オブジェクトの関係を取得します。
localization_priority: Normal
ms.openlocfilehash: 77ad5716e8e30a16f95bf62593a6530d5e759861
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820448"
---
# <a name="get-endpoint"></a><span data-ttu-id="3b934-103">エンドポイントを取得します。</span><span class="sxs-lookup"><span data-stu-id="3b934-103">Get endpoint</span></span>

> <span data-ttu-id="3b934-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3b934-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3b934-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3b934-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3b934-106">プロパティと、特定の[エンドポイント](../resources/endpoint.md)オブジェクトの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="3b934-106">Retrieve the properties and relationships of a specific [endpoint](../resources/endpoint.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3b934-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3b934-107">Permissions</span></span>
<span data-ttu-id="3b934-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3b934-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="3b934-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3b934-110">Permission type</span></span>      | <span data-ttu-id="3b934-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3b934-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3b934-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3b934-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3b934-113">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b934-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3b934-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3b934-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3b934-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3b934-115">Not supported.</span></span>    |
|<span data-ttu-id="3b934-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3b934-116">Application</span></span> | <span data-ttu-id="3b934-117">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b934-117">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3b934-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3b934-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/endpoints/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3b934-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="3b934-119">Optional query parameters</span></span>
<span data-ttu-id="3b934-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="3b934-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3b934-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3b934-121">Request headers</span></span>
| <span data-ttu-id="3b934-122">名前</span><span class="sxs-lookup"><span data-stu-id="3b934-122">Name</span></span>      |<span data-ttu-id="3b934-123">説明</span><span class="sxs-lookup"><span data-stu-id="3b934-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3b934-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="3b934-124">Authorization</span></span>  | <span data-ttu-id="3b934-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3b934-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="3b934-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3b934-127">Content-Type</span></span>   | <span data-ttu-id="3b934-128">アプリケーションまたは Json</span><span class="sxs-lookup"><span data-stu-id="3b934-128">Application/Json</span></span> |

## <a name="request-body"></a><span data-ttu-id="3b934-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="3b934-129">Request body</span></span>
<span data-ttu-id="3b934-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="3b934-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3b934-131">応答</span><span class="sxs-lookup"><span data-stu-id="3b934-131">Response</span></span>

<span data-ttu-id="3b934-132">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文の[エンドポイント](../resources/endpoint.md)オブジェクト。</span><span class="sxs-lookup"><span data-stu-id="3b934-132">If successful, this method returns a `200 OK` response code and [Endpoint](../resources/endpoint.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3b934-133">例</span><span class="sxs-lookup"><span data-stu-id="3b934-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3b934-134">要求</span><span class="sxs-lookup"><span data-stu-id="3b934-134">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_endpoint"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/endpoints/{id}
```
##### <a name="response"></a><span data-ttu-id="3b934-135">応答</span><span class="sxs-lookup"><span data-stu-id="3b934-135">Response</span></span>
<span data-ttu-id="3b934-p104">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3b934-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.Endpoint"
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
<!-- {
  "type": "#page.annotation",
  "description": "Get Endpoint",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
