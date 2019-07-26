---
title: チャットリソースの種類
description: チャットは、1人または複数の参加者間の chatMessages のコレクションです。
author: clearab
doc_type: resourcePageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 83ab8428fb09a7a2dc0546dcebdf2f409d90d25a
ms.sourcegitcommit: 82b73552fff79a4ef7a2ee57fc2d1b3286b5bd4c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/26/2019
ms.locfileid: "35908494"
---
# <a name="chat-resource-type"></a><span data-ttu-id="ef357-103">チャットリソースの種類</span><span class="sxs-lookup"><span data-stu-id="ef357-103">chat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef357-104">チャットは、1人または複数の参加者間の[Chatmessages](chatmessage.md)のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="ef357-104">A chat is a collection of [chatMessages](chatmessage.md) between one or more participants.</span></span> <span data-ttu-id="ef357-105">参加者には、ユーザーまたはアプリがあります。</span><span class="sxs-lookup"><span data-stu-id="ef357-105">Participants can be users or apps.</span></span>

## <a name="methods"></a><span data-ttu-id="ef357-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="ef357-106">Methods</span></span>

|  <span data-ttu-id="ef357-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="ef357-107">Method</span></span>       |  <span data-ttu-id="ef357-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ef357-108">Return Type</span></span>  | <span data-ttu-id="ef357-109">説明</span><span class="sxs-lookup"><span data-stu-id="ef357-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ef357-110">チャットの一覧表示</span><span class="sxs-lookup"><span data-stu-id="ef357-110">List chats</span></span>](../api/chat-list.md) | <span data-ttu-id="ef357-111">[chat](channel.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="ef357-111">[chat](channel.md) collection</span></span> | <span data-ttu-id="ef357-112">ユーザーが属するチャットのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="ef357-112">Get the list of chats a user is part of.</span></span>|
|[<span data-ttu-id="ef357-113">チャットの取得</span><span class="sxs-lookup"><span data-stu-id="ef357-113">Get chat</span></span>](../api/chat-get.md) | [<span data-ttu-id="ef357-114">チャット</span><span class="sxs-lookup"><span data-stu-id="ef357-114">chat</span></span>](channel.md) | <span data-ttu-id="ef357-115">チャットのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="ef357-115">Read properties and relationships of the chat.</span></span>|
|[<span data-ttu-id="ef357-116">チャットメンバーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="ef357-116">List chat members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="ef357-117">[conversationmember](conversationmember.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="ef357-117">[conversationmember](conversationmember.md) collection</span></span> | <span data-ttu-id="ef357-118">チャット内のすべてのユーザーの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="ef357-118">Get the list of all users in the chat.</span></span>|
|[<span data-ttu-id="ef357-119">チャットメンバーを取得する</span><span class="sxs-lookup"><span data-stu-id="ef357-119">Get chat member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="ef357-120">conversationmember</span><span class="sxs-lookup"><span data-stu-id="ef357-120">conversationmember</span></span>](conversationmember.md) | <span data-ttu-id="ef357-121">チャットで1人のユーザーを取得します。</span><span class="sxs-lookup"><span data-stu-id="ef357-121">Get a single user in the chat.</span></span>|
|[<span data-ttu-id="ef357-122">チャット内のメッセージを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="ef357-122">List messages in a chat</span></span>](../api/chatmessage-list.md)  | [<span data-ttu-id="ef357-123">chatMessage</span><span class="sxs-lookup"><span data-stu-id="ef357-123">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="ef357-124">1 対 1 またはグループ チャットでのメッセージを取得します。</span><span class="sxs-lookup"><span data-stu-id="ef357-124">Get messages in a 1:1 or group chat.</span></span> |
|[<span data-ttu-id="ef357-125">チャット内のメッセージを取得する</span><span class="sxs-lookup"><span data-stu-id="ef357-125">Get message in chat</span></span>](../api/chatmessage-get.md)  | [<span data-ttu-id="ef357-126">chatMessage</span><span class="sxs-lookup"><span data-stu-id="ef357-126">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="ef357-127">チャット内の 1 つのメッセージを取得します。</span><span class="sxs-lookup"><span data-stu-id="ef357-127">Get a single message in a chat.</span></span> |

## <a name="properties"></a><span data-ttu-id="ef357-128">Properties</span><span class="sxs-lookup"><span data-stu-id="ef357-128">Properties</span></span>

| <span data-ttu-id="ef357-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ef357-129">Property</span></span>   | <span data-ttu-id="ef357-130">型</span><span class="sxs-lookup"><span data-stu-id="ef357-130">Type</span></span> |<span data-ttu-id="ef357-131">説明</span><span class="sxs-lookup"><span data-stu-id="ef357-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ef357-132">id</span><span class="sxs-lookup"><span data-stu-id="ef357-132">id</span></span>| <span data-ttu-id="ef357-133">String</span><span class="sxs-lookup"><span data-stu-id="ef357-133">String</span></span>| <span data-ttu-id="ef357-134">チャットの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="ef357-134">The chat's unique identifier.</span></span> <span data-ttu-id="ef357-135">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ef357-135">Read-only.</span></span>|
| <span data-ttu-id="ef357-136">topic</span><span class="sxs-lookup"><span data-stu-id="ef357-136">topic</span></span>| <span data-ttu-id="ef357-137">String</span><span class="sxs-lookup"><span data-stu-id="ef357-137">String</span></span>|  <span data-ttu-id="ef357-138">オプションチャットの件名またはトピック。</span><span class="sxs-lookup"><span data-stu-id="ef357-138">(Optional) Subject or topic for the chat.</span></span> <span data-ttu-id="ef357-139">グループチャットでのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="ef357-139">Only available for group chats.</span></span>|
| <span data-ttu-id="ef357-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ef357-140">createdDateTime</span></span>| <span data-ttu-id="ef357-141">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef357-141">dateTimeOffset</span></span>|  <span data-ttu-id="ef357-142">チャットが作成された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="ef357-142">Date and time at which the chat was created.</span></span> <span data-ttu-id="ef357-143">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ef357-143">Read-only.</span></span>|
| <span data-ttu-id="ef357-144">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="ef357-144">lastUpdatedDateTime</span></span>| <span data-ttu-id="ef357-145">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef357-145">dateTimeOffset</span></span>|  <span data-ttu-id="ef357-146">チャットが更新された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="ef357-146">Date and time at which the chat was updated.</span></span> <span data-ttu-id="ef357-147">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ef357-147">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ef357-148">関係</span><span class="sxs-lookup"><span data-stu-id="ef357-148">Relationships</span></span>

| <span data-ttu-id="ef357-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ef357-149">Relationship</span></span> | <span data-ttu-id="ef357-150">型</span><span class="sxs-lookup"><span data-stu-id="ef357-150">Type</span></span> |<span data-ttu-id="ef357-151">説明</span><span class="sxs-lookup"><span data-stu-id="ef357-151">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ef357-152">installedApps</span><span class="sxs-lookup"><span data-stu-id="ef357-152">installedApps</span></span> | <span data-ttu-id="ef357-153">[teamsAppInstallation](teamsappinstallation.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ef357-153">[teamsAppInstallation](teamsappinstallation.md) collection</span></span> | <span data-ttu-id="ef357-154">チャット内のすべてのアプリのコレクション。</span><span class="sxs-lookup"><span data-stu-id="ef357-154">A collection of all the apps in the chat.</span></span> <span data-ttu-id="ef357-155">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="ef357-155">Nullable.</span></span> |
| <span data-ttu-id="ef357-156">members</span><span class="sxs-lookup"><span data-stu-id="ef357-156">members</span></span> | <span data-ttu-id="ef357-157">[conversationMember](conversationmember.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="ef357-157">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="ef357-158">チャット内のすべてのユーザーのコレクション。</span><span class="sxs-lookup"><span data-stu-id="ef357-158">A collection of all people in the chat.</span></span> <span data-ttu-id="ef357-159">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="ef357-159">Nullable.</span></span> |
| <span data-ttu-id="ef357-160">messages</span><span class="sxs-lookup"><span data-stu-id="ef357-160">messages</span></span> | <span data-ttu-id="ef357-161">[chatMessage](chatmessage.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ef357-161">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="ef357-162">チャット内のすべてのメッセージのコレクション。</span><span class="sxs-lookup"><span data-stu-id="ef357-162">A collection of all the messages in the chat.</span></span> <span data-ttu-id="ef357-163">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="ef357-163">Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ef357-164">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ef357-164">JSON representation</span></span>

<span data-ttu-id="ef357-165">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ef357-165">Here is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="ef357-166">関連項目</span><span class="sxs-lookup"><span data-stu-id="ef357-166">See also</span></span>

- [<span data-ttu-id="ef357-167">channel</span><span class="sxs-lookup"><span data-stu-id="ef357-167">channel</span></span>](channel.md)
- [<span data-ttu-id="ef357-168">chatMessage</span><span class="sxs-lookup"><span data-stu-id="ef357-168">chatMessage</span></span>](chatmessage.md)

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
