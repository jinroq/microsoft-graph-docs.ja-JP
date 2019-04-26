---
title: チャットリソースの種類
description: チャットは、1人または複数の参加者間の chatmessages のコレクションです。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 1091021235a50d3dfa237467e319da9b131b7a72
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339717"
---
# <a name="chat-resource-type"></a><span data-ttu-id="21b37-103">チャットリソースの種類</span><span class="sxs-lookup"><span data-stu-id="21b37-103">chat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="21b37-104">チャットは、1人または複数の参加者間の[chatmessages](chatmessage.md)のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="21b37-104">A chat is a collection of [chatMessages](chatmessage.md) between one or more participants.</span></span> <span data-ttu-id="21b37-105">参加者には、ユーザーまたはアプリがあります。</span><span class="sxs-lookup"><span data-stu-id="21b37-105">Participants can be users or apps.</span></span>

## <a name="methods"></a><span data-ttu-id="21b37-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="21b37-106">Methods</span></span>

|  <span data-ttu-id="21b37-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="21b37-107">Method</span></span>       |  <span data-ttu-id="21b37-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="21b37-108">Return Type</span></span>  | <span data-ttu-id="21b37-109">説明</span><span class="sxs-lookup"><span data-stu-id="21b37-109">Description</span></span>| 
|:---------------|:--------|:----------|
|[<span data-ttu-id="21b37-110">チャットの一覧表示</span><span class="sxs-lookup"><span data-stu-id="21b37-110">List chats</span></span>](../api/chat-list.md) | <span data-ttu-id="21b37-111">[chat](channel.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="21b37-111">[chat](channel.md) collection</span></span> | <span data-ttu-id="21b37-112">ユーザーが属するチャットのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="21b37-112">Get the list of chats a user is part of.</span></span>|
|[<span data-ttu-id="21b37-113">チャットの取得</span><span class="sxs-lookup"><span data-stu-id="21b37-113">Get chat</span></span>](../api/chat-get.md) | [<span data-ttu-id="21b37-114">チャット</span><span class="sxs-lookup"><span data-stu-id="21b37-114">chat</span></span>](channel.md) | <span data-ttu-id="21b37-115">チャットのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="21b37-115">Read properties and relationships of the chat.</span></span>|
|[<span data-ttu-id="21b37-116">チャット内のメッセージを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="21b37-116">List messages in a chat</span></span>](../api/chat-list-messages.md)  | [<span data-ttu-id="21b37-117">chatMessage</span><span class="sxs-lookup"><span data-stu-id="21b37-117">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="21b37-118">1:1 またはグループチャットでメッセージを取得します。</span><span class="sxs-lookup"><span data-stu-id="21b37-118">Get messages in a 1:1 or group chat.</span></span> |
|[<span data-ttu-id="21b37-119">チャットでメッセージを取得する</span><span class="sxs-lookup"><span data-stu-id="21b37-119">Get message in chat</span></span>](../api/chat-get-message.md)  | [<span data-ttu-id="21b37-120">chatMessage</span><span class="sxs-lookup"><span data-stu-id="21b37-120">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="21b37-121">チャットで1つのメッセージを取得します。</span><span class="sxs-lookup"><span data-stu-id="21b37-121">Get a single message in a chat.</span></span> |

## <a name="properties"></a><span data-ttu-id="21b37-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="21b37-122">Properties</span></span>

| <span data-ttu-id="21b37-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="21b37-123">Property</span></span>     | <span data-ttu-id="21b37-124">型</span><span class="sxs-lookup"><span data-stu-id="21b37-124">Type</span></span>   |<span data-ttu-id="21b37-125">説明</span><span class="sxs-lookup"><span data-stu-id="21b37-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="21b37-126">id</span><span class="sxs-lookup"><span data-stu-id="21b37-126">id</span></span>| <span data-ttu-id="21b37-127">String</span><span class="sxs-lookup"><span data-stu-id="21b37-127">String</span></span>| <span data-ttu-id="21b37-128">チャットの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="21b37-128">The chat's unique identifier.</span></span> <span data-ttu-id="21b37-129">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="21b37-129">Read-only.</span></span>|
| <span data-ttu-id="21b37-130">topic</span><span class="sxs-lookup"><span data-stu-id="21b37-130">topic</span></span>| <span data-ttu-id="21b37-131">String</span><span class="sxs-lookup"><span data-stu-id="21b37-131">String</span></span>|  <span data-ttu-id="21b37-132">オプションチャットの件名またはトピック。</span><span class="sxs-lookup"><span data-stu-id="21b37-132">(Optional) Subject or topic for the chat.</span></span> <span data-ttu-id="21b37-133">グループチャットでのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="21b37-133">Only available for group chats.</span></span>|
| <span data-ttu-id="21b37-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="21b37-134">createdDateTime</span></span>| <span data-ttu-id="21b37-135">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21b37-135">dateTimeOffset</span></span>|  <span data-ttu-id="21b37-136">チャットが作成された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="21b37-136">Date and time at which the chat was created.</span></span> <span data-ttu-id="21b37-137">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="21b37-137">Read-only.</span></span>|
| <span data-ttu-id="21b37-138">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="21b37-138">lastUpdatedDateTime</span></span>| <span data-ttu-id="21b37-139">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21b37-139">dateTimeOffset</span></span>|  <span data-ttu-id="21b37-140">チャットが更新された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="21b37-140">Date and time at which the chat was updated.</span></span> <span data-ttu-id="21b37-141">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="21b37-141">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="21b37-142">関係</span><span class="sxs-lookup"><span data-stu-id="21b37-142">Relationships</span></span>
| <span data-ttu-id="21b37-143">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="21b37-143">Relationship</span></span> | <span data-ttu-id="21b37-144">型</span><span class="sxs-lookup"><span data-stu-id="21b37-144">Type</span></span>   |<span data-ttu-id="21b37-145">説明</span><span class="sxs-lookup"><span data-stu-id="21b37-145">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="21b37-146">messages</span><span class="sxs-lookup"><span data-stu-id="21b37-146">messages</span></span> | <span data-ttu-id="21b37-147">[chatMessage](chatmessage.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="21b37-147">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="21b37-148">チャット内のすべてのメッセージのコレクション。</span><span class="sxs-lookup"><span data-stu-id="21b37-148">A collection of all the messages in the chat.</span></span> <span data-ttu-id="21b37-149">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="21b37-149">Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="21b37-150">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="21b37-150">JSON representation</span></span>

<span data-ttu-id="21b37-151">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="21b37-151">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.chat"
}-->

```json
{
  "id": "string (identifier)",
  "topic": "string",
  "createdDateTime": "dateTimeOffset",
  "lastUpdatedDateTime": "dateTimeOffset"
}

```

## <a name="see-also"></a><span data-ttu-id="21b37-152">関連項目</span><span class="sxs-lookup"><span data-stu-id="21b37-152">See also</span></span>

- [<span data-ttu-id="21b37-153">channel</span><span class="sxs-lookup"><span data-stu-id="21b37-153">channel</span></span>](channel.md)
- [<span data-ttu-id="21b37-154">chatMessage</span><span class="sxs-lookup"><span data-stu-id="21b37-154">chatMessage</span></span>](chatmessage.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "chat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}
-->
