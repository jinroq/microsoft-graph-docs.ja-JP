---
title: チャネル リソースの種類
description: 'チャネルは、チーム内でのメッセージのコレクションです。 '
author: nkramer
localization_priority: Priority
ms.openlocfilehash: 9a7b12646f36152bef17cec2d206e8e84abdcbbe
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826566"
---
# <a name="channel-resource-type"></a><span data-ttu-id="c177c-103">チャネル リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c177c-103">channel resource type</span></span>



<span data-ttu-id="c177c-104">チャネルは、[チーム](../resources/team.md)内でのメッセージのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="c177c-104">A channel is a collection of messages within a [team](../resources/team.md).</span></span> <span data-ttu-id="c177c-105">チャネルでは、トピックとチーム内での議論の論理的分離を表します。</span><span class="sxs-lookup"><span data-stu-id="c177c-105">A channel represents a topic, and therefore a logical isolation of discussion, within a team.</span></span> <span data-ttu-id="c177c-106">例としては、「金曜日チーム ランチ」のチャネルとチャネルの「アーキテクチャの説明」にあります。</span><span class="sxs-lookup"><span data-stu-id="c177c-106">Examples can be "Friday Team Lunch" channel, and "Architecture Discussion" channel.</span></span>


## <a name="methods"></a><span data-ttu-id="c177c-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="c177c-107">Methods</span></span>

| <span data-ttu-id="c177c-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="c177c-108">Method</span></span>       | <span data-ttu-id="c177c-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c177c-109">Return Type</span></span>  |<span data-ttu-id="c177c-110">説明</span><span class="sxs-lookup"><span data-stu-id="c177c-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c177c-111">チャネルのリスト</span><span class="sxs-lookup"><span data-stu-id="c177c-111">List channels</span></span>](../api/channel-list.md) | <span data-ttu-id="c177c-112">[チャネル](channel.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="c177c-112">[channel](channel.md) collection</span></span> | <span data-ttu-id="c177c-113">このチームでは、チャネルの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="c177c-113">Get the list of channels in this team.</span></span>|
|[<span data-ttu-id="c177c-114">チャネルを作成します。</span><span class="sxs-lookup"><span data-stu-id="c177c-114">Create channel</span></span>](../api/channel-post.md) | [<span data-ttu-id="c177c-115">チャネル</span><span class="sxs-lookup"><span data-stu-id="c177c-115">channel</span></span>](channel.md) | <span data-ttu-id="c177c-116">表示名と説明を含めることで、新しいチャネルを作成します。</span><span class="sxs-lookup"><span data-stu-id="c177c-116">Create a new channel by including the display name and description.</span></span>|
|[<span data-ttu-id="c177c-117">チャネルを取得します。</span><span class="sxs-lookup"><span data-stu-id="c177c-117">Get channel</span></span>](../api/channel-get.md) | [<span data-ttu-id="c177c-118">チャネル</span><span class="sxs-lookup"><span data-stu-id="c177c-118">channel</span></span>](channel.md) | <span data-ttu-id="c177c-119">チャネルのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c177c-119">Read properties and relationships of the channel.</span></span>|
|[<span data-ttu-id="c177c-120">チャネルを更新します。</span><span class="sxs-lookup"><span data-stu-id="c177c-120">Update channel</span></span>](../api/channel-patch.md) | [<span data-ttu-id="c177c-121">チャネル</span><span class="sxs-lookup"><span data-stu-id="c177c-121">channel</span></span>](channel.md) | <span data-ttu-id="c177c-122">チャネルのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c177c-122">Update properties of the channel.</span></span>|
|[<span data-ttu-id="c177c-123">チャネルを削除します。</span><span class="sxs-lookup"><span data-stu-id="c177c-123">Delete channel</span></span>](../api/channel-delete.md) | <span data-ttu-id="c177c-124">なし</span><span class="sxs-lookup"><span data-stu-id="c177c-124">None</span></span> | <span data-ttu-id="c177c-125">チャネルを削除します。</span><span class="sxs-lookup"><span data-stu-id="c177c-125">Delete a channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="c177c-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c177c-126">Properties</span></span>
| <span data-ttu-id="c177c-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c177c-127">Property</span></span>     | <span data-ttu-id="c177c-128">種類</span><span class="sxs-lookup"><span data-stu-id="c177c-128">Type</span></span>   |<span data-ttu-id="c177c-129">説明</span><span class="sxs-lookup"><span data-stu-id="c177c-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c177c-130">説明</span><span class="sxs-lookup"><span data-stu-id="c177c-130">description</span></span>|<span data-ttu-id="c177c-131">String</span><span class="sxs-lookup"><span data-stu-id="c177c-131">String</span></span>|<span data-ttu-id="c177c-132">チャネルの省略可能な説明です。</span><span class="sxs-lookup"><span data-stu-id="c177c-132">Optional textual description for the channel.</span></span>|
|<span data-ttu-id="c177c-133">displayName</span><span class="sxs-lookup"><span data-stu-id="c177c-133">displayName</span></span>|<span data-ttu-id="c177c-134">String</span><span class="sxs-lookup"><span data-stu-id="c177c-134">String</span></span>|<span data-ttu-id="c177c-135">チャネルの名前は、マイクロソフトのチーム内のユーザーに表示されます。</span><span class="sxs-lookup"><span data-stu-id="c177c-135">Channel name as it will appear to the user in Microsoft Teams.</span></span>|
|<span data-ttu-id="c177c-136">id</span><span class="sxs-lookup"><span data-stu-id="c177c-136">id</span></span>|<span data-ttu-id="c177c-137">String</span><span class="sxs-lookup"><span data-stu-id="c177c-137">String</span></span>|<span data-ttu-id="c177c-138">チャネルの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="c177c-138">The channels's unique identifier.</span></span> <span data-ttu-id="c177c-139">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c177c-139">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c177c-140">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c177c-140">Relationships</span></span>
| <span data-ttu-id="c177c-141">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c177c-141">Relationship</span></span> | <span data-ttu-id="c177c-142">型</span><span class="sxs-lookup"><span data-stu-id="c177c-142">Type</span></span>   |<span data-ttu-id="c177c-143">説明</span><span class="sxs-lookup"><span data-stu-id="c177c-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c177c-144">タブ</span><span class="sxs-lookup"><span data-stu-id="c177c-144">tabs</span></span>|<span data-ttu-id="c177c-145">[teamsTab](../resources/teamstab.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="c177c-145">[teamsTab](../resources/teamstab.md) collection</span></span>|<span data-ttu-id="c177c-146">チャネル内のすべてのタブのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="c177c-146">A collection of all the tabs in the channel.</span></span> <span data-ttu-id="c177c-147">ナビゲーション プロパティです。</span><span class="sxs-lookup"><span data-stu-id="c177c-147">A navigation property.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="c177c-148">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c177c-148">JSON representation</span></span>

<span data-ttu-id="c177c-149">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="c177c-149">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "chatthreads"
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
<!-- {
  "type": "#page.annotation",
  "description": "channel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
