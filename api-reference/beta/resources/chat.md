---
title: チャットリソースの種類
description: チャットは、1人または複数の参加者間の chatMessages のコレクションです。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 4d0f1009079c4994814385ae8758af6c211f17a2
ms.sourcegitcommit: afea19508ad74a3583b11b5f7b544c53eafb3740
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/22/2019
ms.locfileid: "34344977"
---
# <a name="chat-resource-type"></a><span data-ttu-id="7dae8-103">チャットリソースの種類</span><span class="sxs-lookup"><span data-stu-id="7dae8-103">chat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7dae8-104">チャットは、1人または複数の参加者間の[Chatmessages](chatmessage.md)のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="7dae8-104">A chat is a collection of [chatMessages](chatmessage.md) between one or more participants.</span></span> <span data-ttu-id="7dae8-105">参加者には、ユーザーまたはアプリがあります。</span><span class="sxs-lookup"><span data-stu-id="7dae8-105">Participants can be users or apps.</span></span>

## <a name="methods"></a><span data-ttu-id="7dae8-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="7dae8-106">Methods</span></span>

|  <span data-ttu-id="7dae8-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="7dae8-107">Method</span></span>       |  <span data-ttu-id="7dae8-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="7dae8-108">Return Type</span></span>  | <span data-ttu-id="7dae8-109">説明</span><span class="sxs-lookup"><span data-stu-id="7dae8-109">Description</span></span>| 
|:---------------|:--------|:----------|
|[<span data-ttu-id="7dae8-110">チャットの一覧表示</span><span class="sxs-lookup"><span data-stu-id="7dae8-110">List chats</span></span>](../api/chat-list.md) | <span data-ttu-id="7dae8-111">[chat](channel.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="7dae8-111">[chat](channel.md) collection</span></span> | <span data-ttu-id="7dae8-112">ユーザーが属するチャットのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="7dae8-112">Get the list of chats a user is part of.</span></span>|
|[<span data-ttu-id="7dae8-113">チャットの取得</span><span class="sxs-lookup"><span data-stu-id="7dae8-113">Get chat</span></span>](../api/chat-get.md) | [<span data-ttu-id="7dae8-114">チャット</span><span class="sxs-lookup"><span data-stu-id="7dae8-114">chat</span></span>](channel.md) | <span data-ttu-id="7dae8-115">チャットのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="7dae8-115">Read properties and relationships of the chat.</span></span>|
|[<span data-ttu-id="7dae8-116">チャットメンバーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="7dae8-116">List chat members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="7dae8-117">[conversationmember](conversationmember.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="7dae8-117">[conversationmember](conversationmember.md) collection</span></span> | <span data-ttu-id="7dae8-118">チャット内のすべてのユーザーの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="7dae8-118">Get the list of all users in the chat.</span></span>|
|[<span data-ttu-id="7dae8-119">チャットメンバーを取得する</span><span class="sxs-lookup"><span data-stu-id="7dae8-119">Get chat member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="7dae8-120">conversationmember</span><span class="sxs-lookup"><span data-stu-id="7dae8-120">conversationmember</span></span>](conversationmember.md) | <span data-ttu-id="7dae8-121">チャットで1人のユーザーを取得します。</span><span class="sxs-lookup"><span data-stu-id="7dae8-121">Get a single user in the chat.</span></span>|
|[<span data-ttu-id="7dae8-122">チャット内のメッセージを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="7dae8-122">List messages in a chat</span></span>](../api/chat-list-messages.md)  | [<span data-ttu-id="7dae8-123">chatMessage</span><span class="sxs-lookup"><span data-stu-id="7dae8-123">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="7dae8-124">1 対 1 またはグループ チャットでのメッセージを取得します。</span><span class="sxs-lookup"><span data-stu-id="7dae8-124">Get messages in a 1:1 or group chat.</span></span> |
|[<span data-ttu-id="7dae8-125">チャット内のメッセージを取得する</span><span class="sxs-lookup"><span data-stu-id="7dae8-125">Get message in chat</span></span>](../api/chat-get-message.md)  | [<span data-ttu-id="7dae8-126">chatMessage</span><span class="sxs-lookup"><span data-stu-id="7dae8-126">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="7dae8-127">チャット内の 1 つのメッセージを取得します。</span><span class="sxs-lookup"><span data-stu-id="7dae8-127">Get a single message in a chat.</span></span> |

## <a name="properties"></a><span data-ttu-id="7dae8-128">Properties</span><span class="sxs-lookup"><span data-stu-id="7dae8-128">Properties</span></span>

| <span data-ttu-id="7dae8-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7dae8-129">Property</span></span>     | <span data-ttu-id="7dae8-130">型</span><span class="sxs-lookup"><span data-stu-id="7dae8-130">Type</span></span>   |<span data-ttu-id="7dae8-131">説明</span><span class="sxs-lookup"><span data-stu-id="7dae8-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7dae8-132">id</span><span class="sxs-lookup"><span data-stu-id="7dae8-132">id</span></span>| <span data-ttu-id="7dae8-133">String</span><span class="sxs-lookup"><span data-stu-id="7dae8-133">String</span></span>| <span data-ttu-id="7dae8-134">チャットの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="7dae8-134">The chat's unique identifier.</span></span> <span data-ttu-id="7dae8-135">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="7dae8-135">Read-only.</span></span>|
| <span data-ttu-id="7dae8-136">topic</span><span class="sxs-lookup"><span data-stu-id="7dae8-136">topic</span></span>| <span data-ttu-id="7dae8-137">String</span><span class="sxs-lookup"><span data-stu-id="7dae8-137">String</span></span>|  <span data-ttu-id="7dae8-138">オプションチャットの件名またはトピック。</span><span class="sxs-lookup"><span data-stu-id="7dae8-138">(Optional) Subject or topic for the chat.</span></span> <span data-ttu-id="7dae8-139">グループチャットでのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="7dae8-139">Only available for group chats.</span></span>|
| <span data-ttu-id="7dae8-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7dae8-140">createdDateTime</span></span>| <span data-ttu-id="7dae8-141">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7dae8-141">dateTimeOffset</span></span>|  <span data-ttu-id="7dae8-142">チャットが作成された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="7dae8-142">Date and time at which the chat was created.</span></span> <span data-ttu-id="7dae8-143">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="7dae8-143">Read-only.</span></span>|
| <span data-ttu-id="7dae8-144">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="7dae8-144">lastUpdatedDateTime</span></span>| <span data-ttu-id="7dae8-145">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7dae8-145">dateTimeOffset</span></span>|  <span data-ttu-id="7dae8-146">チャットが更新された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="7dae8-146">Date and time at which the chat was updated.</span></span> <span data-ttu-id="7dae8-147">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="7dae8-147">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7dae8-148">関係</span><span class="sxs-lookup"><span data-stu-id="7dae8-148">Relationships</span></span>
| <span data-ttu-id="7dae8-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7dae8-149">Relationship</span></span> | <span data-ttu-id="7dae8-150">型</span><span class="sxs-lookup"><span data-stu-id="7dae8-150">Type</span></span>   |<span data-ttu-id="7dae8-151">説明</span><span class="sxs-lookup"><span data-stu-id="7dae8-151">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7dae8-152">members</span><span class="sxs-lookup"><span data-stu-id="7dae8-152">members</span></span> | <span data-ttu-id="7dae8-153">[conversationMember](conversationmember.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="7dae8-153">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="7dae8-154">チャット内のすべてのユーザーのコレクション。</span><span class="sxs-lookup"><span data-stu-id="7dae8-154">A collection of all people in the chat.</span></span> <span data-ttu-id="7dae8-155">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="7dae8-155">Nullable.</span></span> |
| <span data-ttu-id="7dae8-156">messages</span><span class="sxs-lookup"><span data-stu-id="7dae8-156">messages</span></span> | <span data-ttu-id="7dae8-157">[chatMessage](chatmessage.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7dae8-157">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="7dae8-158">チャット内のすべてのメッセージのコレクション。</span><span class="sxs-lookup"><span data-stu-id="7dae8-158">A collection of all the messages in the chat.</span></span> <span data-ttu-id="7dae8-159">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="7dae8-159">Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7dae8-160">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7dae8-160">JSON representation</span></span>

<span data-ttu-id="7dae8-161">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7dae8-161">Here is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="7dae8-162">関連項目</span><span class="sxs-lookup"><span data-stu-id="7dae8-162">See also</span></span>

- [<span data-ttu-id="7dae8-163">channel</span><span class="sxs-lookup"><span data-stu-id="7dae8-163">channel</span></span>](channel.md)
- [<span data-ttu-id="7dae8-164">chatMessage</span><span class="sxs-lookup"><span data-stu-id="7dae8-164">chatMessage</span></span>](chatmessage.md)

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
