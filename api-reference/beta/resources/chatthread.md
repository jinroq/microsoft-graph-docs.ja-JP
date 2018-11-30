---
title: chatThread リソースの種類
description: ChatThread は、マイクロソフトのチームでの chatMessages のコレクションです。
ms.openlocfilehash: ef8f118ae4354a5e4197802708aecfa1fb6f8cb8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073300"
---
# <a name="chatthread-resource-type"></a><span data-ttu-id="48626-103">chatThread リソースの種類</span><span class="sxs-lookup"><span data-stu-id="48626-103">chatThread resource type</span></span>

> <span data-ttu-id="48626-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="48626-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="48626-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="48626-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="48626-106">ChatThread は、マイクロソフトのチームでは、 [chatMessages](chatmessage.md)のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="48626-106">A chatThread is a collection of [chatMessages](chatmessage.md) in Microsoft Teams.</span></span>

> <span data-ttu-id="48626-107">現時点では、chatThreads、[チャネルで作成](../api/channel-post-chatthreads.md)します。</span><span class="sxs-lookup"><span data-stu-id="48626-107">Currently, chatThreads can be [created in channels](../api/channel-post-chatthreads.md).</span></span>  <span data-ttu-id="48626-108">API の将来のリリースでは、チームまたはチャネルの範囲外にいるユーザーの間で直接チャットを読み取り/書き込みと同様に、既存の chatThreads の読み取りをサポートします。</span><span class="sxs-lookup"><span data-stu-id="48626-108">Future API releases will support reading existing chatThreads, as well as reading/writing direct chats between users that are outside the scope of a team or channel.</span></span>

## <a name="methods"></a><span data-ttu-id="48626-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="48626-109">Methods</span></span>

| <span data-ttu-id="48626-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="48626-110">Method</span></span>       | <span data-ttu-id="48626-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="48626-111">Return Type</span></span>  |<span data-ttu-id="48626-112">説明</span><span class="sxs-lookup"><span data-stu-id="48626-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="48626-113">スレッドを作成する</span><span class="sxs-lookup"><span data-stu-id="48626-113">Create thread</span></span>](../api/channel-post-chatthreads.md) | [<span data-ttu-id="48626-114">chatThread</span><span class="sxs-lookup"><span data-stu-id="48626-114">chatThread</span></span>](chatthread.md) |<span data-ttu-id="48626-115">指定のチャネルでは、最初のメッセージを提供する新しいスレッドを開始します。</span><span class="sxs-lookup"><span data-stu-id="48626-115">Start a new thread in the specified channel, providing the first message.</span></span>|

## <a name="properties"></a><span data-ttu-id="48626-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="48626-116">Properties</span></span>
| <span data-ttu-id="48626-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="48626-117">Property</span></span>     | <span data-ttu-id="48626-118">型</span><span class="sxs-lookup"><span data-stu-id="48626-118">Type</span></span>   |<span data-ttu-id="48626-119">説明</span><span class="sxs-lookup"><span data-stu-id="48626-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="48626-120">id</span><span class="sxs-lookup"><span data-stu-id="48626-120">id</span></span>|<span data-ttu-id="48626-121">String</span><span class="sxs-lookup"><span data-stu-id="48626-121">String</span></span>| <span data-ttu-id="48626-122">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="48626-122">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="48626-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="48626-123">Relationships</span></span>
| <span data-ttu-id="48626-124">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="48626-124">Relationship</span></span> | <span data-ttu-id="48626-125">型</span><span class="sxs-lookup"><span data-stu-id="48626-125">Type</span></span>   |<span data-ttu-id="48626-126">説明</span><span class="sxs-lookup"><span data-stu-id="48626-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="48626-127">rootMessage</span><span class="sxs-lookup"><span data-stu-id="48626-127">rootMessage</span></span>|[<span data-ttu-id="48626-128">chatMessage</span><span class="sxs-lookup"><span data-stu-id="48626-128">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="48626-129">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="48626-129">Nullable.</span></span>|
|<span data-ttu-id="48626-130">chatMessages</span><span class="sxs-lookup"><span data-stu-id="48626-130">chatMessages</span></span>|<span data-ttu-id="48626-131">[chatMessage](chatmessage.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="48626-131">[chatMessage](chatmessage.md) collection</span></span>| <span data-ttu-id="48626-132">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="48626-132">Nullable.</span></span>|

> <span data-ttu-id="48626-133">現在これらの関係、暗黙的に存在が、ことはできませんを読み取ったり書き込んだりします。</span><span class="sxs-lookup"><span data-stu-id="48626-133">Currently these relationships exist implicitly, but cannot read or written.</span></span>  <span data-ttu-id="48626-134">今後 API のベータ版のリリースは、これをサポートします。</span><span class="sxs-lookup"><span data-stu-id="48626-134">Future beta API releases will support this.</span></span>

## <a name="json-representation"></a><span data-ttu-id="48626-135">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="48626-135">JSON representation</span></span>

<span data-ttu-id="48626-136">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="48626-136">Here is a JSON representation of the resource</span></span>

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
  "id": "string (identifier)",
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
