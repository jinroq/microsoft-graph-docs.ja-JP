---
title: teamsTab リソースの種類
description: 'TeamsTab は、チーム内のチャネルに固定 (接続) されたタブです。 '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: bf07770d920ee05c7856f89e2e099bcc958ad50c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033692"
---
# <a name="teamstab-resource-type"></a><span data-ttu-id="cbceb-103">teamsTab リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cbceb-103">teamsTab resource type</span></span>



<span data-ttu-id="cbceb-104">TeamsTab は、[チーム](team.md)内の[チャネル](channel.md)に固定 (接続) された[タブ](../resources/teamstab.md)です。</span><span class="sxs-lookup"><span data-stu-id="cbceb-104">A teamsTab is a [tab](../resources/teamstab.md) that's pinned (attached) to a [channel](channel.md) within a [team](team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="cbceb-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="cbceb-105">Methods</span></span>

| <span data-ttu-id="cbceb-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="cbceb-106">Method</span></span>       | <span data-ttu-id="cbceb-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="cbceb-107">Return Type</span></span>  |<span data-ttu-id="cbceb-108">説明</span><span class="sxs-lookup"><span data-stu-id="cbceb-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cbceb-109">タブを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="cbceb-109">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="cbceb-110">teamsTab</span><span class="sxs-lookup"><span data-stu-id="cbceb-110">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="cbceb-111">チャネルにピン留めされているタブを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="cbceb-111">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="cbceb-112">タブを取得する</span><span class="sxs-lookup"><span data-stu-id="cbceb-112">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="cbceb-113">teamsTab</span><span class="sxs-lookup"><span data-stu-id="cbceb-113">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="cbceb-114">チャネルにピン留めされているタブを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="cbceb-114">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="cbceb-115">タブを追加する</span><span class="sxs-lookup"><span data-stu-id="cbceb-115">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="cbceb-116">teamsTab</span><span class="sxs-lookup"><span data-stu-id="cbceb-116">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="cbceb-117">タブをチャネルに追加 (ピン留め) します。</span><span class="sxs-lookup"><span data-stu-id="cbceb-117">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="cbceb-118">タブを削除する</span><span class="sxs-lookup"><span data-stu-id="cbceb-118">Remove tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="cbceb-119">なし</span><span class="sxs-lookup"><span data-stu-id="cbceb-119">None</span></span> | <span data-ttu-id="cbceb-120">チャネルからタブを削除します (ピン留めを外します)。</span><span class="sxs-lookup"><span data-stu-id="cbceb-120">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="cbceb-121">タブを更新する</span><span class="sxs-lookup"><span data-stu-id="cbceb-121">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="cbceb-122">teamsTab</span><span class="sxs-lookup"><span data-stu-id="cbceb-122">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="cbceb-123">タブのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="cbceb-123">Updates the tab properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="cbceb-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cbceb-124">Properties</span></span>

|<span data-ttu-id="cbceb-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cbceb-125">Property</span></span>|<span data-ttu-id="cbceb-126">型</span><span class="sxs-lookup"><span data-stu-id="cbceb-126">Type</span></span>|<span data-ttu-id="cbceb-127">説明</span><span class="sxs-lookup"><span data-stu-id="cbceb-127">Description</span></span>|
|:---------------|:--------|:----------|
|  <span data-ttu-id="cbceb-128">id</span><span class="sxs-lookup"><span data-stu-id="cbceb-128">id</span></span>              |   <span data-ttu-id="cbceb-129">string</span><span class="sxs-lookup"><span data-stu-id="cbceb-129">string</span></span>                  |  <span data-ttu-id="cbceb-130">チャネルタブの特定のインスタンスを一意に識別する識別子。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="cbceb-130">Identifier that uniquely identifies a specific instance of a channel tab. Read only.</span></span>     |
|  <span data-ttu-id="cbceb-131">displayName</span><span class="sxs-lookup"><span data-stu-id="cbceb-131">displayName</span></span>            |   <span data-ttu-id="cbceb-132">string</span><span class="sxs-lookup"><span data-stu-id="cbceb-132">string</span></span>                  |  <span data-ttu-id="cbceb-133">タブの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="cbceb-133">Name of the tab.</span></span>     |
|  <span data-ttu-id="cbceb-134">webUrl</span><span class="sxs-lookup"><span data-stu-id="cbceb-134">webUrl</span></span>          |   <span data-ttu-id="cbceb-135">string</span><span class="sxs-lookup"><span data-stu-id="cbceb-135">string</span></span>                  |  <span data-ttu-id="cbceb-136">Tab インスタンスのディープリンク url。</span><span class="sxs-lookup"><span data-stu-id="cbceb-136">Deep link url of the tab instance.</span></span> <span data-ttu-id="cbceb-137">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cbceb-137">Read only.</span></span>     |
|  <span data-ttu-id="cbceb-138">環境</span><span class="sxs-lookup"><span data-stu-id="cbceb-138">configuration</span></span>        |   [<span data-ttu-id="cbceb-139">teamsTabConfiguration</span><span class="sxs-lookup"><span data-stu-id="cbceb-139">teamsTabConfiguration</span></span>](teamstabconfiguration.md) |  <span data-ttu-id="cbceb-140">タブに適用されるカスタム設定のコンテナーです。このプロパティが設定されると、タブは構成されたことを示します。</span><span class="sxs-lookup"><span data-stu-id="cbceb-140">Container for custom settings applied to a tab. The tab is considered configured only once this property is set.</span></span>     |

## <a name="relationships"></a><span data-ttu-id="cbceb-141">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="cbceb-141">Relationships</span></span>

| <span data-ttu-id="cbceb-142">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="cbceb-142">Relationship</span></span> | <span data-ttu-id="cbceb-143">型</span><span class="sxs-lookup"><span data-stu-id="cbceb-143">Type</span></span>   | <span data-ttu-id="cbceb-144">説明</span><span class="sxs-lookup"><span data-stu-id="cbceb-144">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="cbceb-145">teamsApp</span><span class="sxs-lookup"><span data-stu-id="cbceb-145">teamsApp</span></span>|[<span data-ttu-id="cbceb-146">teamsApp</span><span class="sxs-lookup"><span data-stu-id="cbceb-146">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="cbceb-147">タブにリンクされているアプリケーション。これは、タブの作成後に変更することはできません。</span><span class="sxs-lookup"><span data-stu-id="cbceb-147">The application that is linked to the tab. This cannot be changed after tab creation.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="cbceb-148">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cbceb-148">JSON representation</span></span>

<span data-ttu-id="cbceb-149">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cbceb-149">The following is a JSON representation of the resource.</span></span>


<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.teamsTab"
}-->

```json
{  
  "id": "string",
  "displayName": "string",
  "webUrl": "string",
  "configuration" : "teamsTabConfiguration"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsTab resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

## <a name="see-also"></a><span data-ttu-id="cbceb-150">関連項目</span><span class="sxs-lookup"><span data-stu-id="cbceb-150">See also</span></span>

[<span data-ttu-id="cbceb-151">組み込みタブ タイプの構成</span><span class="sxs-lookup"><span data-stu-id="cbceb-151">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)
