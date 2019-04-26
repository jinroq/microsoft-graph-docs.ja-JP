---
title: チャットリソースの種類
description: チャットは、1人または複数の参加者間の chatmessages のコレクションです。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 1091021235a50d3dfa237467e319da9b131b7a72
ms.sourcegitcommit: 4bdcb5cd3227ff009e10868f2936b3153372b87a
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/25/2019
ms.locfileid: "33301883"
---
# <a name="chat-resource-type"></a><span data-ttu-id="6337d-103">チャットリソースの種類</span><span class="sxs-lookup"><span data-stu-id="6337d-103">chat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6337d-104">チャットは、1人または複数の参加者間の[chatmessages](chatmessage.md)のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="6337d-104">A chat is a collection of [chatMessages](chatmessage.md) between one or more participants.</span></span> <span data-ttu-id="6337d-105">参加者には、ユーザーまたはアプリがあります。</span><span class="sxs-lookup"><span data-stu-id="6337d-105">Participants can be users or apps.</span></span>

## <a name="methods"></a><span data-ttu-id="6337d-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="6337d-106">Methods</span></span>

|  <span data-ttu-id="6337d-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="6337d-107">Method</span></span>       |  <span data-ttu-id="6337d-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="6337d-108">Return Type</span></span>  | <span data-ttu-id="6337d-109">説明</span><span class="sxs-lookup"><span data-stu-id="6337d-109">Description</span></span>| 
|:---------------|:--------|:----------|
|[<span data-ttu-id="6337d-110">チャットの一覧表示</span><span class="sxs-lookup"><span data-stu-id="6337d-110">List chats</span></span>](../api/chat-list.md) | <span data-ttu-id="6337d-111">[chat](channel.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="6337d-111">[chat](channel.md) collection</span></span> | <span data-ttu-id="6337d-112">ユーザーが属するチャットのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="6337d-112">Get the list of chats a user is part of.</span></span>|
|[<span data-ttu-id="6337d-113">チャットの取得</span><span class="sxs-lookup"><span data-stu-id="6337d-113">Get chat</span></span>](../api/chat-get.md) | [<span data-ttu-id="6337d-114">チャット</span><span class="sxs-lookup"><span data-stu-id="6337d-114">chat</span></span>](channel.md) | <span data-ttu-id="6337d-115">チャットのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="6337d-115">Read properties and relationships of the chat.</span></span>|
|[<span data-ttu-id="6337d-116">チャット内のメッセージを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="6337d-116">List messages in a chat</span></span>](../api/chat-list-messages.md)  | [<span data-ttu-id="6337d-117">chatMessage</span><span class="sxs-lookup"><span data-stu-id="6337d-117">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="6337d-118">1:1 またはグループチャットでメッセージを取得します。</span><span class="sxs-lookup"><span data-stu-id="6337d-118">Get messages in a 1:1 or group chat.</span></span> |
|[<span data-ttu-id="6337d-119">チャットでメッセージを取得する</span><span class="sxs-lookup"><span data-stu-id="6337d-119">Get message in chat</span></span>](../api/chat-get-message.md)  | [<span data-ttu-id="6337d-120">chatMessage</span><span class="sxs-lookup"><span data-stu-id="6337d-120">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="6337d-121">チャットで1つのメッセージを取得します。</span><span class="sxs-lookup"><span data-stu-id="6337d-121">Get a single message in a chat.</span></span> |

## <a name="properties"></a><span data-ttu-id="6337d-122">Properties</span><span class="sxs-lookup"><span data-stu-id="6337d-122">Properties</span></span>

| <span data-ttu-id="6337d-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6337d-123">Property</span></span>     | <span data-ttu-id="6337d-124">型</span><span class="sxs-lookup"><span data-stu-id="6337d-124">Type</span></span>   |<span data-ttu-id="6337d-125">説明</span><span class="sxs-lookup"><span data-stu-id="6337d-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6337d-126">id</span><span class="sxs-lookup"><span data-stu-id="6337d-126">id</span></span>| <span data-ttu-id="6337d-127">String</span><span class="sxs-lookup"><span data-stu-id="6337d-127">String</span></span>| <span data-ttu-id="6337d-128">チャットの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="6337d-128">The chat's unique identifier.</span></span> <span data-ttu-id="6337d-129">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="6337d-129">Read-only.</span></span>|
| <span data-ttu-id="6337d-130">topic</span><span class="sxs-lookup"><span data-stu-id="6337d-130">topic</span></span>| <span data-ttu-id="6337d-131">String</span><span class="sxs-lookup"><span data-stu-id="6337d-131">String</span></span>|  <span data-ttu-id="6337d-132">オプションチャットの件名またはトピック。</span><span class="sxs-lookup"><span data-stu-id="6337d-132">(Optional) Subject or topic for the chat.</span></span> <span data-ttu-id="6337d-133">グループチャットでのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="6337d-133">Only available for group chats.</span></span>|
| <span data-ttu-id="6337d-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6337d-134">createdDateTime</span></span>| <span data-ttu-id="6337d-135">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6337d-135">dateTimeOffset</span></span>|  <span data-ttu-id="6337d-136">チャットが作成された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="6337d-136">Date and time at which the chat was created.</span></span> <span data-ttu-id="6337d-137">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="6337d-137">Read-only.</span></span>|
| <span data-ttu-id="6337d-138">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="6337d-138">lastUpdatedDateTime</span></span>| <span data-ttu-id="6337d-139">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6337d-139">dateTimeOffset</span></span>|  <span data-ttu-id="6337d-140">チャットが更新された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="6337d-140">Date and time at which the chat was updated.</span></span> <span data-ttu-id="6337d-141">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="6337d-141">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6337d-142">関係</span><span class="sxs-lookup"><span data-stu-id="6337d-142">Relationships</span></span>
| <span data-ttu-id="6337d-143">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6337d-143">Relationship</span></span> | <span data-ttu-id="6337d-144">型</span><span class="sxs-lookup"><span data-stu-id="6337d-144">Type</span></span>   |<span data-ttu-id="6337d-145">説明</span><span class="sxs-lookup"><span data-stu-id="6337d-145">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6337d-146">messages</span><span class="sxs-lookup"><span data-stu-id="6337d-146">messages</span></span> | <span data-ttu-id="6337d-147">[chatMessage](chatmessage.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6337d-147">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="6337d-148">チャット内のすべてのメッセージのコレクション。</span><span class="sxs-lookup"><span data-stu-id="6337d-148">A collection of all the messages in the chat.</span></span> <span data-ttu-id="6337d-149">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="6337d-149">Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6337d-150">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6337d-150">JSON representation</span></span>

<span data-ttu-id="6337d-151">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6337d-151">Here is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="6337d-152">関連項目</span><span class="sxs-lookup"><span data-stu-id="6337d-152">See also</span></span>

- [<span data-ttu-id="6337d-153">channel</span><span class="sxs-lookup"><span data-stu-id="6337d-153">channel</span></span>](channel.md)
- [<span data-ttu-id="6337d-154">chatMessage</span><span class="sxs-lookup"><span data-stu-id="6337d-154">chatMessage</span></span>](chatmessage.md)

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
