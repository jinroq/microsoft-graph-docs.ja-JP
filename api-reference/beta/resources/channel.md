---
title: チャネルのリソースの種類
description: 'チャネルは、チーム内の chatMessages のコレクションです。 '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: d58a3e0b867a675e378fa126108331fd5b27856c
ms.sourcegitcommit: a4773239d8559899c3f9433b3073e250a56d2e04
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/13/2019
ms.locfileid: "29994469"
---
# <a name="channel-resource-type"></a><span data-ttu-id="81a8d-103">チャネルのリソースの種類</span><span class="sxs-lookup"><span data-stu-id="81a8d-103">channel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81a8d-104">チャネルは、[チーム](../resources/team.md)内の [chatMessages](chatmessage.md) のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="81a8d-104">A channel is a collection of [chatMessages](chatmessage.md) within a [team](../resources/team.md).</span></span> <span data-ttu-id="81a8d-105">チャネルは 1 つのトピック、つまりチーム内でのディスカッションの論理的分離を表します。</span><span class="sxs-lookup"><span data-stu-id="81a8d-105">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span> <span data-ttu-id="81a8d-106">たとえば、「Friday Team Lunch (金曜日のチーム ランチ)」チャネルや「Architecture Discussion (アーキテクチャに関するディスカッション)」チャネルなどです。</span><span class="sxs-lookup"><span data-stu-id="81a8d-106">Examples can be "Friday Team Lunch" channel, and "Architecture Discussion" channel.</span></span>


## <a name="methods"></a><span data-ttu-id="81a8d-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="81a8d-107">Methods</span></span>

