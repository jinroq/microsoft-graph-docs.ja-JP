---
title: オーディオのルーティング グループを作成します。
description: 新しい**audioRoutingGroup**を作成します。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: fe623a581233324e13c949d16570b1396fdd663c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966385"
---
# <a name="create-audio-routing-group"></a><span data-ttu-id="b2ffa-103">オーディオのルーティング グループを作成します。</span><span class="sxs-lookup"><span data-stu-id="b2ffa-103">Create audio routing group</span></span>

> <span data-ttu-id="b2ffa-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b2ffa-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b2ffa-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b2ffa-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b2ffa-106">新しい**audioRoutingGroup**を作成します。</span><span class="sxs-lookup"><span data-stu-id="b2ffa-106">Create a new **audioRoutingGroup**.</span></span>

## <a name="permissions"></a><span data-ttu-id="b2ffa-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b2ffa-107">Permissions</span></span>
<span data-ttu-id="b2ffa-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b2ffa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b2ffa-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b2ffa-110">Permission type</span></span>                        | <span data-ttu-id="b2ffa-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b2ffa-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b2ffa-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b2ffa-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="b2ffa-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b2ffa-113">Not supported.</span></span>                               |
| <span data-ttu-id="b2ffa-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b2ffa-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b2ffa-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b2ffa-115">Not supported.</span></span>                               |
| <span data-ttu-id="b2ffa-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b2ffa-116">Application</span></span>                            | <span data-ttu-id="b2ffa-117">Calls.JoinGroupCalls.All、Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="b2ffa-117">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b2ffa-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b2ffa-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/audioRoutingGroups
POST /applications/{id}/calls/{id}/audioRoutingGroups
```

## <a name="request-headers"></a><span data-ttu-id="b2ffa-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b2ffa-119">Request headers</span></span>
| <span data-ttu-id="b2ffa-120">名前</span><span class="sxs-lookup"><span data-stu-id="b2ffa-120">Name</span></span>          | <span data-ttu-id="b2ffa-121">説明</span><span class="sxs-lookup"><span data-stu-id="b2ffa-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="b2ffa-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b2ffa-122">Authorization</span></span> | <span data-ttu-id="b2ffa-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b2ffa-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b2ffa-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="b2ffa-125">Request body</span></span>
<span data-ttu-id="b2ffa-126">要求の本文には、 [audioRoutingGroup](../resources/audioroutinggroup.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="b2ffa-126">In the request body, supply a JSON representation of [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="b2ffa-127">応答</span><span class="sxs-lookup"><span data-stu-id="b2ffa-127">Response</span></span>
<span data-ttu-id="b2ffa-128">かどうかは成功すると、このメソッドを返します`200 OK`、応答の本体で応答コードと[audioRoutingGroup](../resources/audioroutinggroup.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="b2ffa-128">If successful, this method returns `200 OK` response code and [audioRoutingGroup](../resources/audioroutinggroup.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b2ffa-129">例</span><span class="sxs-lookup"><span data-stu-id="b2ffa-129">Examples</span></span>

### <a name="example-1-one-to-one-audio-routing-group"></a><span data-ttu-id="b2ffa-130">例 1: 1 対 1 のオーディオ ルーティング グループ</span><span class="sxs-lookup"><span data-stu-id="b2ffa-130">Example 1: One-to-one audio routing group</span></span>

##### <a name="request"></a><span data-ttu-id="b2ffa-131">要求</span><span class="sxs-lookup"><span data-stu-id="b2ffa-131">Request</span></span>
<span data-ttu-id="b2ffa-132">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="b2ffa-132">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create-audioRoutingGroup-from-call"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/audioRoutingGroups
Content-Type: application/json
Content-Length: 233

{
  "id": "oneToOne",
  "routingMode": "oneToOne",
  "sources": [
    "632899f8-2ea1-4604-8413-27bd2892079f"
  ],
  "receivers": [
    "550fae72-d251-43ec-868c-373732c2704f"
  ]
}
```

<span data-ttu-id="b2ffa-133">要求の本文には、 [audioRoutingGroup](../resources/audioroutinggroup.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="b2ffa-133">In the request body, supply a JSON representation of [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="b2ffa-134">応答</span><span class="sxs-lookup"><span data-stu-id="b2ffa-134">Response</span></span>

> <span data-ttu-id="b2ffa-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="b2ffa-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "550fae72-d251-43ec-868c-373732c2704f"
  ]
}
```
### <a name="example-2-multicast-audioroutinggroup"></a><span data-ttu-id="b2ffa-137">例 2: マルチキャスト audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="b2ffa-137">Example 2: Multicast audioRoutingGroup</span></span>

##### <a name="request"></a><span data-ttu-id="b2ffa-138">要求</span><span class="sxs-lookup"><span data-stu-id="b2ffa-138">Request</span></span>
<span data-ttu-id="b2ffa-139">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="b2ffa-139">The following example shows the request.</span></span>

```http
POST https://graph.microsoft.com/beta/app/calls/{id}/audioRoutingGroups
Content-Type: application/json
Content-Length: 233
```

<!-- {
  "blockType": "example",
  "name": "create-audioRoutingGroup-from-call",
  "@odata.type": "microsoft.graph.audioRoutingGroup"
}-->

```json
{
  "id": "multicast",
  "routingMode": "multicast",
  "sources": [
    "632899f8-2ea1-4604-8413-27bd2892079f"
  ],
  "receivers": [
    "550fae72-d251-43ec-868c-373732c2704f",
    "72f988bf-86f1-41af-91ab-2d7cd011db47"
  ]
}
```

<span data-ttu-id="b2ffa-140">要求の本文には、 [audioRoutingGroup](../resources/audioroutinggroup.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="b2ffa-140">In the request body, supply a JSON representation of [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="b2ffa-141">応答</span><span class="sxs-lookup"><span data-stu-id="b2ffa-141">Response</span></span>

> <span data-ttu-id="b2ffa-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="b2ffa-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 233
```
<!-- {
  "blockType": "example",
  "truncated": true,
  "@odata.type": "microsoft.graph.audioRoutingGroup"
} -->

```json
{
  "id": "multicast",
  "routingMode": "multicast",
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
  "description": "Create audioRoutingGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
