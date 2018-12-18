---
title: オーディオのルーティング グループを更新します。
description: ソースと、audioRoutingGroup の受信機を変更します。
author: VinodRavichandran
ms.openlocfilehash: ae9e67a9f116a9c1e9dec2b5d742f13917374718
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27336688"
---
# <a name="update-audio-routing-group"></a><span data-ttu-id="d5e2b-103">オーディオのルーティング グループを更新します。</span><span class="sxs-lookup"><span data-stu-id="d5e2b-103">Update audio routing group</span></span>

> <span data-ttu-id="d5e2b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d5e2b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d5e2b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d5e2b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d5e2b-106">ソースと、 [audioRoutingGroup](../resources/audioroutinggroup.md)の受信機を変更します。</span><span class="sxs-lookup"><span data-stu-id="d5e2b-106">Modify sources and receivers of an [audioRoutingGroup](../resources/audioroutinggroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d5e2b-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d5e2b-107">Permissions</span></span>
<span data-ttu-id="d5e2b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d5e2b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d5e2b-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d5e2b-110">Permission type</span></span> | <span data-ttu-id="d5e2b-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d5e2b-111">Permissions (from least to most privileged)</span></span>                |
| :-------------- | :--------------------------------------------------------- |
| <span data-ttu-id="d5e2b-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d5e2b-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="d5e2b-113">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="d5e2b-113">Not Supported</span></span>                       |
| <span data-ttu-id="d5e2b-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d5e2b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5e2b-115">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="d5e2b-115">Not Supported</span></span>                       |
| <span data-ttu-id="d5e2b-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d5e2b-116">Application</span></span>     | <span data-ttu-id="d5e2b-117">Calls.JoinGroupCalls.All、Calls.InitiateGroupCalls.All</span><span class="sxs-lookup"><span data-stu-id="d5e2b-117">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d5e2b-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d5e2b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /app/calls/{id}/audioRoutingGroups/{id}
PATCH /applications/{id}/calls/{id}/audioRoutingGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d5e2b-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d5e2b-119">Request headers</span></span>
| <span data-ttu-id="d5e2b-120">名前</span><span class="sxs-lookup"><span data-stu-id="d5e2b-120">Name</span></span>          | <span data-ttu-id="d5e2b-121">説明</span><span class="sxs-lookup"><span data-stu-id="d5e2b-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="d5e2b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5e2b-122">Authorization</span></span> | <span data-ttu-id="d5e2b-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d5e2b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d5e2b-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="d5e2b-125">Request body</span></span>
<span data-ttu-id="d5e2b-126">要求本文で、更新する関連フィールドの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="d5e2b-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="d5e2b-127">要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変更に基づいて再計算されます。</span><span class="sxs-lookup"><span data-stu-id="d5e2b-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="d5e2b-128">最適なパフォーマンスを得るために、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="d5e2b-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d5e2b-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d5e2b-129">Property</span></span>       | <span data-ttu-id="d5e2b-130">種類</span><span class="sxs-lookup"><span data-stu-id="d5e2b-130">Type</span></span>    |<span data-ttu-id="d5e2b-131">説明</span><span class="sxs-lookup"><span data-stu-id="d5e2b-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d5e2b-132">受信機</span><span class="sxs-lookup"><span data-stu-id="d5e2b-132">receivers</span></span> | <span data-ttu-id="d5e2b-133">String コレクション</span><span class="sxs-lookup"><span data-stu-id="d5e2b-133">String collection</span></span> | <span data-ttu-id="d5e2b-134">ターゲットの参加者、audioRoutingGroup。</span><span class="sxs-lookup"><span data-stu-id="d5e2b-134">The target participants in the audioRoutingGroup.</span></span> |
| <span data-ttu-id="d5e2b-135">routingMode</span><span class="sxs-lookup"><span data-stu-id="d5e2b-135">routingMode</span></span> | <span data-ttu-id="d5e2b-136">String</span><span class="sxs-lookup"><span data-stu-id="d5e2b-136">String</span></span> | <span data-ttu-id="d5e2b-137">使用可能な値は、`oneToOne`、`multicast` です。</span><span class="sxs-lookup"><span data-stu-id="d5e2b-137">Possible values are: `oneToOne`, `multicast`.</span></span> |
| <span data-ttu-id="d5e2b-138">ソース</span><span class="sxs-lookup"><span data-stu-id="d5e2b-138">sources</span></span> | <span data-ttu-id="d5e2b-139">String コレクション</span><span class="sxs-lookup"><span data-stu-id="d5e2b-139">String collection</span></span> | <span data-ttu-id="d5e2b-140">AudioRoutingGroup のソースの構成要素です。</span><span class="sxs-lookup"><span data-stu-id="d5e2b-140">The source participant in the audioRoutingGroup.</span></span> |

## <a name="response"></a><span data-ttu-id="d5e2b-141">応答</span><span class="sxs-lookup"><span data-stu-id="d5e2b-141">Response</span></span>
<span data-ttu-id="d5e2b-142">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[audioRoutingGroup](../resources/audioroutinggroup.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="d5e2b-142">If successful, this method returns a `200 OK` response code and an updated [audioRoutingGroup](../resources/audioroutinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5e2b-143">例</span><span class="sxs-lookup"><span data-stu-id="d5e2b-143">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d5e2b-144">要求</span><span class="sxs-lookup"><span data-stu-id="d5e2b-144">Request</span></span>
<span data-ttu-id="d5e2b-145">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="d5e2b-145">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_audioRoutingGroup"
}-->
```http
PATCH https://graph.microsoft.com/beta/app/calls/{id}/audioRoutingGroups/{id}
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
##### <a name="response"></a><span data-ttu-id="d5e2b-146">応答</span><span class="sxs-lookup"><span data-stu-id="d5e2b-146">Response</span></span>

> <span data-ttu-id="d5e2b-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="d5e2b-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "Update audioRoutingGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
