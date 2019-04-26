---
title: 音声ルーティング グループを更新する
description: audioRoutingGroup のソースとレシーバーを変更します。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: f38105ebb6df2ecd72b6f48051a1409efddc3c5c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322580"
---
# <a name="update-audio-routing-group"></a><span data-ttu-id="a7e0f-103">音声ルーティング グループを更新する</span><span class="sxs-lookup"><span data-stu-id="a7e0f-103">Update audio routing group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a7e0f-104">[audioRoutingGroup](../resources/audioroutinggroup.md)のソースとレシーバーを変更します。</span><span class="sxs-lookup"><span data-stu-id="a7e0f-104">Modify sources and receivers of an [audioRoutingGroup](../resources/audioroutinggroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a7e0f-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a7e0f-105">Permissions</span></span>
<span data-ttu-id="a7e0f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a7e0f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a7e0f-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a7e0f-108">Permission type</span></span> | <span data-ttu-id="a7e0f-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a7e0f-109">Permissions (from least to most privileged)</span></span>                |
| :-------------- | :--------------------------------------------------------- |
| <span data-ttu-id="a7e0f-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a7e0f-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="a7e0f-111">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="a7e0f-111">Not Supported</span></span>                       |
| <span data-ttu-id="a7e0f-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a7e0f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a7e0f-113">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="a7e0f-113">Not Supported</span></span>                       |
| <span data-ttu-id="a7e0f-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a7e0f-114">Application</span></span>     | <span data-ttu-id="a7e0f-115">joingroupcalls を呼び出します。すべて、initiategroupcalls を呼び出します。</span><span class="sxs-lookup"><span data-stu-id="a7e0f-115">Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a7e0f-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a7e0f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /app/calls/{id}/audioRoutingGroups/{id}
PATCH /applications/{id}/calls/{id}/audioRoutingGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a7e0f-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a7e0f-117">Request headers</span></span>
| <span data-ttu-id="a7e0f-118">名前</span><span class="sxs-lookup"><span data-stu-id="a7e0f-118">Name</span></span>          | <span data-ttu-id="a7e0f-119">説明</span><span class="sxs-lookup"><span data-stu-id="a7e0f-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="a7e0f-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="a7e0f-120">Authorization</span></span> | <span data-ttu-id="a7e0f-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a7e0f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a7e0f-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="a7e0f-123">Request body</span></span>
<span data-ttu-id="a7e0f-124">要求本文で、更新する関連フィールドの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="a7e0f-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="a7e0f-125">要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。</span><span class="sxs-lookup"><span data-stu-id="a7e0f-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="a7e0f-126">最適なパフォーマンスを得るために、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="a7e0f-126">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a7e0f-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a7e0f-127">Property</span></span>       | <span data-ttu-id="a7e0f-128">型</span><span class="sxs-lookup"><span data-stu-id="a7e0f-128">Type</span></span>    |<span data-ttu-id="a7e0f-129">説明</span><span class="sxs-lookup"><span data-stu-id="a7e0f-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a7e0f-130">配信</span><span class="sxs-lookup"><span data-stu-id="a7e0f-130">receivers</span></span> | <span data-ttu-id="a7e0f-131">String collection</span><span class="sxs-lookup"><span data-stu-id="a7e0f-131">String collection</span></span> | <span data-ttu-id="a7e0f-132">audioRoutingGroup の対象となる参加者。</span><span class="sxs-lookup"><span data-stu-id="a7e0f-132">The target participants in the audioRoutingGroup.</span></span> |
| <span data-ttu-id="a7e0f-133">routingmode</span><span class="sxs-lookup"><span data-stu-id="a7e0f-133">routingMode</span></span> | <span data-ttu-id="a7e0f-134">String</span><span class="sxs-lookup"><span data-stu-id="a7e0f-134">String</span></span> | <span data-ttu-id="a7e0f-135">使用可能な値は、`oneToOne`、`multicast` です。</span><span class="sxs-lookup"><span data-stu-id="a7e0f-135">Possible values are: `oneToOne`, `multicast`.</span></span> |
| <span data-ttu-id="a7e0f-136">sources</span><span class="sxs-lookup"><span data-stu-id="a7e0f-136">sources</span></span> | <span data-ttu-id="a7e0f-137">String collection</span><span class="sxs-lookup"><span data-stu-id="a7e0f-137">String collection</span></span> | <span data-ttu-id="a7e0f-138">audioRoutingGroup のソース参加者。</span><span class="sxs-lookup"><span data-stu-id="a7e0f-138">The source participant in the audioRoutingGroup.</span></span> |

## <a name="response"></a><span data-ttu-id="a7e0f-139">応答</span><span class="sxs-lookup"><span data-stu-id="a7e0f-139">Response</span></span>
<span data-ttu-id="a7e0f-140">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[audioRoutingGroup](../resources/audioroutinggroup.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a7e0f-140">If successful, this method returns a `200 OK` response code and an updated [audioRoutingGroup](../resources/audioroutinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7e0f-141">例</span><span class="sxs-lookup"><span data-stu-id="a7e0f-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a7e0f-142">要求</span><span class="sxs-lookup"><span data-stu-id="a7e0f-142">Request</span></span>
<span data-ttu-id="a7e0f-143">次の例は要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="a7e0f-143">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update-audioRoutingGroup"
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
##### <a name="response"></a><span data-ttu-id="a7e0f-144">応答</span><span class="sxs-lookup"><span data-stu-id="a7e0f-144">Response</span></span>

> <span data-ttu-id="a7e0f-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="a7e0f-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "Update audioRoutingGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
