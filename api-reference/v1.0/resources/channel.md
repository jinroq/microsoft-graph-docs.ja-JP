---
title: チャネルのリソースの種類
description: 'チャネルは、チーム内のメッセージのコレクションです。 '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 1db6133b4bb4c74e9515a9f14cc6f430ef0e32d5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033018"
---
# <a name="channel-resource-type"></a><span data-ttu-id="e927b-103">チャネルのリソースの種類</span><span class="sxs-lookup"><span data-stu-id="e927b-103">channel resource type</span></span>

<span data-ttu-id="e927b-104">[チーム](../resources/team.md)はチャネルで構成されています。チャネルは、チームのメンバーと会話する場所です。</span><span class="sxs-lookup"><span data-stu-id="e927b-104">[Teams](../resources/team.md) are made up of channels, which are the conversations you have with your teammates.</span></span> <span data-ttu-id="e927b-105">各チャネルは、特定のトピック、部門、プロジェクト専用です。</span><span class="sxs-lookup"><span data-stu-id="e927b-105">Each channel is dedicated to a specific topic, department, or project.</span></span>
<span data-ttu-id="e927b-106">チャネルは、実際に作業を行う場所、チーム全体に対してテキスト、音声、ビデオによる会話を公開する場所、ファイルを共有する場所、タブを追加する場所です。</span><span class="sxs-lookup"><span data-stu-id="e927b-106">Channels are where the work actually gets done - where text, audio, and video conversations open to the whole team happen, where files are shared, and where tabs are added.</span></span>

## <a name="methods"></a><span data-ttu-id="e927b-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="e927b-107">Methods</span></span>

