---
title: チャネルのリソースの種類
description: 'チャネルは、チーム内のメッセージのコレクションです。 '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 2bebf78e4ad31047289bff77e681c34d92a94abf
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163715"
---
# <a name="channel-resource-type"></a><span data-ttu-id="5b363-103">チャネルのリソースの種類</span><span class="sxs-lookup"><span data-stu-id="5b363-103">channel resource type</span></span>



<span data-ttu-id="5b363-104">チャネルは、[チーム](../resources/team.md)内のメッセージのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="5b363-104">A channel is a collection of messages within a [team](../resources/team.md).</span></span> <span data-ttu-id="5b363-105">チャネルは 1 つのトピック、つまりチーム内でのディスカッションの論理的分離を表します。</span><span class="sxs-lookup"><span data-stu-id="5b363-105">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span> <span data-ttu-id="5b363-106">たとえば、「Friday Team Lunch (金曜日のチーム ランチ)」チャネルや「Architecture Discussion (アーキテクチャに関するディスカッション)」チャネルなどです。</span><span class="sxs-lookup"><span data-stu-id="5b363-106">Examples can be "Friday Team Lunch" channel, and "Architecture Discussion" channel.</span></span>


## <a name="methods"></a><span data-ttu-id="5b363-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="5b363-107">Methods</span></span>

| <span data-ttu-id="5b363-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="5b363-108">Method</span></span>       | <span data-ttu-id="5b363-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="5b363-109">Return Type</span></span>  |<span data-ttu-id="5b363-110">説明</span><span class="sxs-lookup"><span data-stu-id="5b363-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5b363-111">チャネルを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="5b363-111">List channels</span></span>](../api/channel-list.md) | <span data-ttu-id="5b363-112">[channel](channel.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="5b363-112">[channel](channel.md) collection</span></span> | <span data-ttu-id="5b363-113">このチーム内のチャネルの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="5b363-113">Retrieve the list of channels in this team.</span></span>|
|[<span data-ttu-id="5b363-114">チャネルを作成する</span><span class="sxs-lookup"><span data-stu-id="5b363-114">Create channel</span></span>](../api/channel-post.md) | [<span data-ttu-id="5b363-115">channel</span><span class="sxs-lookup"><span data-stu-id="5b363-115">channel</span></span>](channel.md) | <span data-ttu-id="5b363-116">表示名と説明を指定して新しいチャネルを作成します。</span><span class="sxs-lookup"><span data-stu-id="5b363-116">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="5b363-117">チャネルを取得する</span><span class="sxs-lookup"><span data-stu-id="5b363-117">Get channel</span></span>](../api/channel-get.md) | [<span data-ttu-id="5b363-118">channel</span><span class="sxs-lookup"><span data-stu-id="5b363-118">channel</span></span>](channel.md) | <span data-ttu-id="5b363-119">チャネルのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="5b363-119">Read the properties and relationships of the page.</span></span>|
|[<span data-ttu-id="5b363-120">チャネルを更新する</span><span class="sxs-lookup"><span data-stu-id="5b363-120">Update channel</span></span>](../api/channel-patch.md) | [<span data-ttu-id="5b363-121">channel</span><span class="sxs-lookup"><span data-stu-id="5b363-121">channel</span></span>](channel.md) | <span data-ttu-id="5b363-122">チャネルのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="5b363-122">Update properties of the channel.</span></span>|
|[<span data-ttu-id="5b363-123">チャネルを削除する</span><span class="sxs-lookup"><span data-stu-id="5b363-123">Delete channel</span></span>](../api/channel-delete.md) | <span data-ttu-id="5b363-124">なし</span><span class="sxs-lookup"><span data-stu-id="5b363-124">None</span></span> | <span data-ttu-id="5b363-125">チャネルを削除します。</span><span class="sxs-lookup"><span data-stu-id="5b363-125">Delete a device channel</span></span>|

## <a name="properties"></a><span data-ttu-id="5b363-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5b363-126">Properties</span></span>
| <span data-ttu-id="5b363-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5b363-127">Property</span></span>     | <span data-ttu-id="5b363-128">型</span><span class="sxs-lookup"><span data-stu-id="5b363-128">Type</span></span>   |<span data-ttu-id="5b363-129">説明</span><span class="sxs-lookup"><span data-stu-id="5b363-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5b363-130">description</span><span class="sxs-lookup"><span data-stu-id="5b363-130">description</span></span>|<span data-ttu-id="5b363-131">String</span><span class="sxs-lookup"><span data-stu-id="5b363-131">String</span></span>|<span data-ttu-id="5b363-132">チャネルの説明テキストです (省略可能)。</span><span class="sxs-lookup"><span data-stu-id="5b363-132">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="5b363-133">displayName</span><span class="sxs-lookup"><span data-stu-id="5b363-133">displayName</span></span>|<span data-ttu-id="5b363-134">String</span><span class="sxs-lookup"><span data-stu-id="5b363-134">String</span></span>|<span data-ttu-id="5b363-135">Microsoft Teams でユーザーに対して表示されるチャネルの名前。</span><span class="sxs-lookup"><span data-stu-id="5b363-135">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="5b363-136">id</span><span class="sxs-lookup"><span data-stu-id="5b363-136">id</span></span>|<span data-ttu-id="5b363-137">String</span><span class="sxs-lookup"><span data-stu-id="5b363-137">String</span></span>|<span data-ttu-id="5b363-138">チャネルの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="5b363-138">The unique identifier.</span></span> <span data-ttu-id="5b363-139">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="5b363-139">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5b363-140">関係</span><span class="sxs-lookup"><span data-stu-id="5b363-140">Relationships</span></span>
| <span data-ttu-id="5b363-141">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5b363-141">Relationship</span></span> | <span data-ttu-id="5b363-142">型</span><span class="sxs-lookup"><span data-stu-id="5b363-142">Type</span></span>   |<span data-ttu-id="5b363-143">説明</span><span class="sxs-lookup"><span data-stu-id="5b363-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5b363-144">tabs</span><span class="sxs-lookup"><span data-stu-id="5b363-144">Tabs</span></span>|<span data-ttu-id="5b363-145">[teamsTab](../resources/teamstab.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="5b363-145">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="5b363-146">チャネル内のすべてのタブのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="5b363-146">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="5b363-147">ナビゲーションのプロパティです。</span><span class="sxs-lookup"><span data-stu-id="5b363-147">A navigation property.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="5b363-148">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5b363-148">JSON representation</span></span>

<span data-ttu-id="5b363-149">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="5b363-149">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.channel"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)"
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
