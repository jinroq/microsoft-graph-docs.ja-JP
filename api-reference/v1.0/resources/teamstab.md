---
title: teamsTab リソースの種類
description: 'タブでは、teamsTab をチーム内でのチャネル (接続) を固定しました。 '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 181d2fd23ff922709b3e098f6069adf300ad3928
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574671"
---
# <a name="teamstab-resource-type"></a><span data-ttu-id="180c4-103">teamsTab リソースの種類</span><span class="sxs-lookup"><span data-stu-id="180c4-103">teamsTab resource type</span></span>



<span data-ttu-id="180c4-104">[] タブ](../resources/teamstab.md)では、teamsTab を[チーム](team.md)内での[チャネル](channel.md)(接続) を固定しました。</span><span class="sxs-lookup"><span data-stu-id="180c4-104">A teamsTab is a [tab](../resources/teamstab.md) that's pinned (attached) to a [channel](channel.md) within a [team](team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="180c4-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="180c4-105">Methods</span></span>

| <span data-ttu-id="180c4-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="180c4-106">Method</span></span>       | <span data-ttu-id="180c4-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="180c4-107">Return Type</span></span>  |<span data-ttu-id="180c4-108">説明</span><span class="sxs-lookup"><span data-stu-id="180c4-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="180c4-109">[一覧] タブ](../api/teamstab-list.md)</span><span class="sxs-lookup"><span data-stu-id="180c4-109">[List tabs](../api/teamstab-list.md)</span></span> | [<span data-ttu-id="180c4-110">teamsTab</span><span class="sxs-lookup"><span data-stu-id="180c4-110">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="180c4-111">リスト タブは、チャンネルに固定します。</span><span class="sxs-lookup"><span data-stu-id="180c4-111">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="180c4-112">タブを取得します。</span><span class="sxs-lookup"><span data-stu-id="180c4-112">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="180c4-113">teamsTab</span><span class="sxs-lookup"><span data-stu-id="180c4-113">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="180c4-114">チャンネルに固定されているタブを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="180c4-114">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="180c4-115">タブを追加します。</span><span class="sxs-lookup"><span data-stu-id="180c4-115">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="180c4-116">teamsTab</span><span class="sxs-lookup"><span data-stu-id="180c4-116">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="180c4-117">(ピン) を追加するチャンネルをタブします。</span><span class="sxs-lookup"><span data-stu-id="180c4-117">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="180c4-118">タブを削除します。</span><span class="sxs-lookup"><span data-stu-id="180c4-118">Remove tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="180c4-119">なし</span><span class="sxs-lookup"><span data-stu-id="180c4-119">None</span></span> | <span data-ttu-id="180c4-120">削除 (固定解除) チャネルからタブします。</span><span class="sxs-lookup"><span data-stu-id="180c4-120">Removes (unpins) a tab from a channel.</span></span>|
|<span data-ttu-id="180c4-121">[[更新] タブ](../api/teamstab-update.md)</span><span class="sxs-lookup"><span data-stu-id="180c4-121">[Update tab](../api/teamstab-update.md)</span></span> | [<span data-ttu-id="180c4-122">teamsTab</span><span class="sxs-lookup"><span data-stu-id="180c4-122">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="180c4-123">タブのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="180c4-123">Updates the tab properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="180c4-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="180c4-124">Properties</span></span>

|<span data-ttu-id="180c4-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="180c4-125">Property</span></span>|<span data-ttu-id="180c4-126">型</span><span class="sxs-lookup"><span data-stu-id="180c4-126">Type</span></span>|<span data-ttu-id="180c4-127">説明</span><span class="sxs-lookup"><span data-stu-id="180c4-127">Description</span></span>|
|:---------------|:--------|:----------|
|  <span data-ttu-id="180c4-128">id</span><span class="sxs-lookup"><span data-stu-id="180c4-128">id</span></span>              |   <span data-ttu-id="180c4-129">文字列</span><span class="sxs-lookup"><span data-stu-id="180c4-129">string</span></span>                  |  <span data-ttu-id="180c4-130">チャネル タブ読み取りのみの特定のインスタンスを一意に識別する識別子です。</span><span class="sxs-lookup"><span data-stu-id="180c4-130">Identifier that uniquely identifies a specific instance of a channel tab. Read only.</span></span>     |
|  <span data-ttu-id="180c4-131">displayName</span><span class="sxs-lookup"><span data-stu-id="180c4-131">displayName</span></span>            |   <span data-ttu-id="180c4-132">string</span><span class="sxs-lookup"><span data-stu-id="180c4-132">string</span></span>                  |  <span data-ttu-id="180c4-133">タブの名前です。</span><span class="sxs-lookup"><span data-stu-id="180c4-133">Name of the tab.</span></span>     |
|  <span data-ttu-id="180c4-134">webUrl</span><span class="sxs-lookup"><span data-stu-id="180c4-134">webUrl</span></span>          |   <span data-ttu-id="180c4-135">文字列</span><span class="sxs-lookup"><span data-stu-id="180c4-135">string</span></span>                  |  <span data-ttu-id="180c4-136">タブのインスタンスの高度なリンクの url です。</span><span class="sxs-lookup"><span data-stu-id="180c4-136">Deep link url of the tab instance.</span></span> <span data-ttu-id="180c4-137">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="180c4-137">Read only.</span></span>     |
|  <span data-ttu-id="180c4-138">configuration</span><span class="sxs-lookup"><span data-stu-id="180c4-138">configuration</span></span>        |   [<span data-ttu-id="180c4-139">teamsTabConfiguration</span><span class="sxs-lookup"><span data-stu-id="180c4-139">teamsTabConfiguration</span></span>](teamstabconfiguration.md) |  <span data-ttu-id="180c4-140">タブに適用するカスタム設定のコンテナーです。タブでは、このプロパティが 1 回だけが構成されていると見なされます。</span><span class="sxs-lookup"><span data-stu-id="180c4-140">Container for custom settings applied to a tab. The tab is considered configured only once this property is set.</span></span>     |

## <a name="relationships"></a><span data-ttu-id="180c4-141">関係</span><span class="sxs-lookup"><span data-stu-id="180c4-141">Relationships</span></span>

| <span data-ttu-id="180c4-142">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="180c4-142">Relationship</span></span> | <span data-ttu-id="180c4-143">型</span><span class="sxs-lookup"><span data-stu-id="180c4-143">Type</span></span>   | <span data-ttu-id="180c4-144">説明</span><span class="sxs-lookup"><span data-stu-id="180c4-144">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="180c4-145">teamsApp</span><span class="sxs-lookup"><span data-stu-id="180c4-145">teamsApp</span></span>|[<span data-ttu-id="180c4-146">teamsApp</span><span class="sxs-lookup"><span data-stu-id="180c4-146">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="180c4-147">タブにリンクされているアプリケーションです。タブを作成した後は、これを変更できません。</span><span class="sxs-lookup"><span data-stu-id="180c4-147">The application that is linked to the tab. This cannot be changed after tab creation.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="180c4-148">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="180c4-148">JSON representation</span></span>

<span data-ttu-id="180c4-149">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="180c4-149">The following is a JSON representation of the resource.</span></span>


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

## <a name="see-also"></a><span data-ttu-id="180c4-150">関連項目</span><span class="sxs-lookup"><span data-stu-id="180c4-150">See also</span></span>

[<span data-ttu-id="180c4-151">組み込みタブのタイプを設定します。</span><span class="sxs-lookup"><span data-stu-id="180c4-151">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)
