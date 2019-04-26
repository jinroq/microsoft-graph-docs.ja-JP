---
title: 音声ルーティング グループを取得する
description: audioRoutingGroup オブジェクトのプロパティとリレーションシップを取得します。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 0f9d3d76a07bfae88f53181ff04c3fab3ee6d220
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322565"
---
# <a name="get-audio-routing-group"></a><span data-ttu-id="627c8-103">音声ルーティング グループを取得する</span><span class="sxs-lookup"><span data-stu-id="627c8-103">Get audio routing group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="627c8-104">[audioRoutingGroup](../resources/audioroutinggroup.md)オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="627c8-104">Retrieve the properties and relationships of an [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="627c8-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="627c8-105">Permissions</span></span>
<span data-ttu-id="627c8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="627c8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="627c8-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="627c8-108">Permission type</span></span>                        | <span data-ttu-id="627c8-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="627c8-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="627c8-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="627c8-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="627c8-111">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="627c8-111">Not Supported</span></span>                               |
| <span data-ttu-id="627c8-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="627c8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="627c8-113">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="627c8-113">Not Supported</span></span>                               |
| <span data-ttu-id="627c8-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="627c8-114">Application</span></span>                            | <span data-ttu-id="627c8-115">joingroupcalls を呼び出します。すべて、initiategroupcalls を呼び出します。</span><span class="sxs-lookup"><span data-stu-id="627c8-115">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="627c8-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="627c8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}/audioRoutingGroups/{id}
GET /applications/{id}/calls/{id}/audioRoutingGroups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="627c8-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="627c8-117">Optional query parameters</span></span>
<span data-ttu-id="627c8-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="627c8-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="627c8-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="627c8-119">Request headers</span></span>
| <span data-ttu-id="627c8-120">名前</span><span class="sxs-lookup"><span data-stu-id="627c8-120">Name</span></span>          | <span data-ttu-id="627c8-121">説明</span><span class="sxs-lookup"><span data-stu-id="627c8-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="627c8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="627c8-122">Authorization</span></span> | <span data-ttu-id="627c8-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="627c8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="627c8-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="627c8-125">Request body</span></span>
<span data-ttu-id="627c8-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="627c8-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="627c8-127">応答</span><span class="sxs-lookup"><span data-stu-id="627c8-127">Response</span></span>
<span data-ttu-id="627c8-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[audioRoutingGroup](../resources/audioroutinggroup.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="627c8-128">If successful, this method returns a `200 OK` response code and an [audioRoutingGroup](../resources/audioroutinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="627c8-129">例</span><span class="sxs-lookup"><span data-stu-id="627c8-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="627c8-130">要求</span><span class="sxs-lookup"><span data-stu-id="627c8-130">Request</span></span>
<span data-ttu-id="627c8-131">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="627c8-131">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get-audioRoutingGroup"
}-->
```http
GET https://graph.microsoft.com/beta/app/calls/{id}/audioRoutingGroups/{id}
```

##### <a name="response"></a><span data-ttu-id="627c8-132">応答</span><span class="sxs-lookup"><span data-stu-id="627c8-132">Response</span></span>

> <span data-ttu-id="627c8-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="627c8-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Get audioRoutingGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
