---
title: chatThread リソース型
description: ChatThread は、Microsoft Teams における chatMessages のコレクションです。
localization_priority: Priority
ms.openlocfilehash: 19365109c2008d52d3597b3d23fc1baefa5cfd1c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399606"
---
# <a name="chatthread-resource-type"></a><span data-ttu-id="4dcb4-103">chatThread リソース型</span><span class="sxs-lookup"><span data-stu-id="4dcb4-103">chatThread resource type</span></span>

> <span data-ttu-id="4dcb4-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4dcb4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4dcb4-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4dcb4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4dcb4-106">ChatThread は、Microsoft Teams における [chatMessages](chatmessage.md) のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="4dcb4-106">A chatThread is a collection of [chatMessages](chatmessage.md) in Microsoft Teams.</span></span>

> <span data-ttu-id="4dcb4-107">現在のところ、ChatThreads は[チャネル内で作成](../api/channel-post-chatthreads.md)できます。</span><span class="sxs-lookup"><span data-stu-id="4dcb4-107">Currently, chatThreads can be [created in channels](../api/channel-post-chatthreads.md).</span></span>  <span data-ttu-id="4dcb4-108">API の今後のリリースでは、既存の chatThreads の読み取りに加えて、チームやチャネルの範囲外のユーザー間での直接チャットの読み取り/書き込みをサポートします。</span><span class="sxs-lookup"><span data-stu-id="4dcb4-108">Future API releases will support reading existing chatThreads, as well as reading/writing direct chats between users that are outside the scope of a team or channel.</span></span>

## <a name="methods"></a><span data-ttu-id="4dcb4-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="4dcb4-109">Methods</span></span>

| <span data-ttu-id="4dcb4-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="4dcb4-110">Method</span></span>       | <span data-ttu-id="4dcb4-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="4dcb4-111">Return Type</span></span>  |<span data-ttu-id="4dcb4-112">説明</span><span class="sxs-lookup"><span data-stu-id="4dcb4-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4dcb4-113">Create thread</span><span class="sxs-lookup"><span data-stu-id="4dcb4-113">Create thread</span></span>](../api/channel-post-chatthreads.md) | [<span data-ttu-id="4dcb4-114">chatThread</span><span class="sxs-lookup"><span data-stu-id="4dcb4-114">chatThread</span></span>](chatthread.md) |<span data-ttu-id="4dcb4-115">最初のメッセージを指定して、指定したチャネルで新しいスレッドを開始します。</span><span class="sxs-lookup"><span data-stu-id="4dcb4-115">Start a new thread in the specified channel, providing the first message.</span></span>|

## <a name="properties"></a><span data-ttu-id="4dcb4-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4dcb4-116">Properties</span></span>
| <span data-ttu-id="4dcb4-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4dcb4-117">Property</span></span>     | <span data-ttu-id="4dcb4-118">型</span><span class="sxs-lookup"><span data-stu-id="4dcb4-118">Type</span></span>   |<span data-ttu-id="4dcb4-119">説明</span><span class="sxs-lookup"><span data-stu-id="4dcb4-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4dcb4-120">id</span><span class="sxs-lookup"><span data-stu-id="4dcb4-120">id</span></span>|<span data-ttu-id="4dcb4-121">String</span><span class="sxs-lookup"><span data-stu-id="4dcb4-121">String</span></span>| <span data-ttu-id="4dcb4-122">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4dcb4-122">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4dcb4-123">関係</span><span class="sxs-lookup"><span data-stu-id="4dcb4-123">Relationships</span></span>
| <span data-ttu-id="4dcb4-124">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4dcb4-124">Relationship</span></span> | <span data-ttu-id="4dcb4-125">型</span><span class="sxs-lookup"><span data-stu-id="4dcb4-125">Type</span></span>   |<span data-ttu-id="4dcb4-126">説明</span><span class="sxs-lookup"><span data-stu-id="4dcb4-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4dcb4-127">rootMessage</span><span class="sxs-lookup"><span data-stu-id="4dcb4-127">rootMessage</span></span>|[<span data-ttu-id="4dcb4-128">chatMessage</span><span class="sxs-lookup"><span data-stu-id="4dcb4-128">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="4dcb4-129">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="4dcb4-129">Nullable.</span></span>|
|<span data-ttu-id="4dcb4-130">chatMessages</span><span class="sxs-lookup"><span data-stu-id="4dcb4-130">chatMessages</span></span>|<span data-ttu-id="4dcb4-131">[chatMessage](chatmessage.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4dcb4-131">[chatMessage](chatmessage.md) collection</span></span>| <span data-ttu-id="4dcb4-132">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="4dcb4-132">Nullable.</span></span>|

> <span data-ttu-id="4dcb4-133">現在、これらの関係は暗黙的に存在しますが、読み取り/書き込みはできません。</span><span class="sxs-lookup"><span data-stu-id="4dcb4-133">Currently these relationships exist implicitly, but cannot read or written.</span></span>  <span data-ttu-id="4dcb4-134">将来的に、ベータ版の API リリースでこの機能がサポートされます。</span><span class="sxs-lookup"><span data-stu-id="4dcb4-134">Future beta API releases will support this.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4dcb4-135">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4dcb4-135">JSON representation</span></span>

<span data-ttu-id="4dcb4-136">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="4dcb4-136">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "posts"
  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatThread"
}-->

```json
{
  "id": "string (identifier)"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chatThread resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