| <span data-ttu-id="81a8d-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="81a8d-108">Method</span></span>       | <span data-ttu-id="81a8d-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="81a8d-109">Return Type</span></span>  |<span data-ttu-id="81a8d-110">説明</span><span class="sxs-lookup"><span data-stu-id="81a8d-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="81a8d-111">チャネルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="81a8d-111">List channels</span></span>](../api/channel-list.md) | <span data-ttu-id="81a8d-112">[channel](channel.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="81a8d-112">[channel](channel.md) collection</span></span> | <span data-ttu-id="81a8d-113">このチーム内のチャネルの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="81a8d-113">Retrieve the list of channels in this team.</span></span>|
|[<span data-ttu-id="81a8d-114">チャネルを作成する</span><span class="sxs-lookup"><span data-stu-id="81a8d-114">Create channel</span></span>](../api/channel-post.md) | [<span data-ttu-id="81a8d-115">channel</span><span class="sxs-lookup"><span data-stu-id="81a8d-115">channel</span></span>](channel.md) | <span data-ttu-id="81a8d-116">表示名と説明を指定して新しいチャネルを作成します。</span><span class="sxs-lookup"><span data-stu-id="81a8d-116">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="81a8d-117">チャネルを取得する</span><span class="sxs-lookup"><span data-stu-id="81a8d-117">Get channel</span></span>](../api/channel-get.md) | [<span data-ttu-id="81a8d-118">channel</span><span class="sxs-lookup"><span data-stu-id="81a8d-118">channel</span></span>](channel.md) | <span data-ttu-id="81a8d-119">チャネルのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="81a8d-119">Read properties and relationships of the windowsInformationProtectionNetworkLearningSummary object.</span></span>|
|[<span data-ttu-id="81a8d-120">チャネルを更新する</span><span class="sxs-lookup"><span data-stu-id="81a8d-120">Update channel</span></span>](../api/channel-patch.md) | [<span data-ttu-id="81a8d-121">channel</span><span class="sxs-lookup"><span data-stu-id="81a8d-121">channel</span></span>](channel.md) | <span data-ttu-id="81a8d-122">チャネルのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="81a8d-122">Update properties of the channel.</span></span>|
|<span data-ttu-id="81a8d-123">[チャネルを削除する](../api/channel-delete.md)</span><span class="sxs-lookup"><span data-stu-id="81a8d-123">[](../api/channel-delete.md)Delete a device channel</span></span> | <span data-ttu-id="81a8d-124">なし</span><span class="sxs-lookup"><span data-stu-id="81a8d-124">None</span></span> | <span data-ttu-id="81a8d-125">チャネルを削除します。</span><span class="sxs-lookup"><span data-stu-id="81a8d-125">Delete a device channel</span></span>|
|[<span data-ttu-id="81a8d-126">チャネル メッセージを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="81a8d-126">List channel messages</span></span>](../api/channel-list-messages.md)  | [<span data-ttu-id="81a8d-127">chatMessage</span><span class="sxs-lookup"><span data-stu-id="81a8d-127">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="81a8d-128">チャネルのメッセージを取得します。</span><span class="sxs-lookup"><span data-stu-id="81a8d-128">Get messages in a channel</span></span> |
|[<span data-ttu-id="81a8d-129">チャネル メッセージを送信する</span><span class="sxs-lookup"><span data-stu-id="81a8d-129">Send channel message</span></span>](../api/channel-post-chatmessage.md)  | [<span data-ttu-id="81a8d-130">chatMessage</span><span class="sxs-lookup"><span data-stu-id="81a8d-130">chatMessage</span></span>](../resources/chatmessage.md) | [<span data-ttu-id="81a8d-131">メッセージをチャネルに送信する</span><span class="sxs-lookup"><span data-stu-id="81a8d-131">Send a message to a channel</span></span>](../api/channel-post-chatmessage.md) |


## <a name="properties"></a><span data-ttu-id="81a8d-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="81a8d-132">Properties</span></span>
| <span data-ttu-id="81a8d-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="81a8d-133">Property</span></span>     | <span data-ttu-id="81a8d-134">型</span><span class="sxs-lookup"><span data-stu-id="81a8d-134">Type</span></span>   |<span data-ttu-id="81a8d-135">説明</span><span class="sxs-lookup"><span data-stu-id="81a8d-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="81a8d-136">description</span><span class="sxs-lookup"><span data-stu-id="81a8d-136">description</span></span>|<span data-ttu-id="81a8d-137">String</span><span class="sxs-lookup"><span data-stu-id="81a8d-137">String</span></span>|<span data-ttu-id="81a8d-138">チャネルの説明テキストです (省略可能)。</span><span class="sxs-lookup"><span data-stu-id="81a8d-138">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="81a8d-139">displayName</span><span class="sxs-lookup"><span data-stu-id="81a8d-139">displayName</span></span>|<span data-ttu-id="81a8d-140">String</span><span class="sxs-lookup"><span data-stu-id="81a8d-140">String</span></span>|<span data-ttu-id="81a8d-141">Microsoft Teams でユーザーに対して表示されるチャネルの名前。</span><span class="sxs-lookup"><span data-stu-id="81a8d-141">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="81a8d-142">id</span><span class="sxs-lookup"><span data-stu-id="81a8d-142">id</span></span>|<span data-ttu-id="81a8d-143">String</span><span class="sxs-lookup"><span data-stu-id="81a8d-143">String</span></span>|<span data-ttu-id="81a8d-144">チャネルの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="81a8d-144">The unique identifier.</span></span> <span data-ttu-id="81a8d-145">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="81a8d-145">Read-only.</span></span>|
|<span data-ttu-id="81a8d-146">isFavoriteByDefault</span><span class="sxs-lookup"><span data-stu-id="81a8d-146">isFavoriteByDefault</span></span>|<span data-ttu-id="81a8d-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="81a8d-147">Boolean</span></span>|<span data-ttu-id="81a8d-148">チームのメンバー全員に対してチャネルを「お気に入り」として自動的にマークするかどうか。</span><span class="sxs-lookup"><span data-stu-id="81a8d-148">Whether the channel should automatically be marked 'favorite' for all members of the team.</span></span> <span data-ttu-id="81a8d-149">既定値: `false`。</span><span class="sxs-lookup"><span data-stu-id="81a8d-149">`false`  .</span></span>|
|<span data-ttu-id="81a8d-150">email</span><span class="sxs-lookup"><span data-stu-id="81a8d-150">email</span></span>|<span data-ttu-id="81a8d-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="81a8d-151">Boolean</span></span>| <span data-ttu-id="81a8d-152">チャネルにメッセージを送信するときのメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="81a8d-152">The email address for sending messages to the channel.</span></span> <span data-ttu-id="81a8d-153">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="81a8d-153">Read-only.</span></span>|
|<span data-ttu-id="81a8d-154">webUrl</span><span class="sxs-lookup"><span data-stu-id="81a8d-154">webUrl</span></span>|<span data-ttu-id="81a8d-155">String</span><span class="sxs-lookup"><span data-stu-id="81a8d-155">String</span></span>|<span data-ttu-id="81a8d-156">Microsoft Teams のチャネルに移動するハイパーリンク。</span><span class="sxs-lookup"><span data-stu-id="81a8d-156">A hyperlink that will go to the team in the Microsoft Teams client.</span></span> <span data-ttu-id="81a8d-157">これは、Microsoft Teams でチャネルを右クリックし、[チームへのリンクを取得] を選択すると作成される URL です。</span><span class="sxs-lookup"><span data-stu-id="81a8d-157">This is the URL that you get when you right-click a team in the Microsoft Teams client and select Get link to team.</span></span> <span data-ttu-id="81a8d-158">この URL は不透明 blob として扱われる必要があり、また解析されません。</span><span class="sxs-lookup"><span data-stu-id="81a8d-158">This URL should be treated as an opaque blob, and not parsed.</span></span> <span data-ttu-id="81a8d-159">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="81a8d-159">Read-only.</span></span>|


## <a name="relationships"></a><span data-ttu-id="81a8d-160">関係</span><span class="sxs-lookup"><span data-stu-id="81a8d-160">Relationships</span></span>
| <span data-ttu-id="81a8d-161">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="81a8d-161">Relationship</span></span> | <span data-ttu-id="81a8d-162">型</span><span class="sxs-lookup"><span data-stu-id="81a8d-162">Type</span></span>   |<span data-ttu-id="81a8d-163">説明</span><span class="sxs-lookup"><span data-stu-id="81a8d-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="81a8d-164">messages</span><span class="sxs-lookup"><span data-stu-id="81a8d-164">messages</span></span>|<span data-ttu-id="81a8d-165">[chatMessage](chatmessage.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="81a8d-165">[chatMessage](chatmessage.md) collection</span></span>|<span data-ttu-id="81a8d-166">チャネル内のすべてのメッセージのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="81a8d-166">A collection of all the messages in the channel.</span></span> <span data-ttu-id="81a8d-167">ナビゲーションのプロパティです。</span><span class="sxs-lookup"><span data-stu-id="81a8d-167">A navigation property.</span></span> <span data-ttu-id="81a8d-168">Null 許容型です。</span><span class="sxs-lookup"><span data-stu-id="81a8d-168">Nullable.</span></span> <span data-ttu-id="81a8d-169">現在この API では読み取りだけがサポートされていますが、最終的にはメッセージの作成もサポートされる予定です。</span><span class="sxs-lookup"><span data-stu-id="81a8d-169">Currently this API only supports reading but will eventually support writing messages too.</span></span>|
|<span data-ttu-id="81a8d-170">tabs</span><span class="sxs-lookup"><span data-stu-id="81a8d-170">Tabs</span></span>|<span data-ttu-id="81a8d-171">[teamsTab](../resources/teamstab.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="81a8d-171">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="81a8d-172">チャネル内のすべてのタブのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="81a8d-172">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="81a8d-173">ナビゲーションのプロパティです。</span><span class="sxs-lookup"><span data-stu-id="81a8d-173">A navigation property.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="81a8d-174">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="81a8d-174">JSON representation</span></span>

<span data-ttu-id="81a8d-175">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="81a8d-175">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "messages"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.channel"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)",
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "channel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/channel.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
