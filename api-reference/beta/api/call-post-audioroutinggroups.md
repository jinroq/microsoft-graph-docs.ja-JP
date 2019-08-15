---
title: 音声ルーティング グループを作成する
description: 新しい**audioRoutingGroup**を作成します。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: d552cbec4a2f38b7730aa56499567a54fedde760
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36418909"
---
# <a name="create-audio-routing-group"></a><span data-ttu-id="19fa1-103">音声ルーティング グループを作成する</span><span class="sxs-lookup"><span data-stu-id="19fa1-103">Create audio routing group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="19fa1-104">新しい**audioRoutingGroup**を作成します。</span><span class="sxs-lookup"><span data-stu-id="19fa1-104">Create a new **audioRoutingGroup**.</span></span>

## <a name="permissions"></a><span data-ttu-id="19fa1-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="19fa1-105">Permissions</span></span>
<span data-ttu-id="19fa1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="19fa1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="19fa1-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="19fa1-108">Permission type</span></span>                        | <span data-ttu-id="19fa1-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="19fa1-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="19fa1-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="19fa1-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="19fa1-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="19fa1-111">Not supported.</span></span>                               |
| <span data-ttu-id="19fa1-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="19fa1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19fa1-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="19fa1-113">Not supported.</span></span>                               |
| <span data-ttu-id="19fa1-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="19fa1-114">Application</span></span>                            | <span data-ttu-id="19fa1-115">JoinGroupCalls を呼び出します。すべて、InitiateGroupCalls を呼び出します。</span><span class="sxs-lookup"><span data-stu-id="19fa1-115">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="19fa1-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="19fa1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/audioRoutingGroups
POST /applications/{id}/calls/{id}/audioRoutingGroups
```

## <a name="request-headers"></a><span data-ttu-id="19fa1-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="19fa1-117">Request headers</span></span>
| <span data-ttu-id="19fa1-118">名前</span><span class="sxs-lookup"><span data-stu-id="19fa1-118">Name</span></span>          | <span data-ttu-id="19fa1-119">説明</span><span class="sxs-lookup"><span data-stu-id="19fa1-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="19fa1-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="19fa1-120">Authorization</span></span> | <span data-ttu-id="19fa1-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="19fa1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="19fa1-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="19fa1-123">Request body</span></span>
<span data-ttu-id="19fa1-124">要求本文で、 [audioRoutingGroup](../resources/audioroutinggroup.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="19fa1-124">In the request body, supply a JSON representation of [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="19fa1-125">応答</span><span class="sxs-lookup"><span data-stu-id="19fa1-125">Response</span></span>
<span data-ttu-id="19fa1-126">成功した場合、この`200 OK`メソッドは応答コードと、応答本文で[audioRoutingGroup](../resources/audioroutinggroup.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="19fa1-126">If successful, this method returns `200 OK` response code and [audioRoutingGroup](../resources/audioroutinggroup.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="19fa1-127">例</span><span class="sxs-lookup"><span data-stu-id="19fa1-127">Examples</span></span>

### <a name="example-1-one-to-one-audio-routing-group"></a><span data-ttu-id="19fa1-128">例 1: 1 対1の音声ルーティンググループ</span><span class="sxs-lookup"><span data-stu-id="19fa1-128">Example 1: One-to-one audio routing group</span></span>

##### <a name="request"></a><span data-ttu-id="19fa1-129">要求</span><span class="sxs-lookup"><span data-stu-id="19fa1-129">Request</span></span>
<span data-ttu-id="19fa1-130">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="19fa1-130">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="19fa1-131">プロトコル</span><span class="sxs-lookup"><span data-stu-id="19fa1-131">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="19fa1-132">C#</span><span class="sxs-lookup"><span data-stu-id="19fa1-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-audioroutinggroup-from-call-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="19fa1-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="19fa1-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-audioroutinggroup-from-call-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="19fa1-134">目的-C</span><span class="sxs-lookup"><span data-stu-id="19fa1-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-audioroutinggroup-from-call-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="19fa1-135">要求本文で、 [audioRoutingGroup](../resources/audioroutinggroup.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="19fa1-135">In the request body, supply a JSON representation of [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="19fa1-136">応答</span><span class="sxs-lookup"><span data-stu-id="19fa1-136">Response</span></span>

> <span data-ttu-id="19fa1-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="19fa1-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
### <a name="example-2-multicast-audioroutinggroup"></a><span data-ttu-id="19fa1-139">例 2: マルチキャスト audioRoutingGroup</span><span class="sxs-lookup"><span data-stu-id="19fa1-139">Example 2: Multicast audioRoutingGroup</span></span>

##### <a name="request"></a><span data-ttu-id="19fa1-140">要求</span><span class="sxs-lookup"><span data-stu-id="19fa1-140">Request</span></span>
<span data-ttu-id="19fa1-141">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="19fa1-141">The following example shows the request.</span></span>

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

<span data-ttu-id="19fa1-142">要求本文で、 [audioRoutingGroup](../resources/audioroutinggroup.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="19fa1-142">In the request body, supply a JSON representation of [audioRoutingGroup](../resources/audioroutinggroup.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="19fa1-143">応答</span><span class="sxs-lookup"><span data-stu-id="19fa1-143">Response</span></span>

> <span data-ttu-id="19fa1-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="19fa1-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Create audioRoutingGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