| <span data-ttu-id="e927b-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="e927b-108">Method</span></span>       | <span data-ttu-id="e927b-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e927b-109">Return Type</span></span>  |<span data-ttu-id="e927b-110">説明</span><span class="sxs-lookup"><span data-stu-id="e927b-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e927b-111">チャネルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="e927b-111">List channels</span></span>](../api/channel-list.md) | <span data-ttu-id="e927b-112">[channel](channel.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e927b-112">[channel](channel.md) collection</span></span> | <span data-ttu-id="e927b-113">このチーム内のチャネルの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="e927b-113">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="e927b-114">チャネルを作成する</span><span class="sxs-lookup"><span data-stu-id="e927b-114">Create channel</span></span>](../api/channel-post.md) | [<span data-ttu-id="e927b-115">channel</span><span class="sxs-lookup"><span data-stu-id="e927b-115">channel</span></span>](channel.md) | <span data-ttu-id="e927b-116">表示名と説明を指定して新しいチャネルを作成します。</span><span class="sxs-lookup"><span data-stu-id="e927b-116">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="e927b-117">チャネルを取得する</span><span class="sxs-lookup"><span data-stu-id="e927b-117">Get channel</span></span>](../api/channel-get.md) | [<span data-ttu-id="e927b-118">channel</span><span class="sxs-lookup"><span data-stu-id="e927b-118">channel</span></span>](channel.md) | <span data-ttu-id="e927b-119">チャネルのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e927b-119">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="e927b-120">チャネルを更新する</span><span class="sxs-lookup"><span data-stu-id="e927b-120">Update channel</span></span>](../api/channel-patch.md) | [<span data-ttu-id="e927b-121">channel</span><span class="sxs-lookup"><span data-stu-id="e927b-121">channel</span></span>](channel.md) | <span data-ttu-id="e927b-122">チャネルのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e927b-122">Update properties of the channel.</span></span>|
|[<span data-ttu-id="e927b-123">チャネルを削除する</span><span class="sxs-lookup"><span data-stu-id="e927b-123">Delete channel</span></span>](../api/channel-delete.md) | <span data-ttu-id="e927b-124">なし</span><span class="sxs-lookup"><span data-stu-id="e927b-124">None</span></span> | <span data-ttu-id="e927b-125">チャネルを削除します。</span><span class="sxs-lookup"><span data-stu-id="e927b-125">Delete a channel.</span></span>|
|[<span data-ttu-id="e927b-126">タブを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="e927b-126">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="e927b-127">teamsTab</span><span class="sxs-lookup"><span data-stu-id="e927b-127">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="e927b-128">チャネルにピン留めされているタブを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="e927b-128">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="e927b-129">タブを取得する</span><span class="sxs-lookup"><span data-stu-id="e927b-129">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="e927b-130">teamsTab</span><span class="sxs-lookup"><span data-stu-id="e927b-130">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="e927b-131">チャネルにピン留めされているタブを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e927b-131">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="e927b-132">タブを追加する</span><span class="sxs-lookup"><span data-stu-id="e927b-132">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="e927b-133">teamsTab</span><span class="sxs-lookup"><span data-stu-id="e927b-133">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="e927b-134">タブをチャネルに追加 (ピン留め) します。</span><span class="sxs-lookup"><span data-stu-id="e927b-134">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="e927b-135">タブを削除する</span><span class="sxs-lookup"><span data-stu-id="e927b-135">Remove tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="e927b-136">なし</span><span class="sxs-lookup"><span data-stu-id="e927b-136">None</span></span> | <span data-ttu-id="e927b-137">チャネルからタブを削除します (ピン留めを外します)。</span><span class="sxs-lookup"><span data-stu-id="e927b-137">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="e927b-138">タブを更新する</span><span class="sxs-lookup"><span data-stu-id="e927b-138">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="e927b-139">teamsTab</span><span class="sxs-lookup"><span data-stu-id="e927b-139">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="e927b-140">タブのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e927b-140">Updates the tab properties.</span></span>|

## <a name="properties"></a><span data-ttu-id="e927b-141">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e927b-141">Properties</span></span>
| <span data-ttu-id="e927b-142">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e927b-142">Property</span></span>     | <span data-ttu-id="e927b-143">型</span><span class="sxs-lookup"><span data-stu-id="e927b-143">Type</span></span>   |<span data-ttu-id="e927b-144">説明</span><span class="sxs-lookup"><span data-stu-id="e927b-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e927b-145">description</span><span class="sxs-lookup"><span data-stu-id="e927b-145">description</span></span>|<span data-ttu-id="e927b-146">String</span><span class="sxs-lookup"><span data-stu-id="e927b-146">String</span></span>|<span data-ttu-id="e927b-147">チャネルの説明テキストです (省略可能)。</span><span class="sxs-lookup"><span data-stu-id="e927b-147">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="e927b-148">displayName</span><span class="sxs-lookup"><span data-stu-id="e927b-148">displayName</span></span>|<span data-ttu-id="e927b-149">String</span><span class="sxs-lookup"><span data-stu-id="e927b-149">String</span></span>|<span data-ttu-id="e927b-150">Microsoft Teams でユーザーに対して表示されるチャネルの名前。</span><span class="sxs-lookup"><span data-stu-id="e927b-150">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="e927b-151">メール</span><span class="sxs-lookup"><span data-stu-id="e927b-151">email</span></span>|<span data-ttu-id="e927b-152">String</span><span class="sxs-lookup"><span data-stu-id="e927b-152">String</span></span>| <span data-ttu-id="e927b-153">チャネルにメッセージを送信するときのメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="e927b-153">The email address for sending messages to the channel.</span></span> <span data-ttu-id="e927b-154">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="e927b-154">Read-only.</span></span>|
|<span data-ttu-id="e927b-155">id</span><span class="sxs-lookup"><span data-stu-id="e927b-155">id</span></span>|<span data-ttu-id="e927b-156">String</span><span class="sxs-lookup"><span data-stu-id="e927b-156">String</span></span>|<span data-ttu-id="e927b-157">チャネルの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="e927b-157">The channels's unique identifier.</span></span> <span data-ttu-id="e927b-158">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="e927b-158">Read-only.</span></span>|
|<span data-ttu-id="e927b-159">webUrl</span><span class="sxs-lookup"><span data-stu-id="e927b-159">webUrl</span></span>|<span data-ttu-id="e927b-160">String</span><span class="sxs-lookup"><span data-stu-id="e927b-160">String</span></span>|<span data-ttu-id="e927b-161">Microsoft Teams のチャネルに移動するハイパーリンク。</span><span class="sxs-lookup"><span data-stu-id="e927b-161">A hyperlink that will navigate to the channel in Microsoft Teams.</span></span> <span data-ttu-id="e927b-162">これは、Microsoft Teams でチャネルを右クリックし、[チームへのリンクを取得] を選択すると作成される URL です。</span><span class="sxs-lookup"><span data-stu-id="e927b-162">This is the URL that you get when you right-click a channel in Microsoft Teams and select Get link to channel.</span></span> <span data-ttu-id="e927b-163">この URL は不透明 blob として扱われる必要があり、また解析されません。</span><span class="sxs-lookup"><span data-stu-id="e927b-163">This URL should be treated as an opaque blob, and not parsed.</span></span> <span data-ttu-id="e927b-164">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="e927b-164">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e927b-165">関係</span><span class="sxs-lookup"><span data-stu-id="e927b-165">Relationships</span></span>
| <span data-ttu-id="e927b-166">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e927b-166">Relationship</span></span> | <span data-ttu-id="e927b-167">型</span><span class="sxs-lookup"><span data-stu-id="e927b-167">Type</span></span>   |<span data-ttu-id="e927b-168">説明</span><span class="sxs-lookup"><span data-stu-id="e927b-168">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e927b-169">tabs</span><span class="sxs-lookup"><span data-stu-id="e927b-169">tabs</span></span>|<span data-ttu-id="e927b-170">[teamsTab](../resources/teamstab.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e927b-170">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="e927b-171">チャネル内のすべてのタブのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="e927b-171">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="e927b-172">ナビゲーションのプロパティです。</span><span class="sxs-lookup"><span data-stu-id="e927b-172">A navigation property.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="e927b-173">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e927b-173">JSON representation</span></span>

<span data-ttu-id="e927b-174">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="e927b-174">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.channel"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "email": "string (identifier)",
  "id": "string",
  "webUrl": "string"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "channel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
