---
title: オーディオのルーティング グループを取得します。
description: プロパティと audioRoutingGroup オブジェクトの関係を取得します。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 810a27c91c5a31a970f7b279d774d12bf049210d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524038"
---
# <a name="get-audio-routing-group"></a><span data-ttu-id="b9a2b-103">オーディオのルーティング グループを取得します。</span><span class="sxs-lookup"><span data-stu-id="b9a2b-103">Get audio routing group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9a2b-104">プロパティと[audioRoutingGroup](../resources/audioroutinggroup.md)オブジェクトの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="b9a2b-104">Retrieve the properties and relationships of an [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b9a2b-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b9a2b-105">Permissions</span></span>
<span data-ttu-id="b9a2b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b9a2b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b9a2b-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b9a2b-108">Permission type</span></span>                        | <span data-ttu-id="b9a2b-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b9a2b-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b9a2b-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b9a2b-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b9a2b-111">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="b9a2b-111">Not Supported</span></span>                               |
| <span data-ttu-id="b9a2b-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b9a2b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9a2b-113">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="b9a2b-113">Not Supported</span></span>                               |
| <span data-ttu-id="b9a2b-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b9a2b-114">Application</span></span>                            | <span data-ttu-id="b9a2b-115">Calls.JoinGroupCalls.All、Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="b9a2b-115">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b9a2b-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b9a2b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}/audioRoutingGroups/{id}
GET /applications/{id}/calls/{id}/audioRoutingGroups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b9a2b-117">省略可能なクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="b9a2b-117">Optional query parameters</span></span>
<span data-ttu-id="b9a2b-118">このメソッドは、応答をカスタマイズするために[OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="b9a2b-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b9a2b-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b9a2b-119">Request headers</span></span>
| <span data-ttu-id="b9a2b-120">名前</span><span class="sxs-lookup"><span data-stu-id="b9a2b-120">Name</span></span>          | <span data-ttu-id="b9a2b-121">説明</span><span class="sxs-lookup"><span data-stu-id="b9a2b-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="b9a2b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9a2b-122">Authorization</span></span> | <span data-ttu-id="b9a2b-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b9a2b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b9a2b-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="b9a2b-125">Request body</span></span>
<span data-ttu-id="b9a2b-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b9a2b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9a2b-127">応答</span><span class="sxs-lookup"><span data-stu-id="b9a2b-127">Response</span></span>
<span data-ttu-id="b9a2b-128">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の[audioRoutingGroup](../resources/audioroutinggroup.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="b9a2b-128">If successful, this method returns a `200 OK` response code and an [audioRoutingGroup](../resources/audioroutinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9a2b-129">例</span><span class="sxs-lookup"><span data-stu-id="b9a2b-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b9a2b-130">要求</span><span class="sxs-lookup"><span data-stu-id="b9a2b-130">Request</span></span>
<span data-ttu-id="b9a2b-131">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="b9a2b-131">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get-audioRoutingGroup"
}-->
```http
GET https://graph.microsoft.com/beta/app/calls/{id}/audioRoutingGroups/{id}
```

##### <a name="response"></a><span data-ttu-id="b9a2b-132">応答</span><span class="sxs-lookup"><span data-stu-id="b9a2b-132">Response</span></span>

> <span data-ttu-id="b9a2b-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="b9a2b-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/api/audioroutinggroup-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
