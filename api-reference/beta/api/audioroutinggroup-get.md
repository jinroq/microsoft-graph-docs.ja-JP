---
title: オーディオのルーティング グループを取得します。
description: プロパティと audioRoutingGroup オブジェクトの関係を取得します。
ms.openlocfilehash: 4da3ceb829cf1a2e59fa34c7073fe7f54126a199
ms.sourcegitcommit: 4a46cfd112c8089fc07e4e5ccdccaf415a3a0e7f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/05/2018
ms.locfileid: "27156013"
---
# <a name="get-audio-routing-group"></a><span data-ttu-id="65425-103">オーディオのルーティング グループを取得します。</span><span class="sxs-lookup"><span data-stu-id="65425-103">Get audio routing group</span></span>

> <span data-ttu-id="65425-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="65425-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="65425-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="65425-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="65425-106">プロパティと[audioRoutingGroup](../resources/audioroutinggroup.md)オブジェクトの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="65425-106">Retrieve the properties and relationships of an [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="65425-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="65425-107">Permissions</span></span>
<span data-ttu-id="65425-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="65425-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="65425-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="65425-110">Permission type</span></span>                        | <span data-ttu-id="65425-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="65425-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="65425-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="65425-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="65425-113">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="65425-113">Not Supported</span></span>                               |
| <span data-ttu-id="65425-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="65425-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65425-115">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="65425-115">Not Supported</span></span>                               |
| <span data-ttu-id="65425-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="65425-116">Application</span></span>     | <span data-ttu-id="65425-117">Calls.JoinGroupCalls.All、Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="65425-117">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="65425-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="65425-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}/audioRoutingGroups/{id}
GET /applications/{id}/calls/{id}/audioRoutingGroups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="65425-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="65425-119">Optional query parameters</span></span>
<span data-ttu-id="65425-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="65425-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="65425-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="65425-121">Request headers</span></span>
| <span data-ttu-id="65425-122">名前</span><span class="sxs-lookup"><span data-stu-id="65425-122">Name</span></span>          | <span data-ttu-id="65425-123">説明</span><span class="sxs-lookup"><span data-stu-id="65425-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="65425-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="65425-124">Authorization</span></span> | <span data-ttu-id="65425-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="65425-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="65425-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="65425-127">Request body</span></span>
<span data-ttu-id="65425-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="65425-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="65425-129">応答</span><span class="sxs-lookup"><span data-stu-id="65425-129">Response</span></span>
<span data-ttu-id="65425-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の[audioRoutingGroup](../resources/audioroutinggroup.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="65425-130">If successful, this method returns a `200 OK` response code and an [audioRoutingGroup](../resources/audioroutinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65425-131">例</span><span class="sxs-lookup"><span data-stu-id="65425-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="65425-132">要求</span><span class="sxs-lookup"><span data-stu-id="65425-132">Request</span></span>
<span data-ttu-id="65425-133">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="65425-133">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_audioRoutingGroup"
}-->
```http
GET https://graph.microsoft.com/beta/app/calls/{id}/audioRoutingGroups/{id}
```

##### <a name="response"></a><span data-ttu-id="65425-134">応答</span><span class="sxs-lookup"><span data-stu-id="65425-134">Response</span></span>

> <span data-ttu-id="65425-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="65425-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.audioRoutingGroup"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 233

{
  "id": "oneToOne",
  "routingMode": "oneToOne",
  "sources": [
    "632899f8-2ea1-4604-8413-27bd2892079f"
  ],
  "receivers": [
    "550fae72-d251-43ec-868c-373732c2704f",
    "72f988bf-86f1-41af-91ab-2d7cd011db47"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get audioRoutingGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
