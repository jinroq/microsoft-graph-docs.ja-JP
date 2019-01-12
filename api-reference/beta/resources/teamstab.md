---
title: teamsTab リソースの種類
description: 'タブでは、teamsTab をチーム内でのチャネル (接続) を固定しました。 '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 3c5cf5ef33f53cfaca7189df24e5dfd880a77241
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947149"
---
# <a name="teamstab-resource-type"></a><span data-ttu-id="60fe4-103">teamsTab リソースの種類</span><span class="sxs-lookup"><span data-stu-id="60fe4-103">teamsTab resource type</span></span>

> <span data-ttu-id="60fe4-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="60fe4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="60fe4-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="60fe4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="60fe4-106">[] タブ](../resources/teamstab.md)では、teamsTab を[チーム](team.md)内での[チャネル](channel.md)(接続) を固定しました。</span><span class="sxs-lookup"><span data-stu-id="60fe4-106">A teamsTab is a [tab](../resources/teamstab.md) that's pinned (attached) to a [channel](channel.md) within a [team](team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="60fe4-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="60fe4-107">Methods</span></span>

| <span data-ttu-id="60fe4-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="60fe4-108">Method</span></span>       | <span data-ttu-id="60fe4-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="60fe4-109">Return Type</span></span>  |<span data-ttu-id="60fe4-110">説明</span><span class="sxs-lookup"><span data-stu-id="60fe4-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="60fe4-111">[一覧] タブ](../api/teamstab-list.md)</span><span class="sxs-lookup"><span data-stu-id="60fe4-111">[List tabs](../api/teamstab-list.md)</span></span> | [<span data-ttu-id="60fe4-112">teamsTab</span><span class="sxs-lookup"><span data-stu-id="60fe4-112">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="60fe4-113">リスト タブは、チャンネルに固定します。</span><span class="sxs-lookup"><span data-stu-id="60fe4-113">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="60fe4-114">タブを取得します。</span><span class="sxs-lookup"><span data-stu-id="60fe4-114">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="60fe4-115">teamsTab</span><span class="sxs-lookup"><span data-stu-id="60fe4-115">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="60fe4-116">チャンネルに固定されているタブを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="60fe4-116">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="60fe4-117">タブを追加します。</span><span class="sxs-lookup"><span data-stu-id="60fe4-117">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="60fe4-118">teamsTab</span><span class="sxs-lookup"><span data-stu-id="60fe4-118">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="60fe4-119">(ピン) を追加するチャンネルをタブします。</span><span class="sxs-lookup"><span data-stu-id="60fe4-119">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="60fe4-120">タブを削除します。</span><span class="sxs-lookup"><span data-stu-id="60fe4-120">Remove tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="60fe4-121">なし</span><span class="sxs-lookup"><span data-stu-id="60fe4-121">None</span></span> | <span data-ttu-id="60fe4-122">削除 (固定解除) チャネルからタブします。</span><span class="sxs-lookup"><span data-stu-id="60fe4-122">Removes (unpins) a tab from a channel.</span></span>|
|<span data-ttu-id="60fe4-123">[[更新] タブ](../api/teamstab-update.md)</span><span class="sxs-lookup"><span data-stu-id="60fe4-123">[Update tab](../api/teamstab-update.md)</span></span> | [<span data-ttu-id="60fe4-124">teamsTab</span><span class="sxs-lookup"><span data-stu-id="60fe4-124">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="60fe4-125">タブのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="60fe4-125">Updates the tab properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="60fe4-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="60fe4-126">Properties</span></span>

|<span data-ttu-id="60fe4-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="60fe4-127">Property</span></span>|<span data-ttu-id="60fe4-128">種類</span><span class="sxs-lookup"><span data-stu-id="60fe4-128">Type</span></span>|<span data-ttu-id="60fe4-129">説明</span><span class="sxs-lookup"><span data-stu-id="60fe4-129">Description</span></span>|
|:---------------|:--------|:----------|
|  <span data-ttu-id="60fe4-130">ID</span><span class="sxs-lookup"><span data-stu-id="60fe4-130">id</span></span>              |   <span data-ttu-id="60fe4-131">文字列</span><span class="sxs-lookup"><span data-stu-id="60fe4-131">string</span></span>                  |  <span data-ttu-id="60fe4-132">チャネル タブ読み取りのみの特定のインスタンスを一意に識別する識別子です。</span><span class="sxs-lookup"><span data-stu-id="60fe4-132">Identifier that uniquely identifies a specific instance of a channel tab. Read only.</span></span>     |
|  <span data-ttu-id="60fe4-133">displayName</span><span class="sxs-lookup"><span data-stu-id="60fe4-133">displayName</span></span>            |   <span data-ttu-id="60fe4-134">string</span><span class="sxs-lookup"><span data-stu-id="60fe4-134">string</span></span>                  |  <span data-ttu-id="60fe4-135">タブの名前です。</span><span class="sxs-lookup"><span data-stu-id="60fe4-135">Name of the tab.</span></span>     |
|  <span data-ttu-id="60fe4-136">name</span><span class="sxs-lookup"><span data-stu-id="60fe4-136">name</span></span>            |   <span data-ttu-id="60fe4-137">文字列</span><span class="sxs-lookup"><span data-stu-id="60fe4-137">string</span></span>                  |  <span data-ttu-id="60fe4-138">(非推奨)タブの名前です。</span><span class="sxs-lookup"><span data-stu-id="60fe4-138">(Deprecated) Name of the tab.</span></span>     |
|  <span data-ttu-id="60fe4-139">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="60fe4-139">teamsAppId</span></span>           |   <span data-ttu-id="60fe4-140">文字列</span><span class="sxs-lookup"><span data-stu-id="60fe4-140">string</span></span>             |  <span data-ttu-id="60fe4-141">タブのアプリケーション定義の識別子です。タブを作成した後は、この値を変更できません。</span><span class="sxs-lookup"><span data-stu-id="60fe4-141">App definition identifier of the tab. This value cannot be changed after tab creation.</span></span>     |
|  <span data-ttu-id="60fe4-142">sortOrderIndex</span><span class="sxs-lookup"><span data-stu-id="60fe4-142">sortOrderIndex</span></span>  |   <span data-ttu-id="60fe4-143">int</span><span class="sxs-lookup"><span data-stu-id="60fe4-143">int</span></span>                     |  <span data-ttu-id="60fe4-144">タブの並べ替え順序のインデックス。</span><span class="sxs-lookup"><span data-stu-id="60fe4-144">Index of the order used for sorting tabs.</span></span>     |
|  <span data-ttu-id="60fe4-145">webUrl</span><span class="sxs-lookup"><span data-stu-id="60fe4-145">webUrl</span></span>          |   <span data-ttu-id="60fe4-146">文字列</span><span class="sxs-lookup"><span data-stu-id="60fe4-146">string</span></span>                  |  <span data-ttu-id="60fe4-147">タブのインスタンスの高度なリンクの url です。</span><span class="sxs-lookup"><span data-stu-id="60fe4-147">Deep link url of the tab instance.</span></span> <span data-ttu-id="60fe4-148">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="60fe4-148">Read only.</span></span>     |
|  <span data-ttu-id="60fe4-149">configuration</span><span class="sxs-lookup"><span data-stu-id="60fe4-149">configuration</span></span>        |   [<span data-ttu-id="60fe4-150">teamsTabConfiguration</span><span class="sxs-lookup"><span data-stu-id="60fe4-150">teamsTabConfiguration</span></span>](teamstabconfiguration.md) |  <span data-ttu-id="60fe4-151">タブに適用するカスタム設定のコンテナーです。タブでは、このプロパティが 1 回だけが構成されていると見なされます。</span><span class="sxs-lookup"><span data-stu-id="60fe4-151">Container for custom settings applied to a tab. The tab is considered configured only once this property is set.</span></span>     |

## <a name="relationships"></a><span data-ttu-id="60fe4-152">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="60fe4-152">Relationships</span></span>

| <span data-ttu-id="60fe4-153">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="60fe4-153">Relationship</span></span> | <span data-ttu-id="60fe4-154">型</span><span class="sxs-lookup"><span data-stu-id="60fe4-154">Type</span></span>   | <span data-ttu-id="60fe4-155">説明</span><span class="sxs-lookup"><span data-stu-id="60fe4-155">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="60fe4-156">teamsApp</span><span class="sxs-lookup"><span data-stu-id="60fe4-156">teamsApp</span></span>|[<span data-ttu-id="60fe4-157">teamsApp</span><span class="sxs-lookup"><span data-stu-id="60fe4-157">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="60fe4-158">タブにリンクされているアプリケーションです。</span><span class="sxs-lookup"><span data-stu-id="60fe4-158">The application that is linked to the tab.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="60fe4-159">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="60fe4-159">JSON representation</span></span>

<span data-ttu-id="60fe4-160">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="60fe4-160">The following is a JSON representation of the resource.</span></span>


<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.teamsTab"
}-->

```json
{  
  "id": "string",
  "displayName": "string",
  "teamsAppId": "string",
  "sortOrderIndex": "string",
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

## <a name="see-also"></a><span data-ttu-id="60fe4-161">関連項目</span><span class="sxs-lookup"><span data-stu-id="60fe4-161">See also</span></span>

[<span data-ttu-id="60fe4-162">組み込みタブのタイプを設定します。</span><span class="sxs-lookup"><span data-stu-id="60fe4-162">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)
