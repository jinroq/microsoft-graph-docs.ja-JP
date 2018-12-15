---
title: teamsTab リソースの種類
description: 'タブでは、teamsTab をチーム内でのチャネル (接続) を固定しました。 '
ms.openlocfilehash: 102d4c0b766d8a0d9bdf22cb2ed76f5e06d87ad5
ms.sourcegitcommit: f3d479edf03935d0edbbc7668a65f7cde2a56c92
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/15/2018
ms.locfileid: "27283620"
---
# <a name="teamstab-resource-type"></a><span data-ttu-id="200c0-103">teamsTab リソースの種類</span><span class="sxs-lookup"><span data-stu-id="200c0-103">teamsTab resource type</span></span>

> <span data-ttu-id="200c0-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="200c0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="200c0-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="200c0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="200c0-106">[] タブ](../resources/teamstab.md)では、teamsTab を[チーム](team.md)内での[チャネル](channel.md)(接続) を固定しました。</span><span class="sxs-lookup"><span data-stu-id="200c0-106">A teamsTab is a [tab](../resources/teamstab.md) that's pinned (attached) to a [channel](channel.md) within a [team](team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="200c0-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="200c0-107">Methods</span></span>

| <span data-ttu-id="200c0-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="200c0-108">Method</span></span>       | <span data-ttu-id="200c0-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="200c0-109">Return Type</span></span>  |<span data-ttu-id="200c0-110">説明</span><span class="sxs-lookup"><span data-stu-id="200c0-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="200c0-111">[一覧] タブ](../api/teamstab-list.md)</span><span class="sxs-lookup"><span data-stu-id="200c0-111">[List tabs](../api/teamstab-list.md)</span></span> | [<span data-ttu-id="200c0-112">teamsTab</span><span class="sxs-lookup"><span data-stu-id="200c0-112">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="200c0-113">リスト タブは、チャンネルに固定します。</span><span class="sxs-lookup"><span data-stu-id="200c0-113">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="200c0-114">タブを取得します。</span><span class="sxs-lookup"><span data-stu-id="200c0-114">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="200c0-115">teamsTab</span><span class="sxs-lookup"><span data-stu-id="200c0-115">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="200c0-116">チャンネルに固定されているタブを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="200c0-116">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="200c0-117">タブを追加します。</span><span class="sxs-lookup"><span data-stu-id="200c0-117">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="200c0-118">teamsTab</span><span class="sxs-lookup"><span data-stu-id="200c0-118">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="200c0-119">(ピン) を追加するチャンネルをタブします。</span><span class="sxs-lookup"><span data-stu-id="200c0-119">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="200c0-120">タブを削除します。</span><span class="sxs-lookup"><span data-stu-id="200c0-120">Remove tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="200c0-121">なし</span><span class="sxs-lookup"><span data-stu-id="200c0-121">None</span></span> | <span data-ttu-id="200c0-122">削除 (固定解除) チャネルからタブします。</span><span class="sxs-lookup"><span data-stu-id="200c0-122">Removes (unpins) a tab from a channel.</span></span>|
|<span data-ttu-id="200c0-123">[[更新] タブ](../api/teamstab-update.md)</span><span class="sxs-lookup"><span data-stu-id="200c0-123">[Update tab](../api/teamstab-update.md)</span></span> | [<span data-ttu-id="200c0-124">teamsTab</span><span class="sxs-lookup"><span data-stu-id="200c0-124">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="200c0-125">タブのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="200c0-125">Updates the tab properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="200c0-126">Properties</span><span class="sxs-lookup"><span data-stu-id="200c0-126">Properties</span></span>

|<span data-ttu-id="200c0-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="200c0-127">Property</span></span>|<span data-ttu-id="200c0-128">種類</span><span class="sxs-lookup"><span data-stu-id="200c0-128">Type</span></span>|<span data-ttu-id="200c0-129">説明</span><span class="sxs-lookup"><span data-stu-id="200c0-129">Description</span></span>|
|:---------------|:--------|:----------|
|  <span data-ttu-id="200c0-130">ID</span><span class="sxs-lookup"><span data-stu-id="200c0-130">id</span></span>              |   <span data-ttu-id="200c0-131">string</span><span class="sxs-lookup"><span data-stu-id="200c0-131">string</span></span>                  |  <span data-ttu-id="200c0-132">チャネル タブ読み取りのみの特定のインスタンスを一意に識別する識別子です。</span><span class="sxs-lookup"><span data-stu-id="200c0-132">Identifier that uniquely identifies a specific instance of a channel tab. Read only.</span></span>     |
|  <span data-ttu-id="200c0-133">displayName</span><span class="sxs-lookup"><span data-stu-id="200c0-133">displayName</span></span>            |   <span data-ttu-id="200c0-134">string</span><span class="sxs-lookup"><span data-stu-id="200c0-134">string</span></span>                  |  <span data-ttu-id="200c0-135">タブの名前です。</span><span class="sxs-lookup"><span data-stu-id="200c0-135">Name of the tab.</span></span>     |
|  <span data-ttu-id="200c0-136">name</span><span class="sxs-lookup"><span data-stu-id="200c0-136">name</span></span>            |   <span data-ttu-id="200c0-137">文字列</span><span class="sxs-lookup"><span data-stu-id="200c0-137">string</span></span>                  |  <span data-ttu-id="200c0-138">(非推奨)タブの名前です。</span><span class="sxs-lookup"><span data-stu-id="200c0-138">(Deprecated) Name of the tab.</span></span>     |
|  <span data-ttu-id="200c0-139">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="200c0-139">teamsAppId</span></span>           |   <span data-ttu-id="200c0-140">string</span><span class="sxs-lookup"><span data-stu-id="200c0-140">string</span></span>             |  <span data-ttu-id="200c0-141">タブのアプリケーション定義の識別子です。タブを作成した後は、この値を変更できません。</span><span class="sxs-lookup"><span data-stu-id="200c0-141">App definition identifier of the tab. This value cannot be changed after tab creation.</span></span>     |
|  <span data-ttu-id="200c0-142">sortOrderIndex</span><span class="sxs-lookup"><span data-stu-id="200c0-142">sortOrderIndex</span></span>  |   <span data-ttu-id="200c0-143">int</span><span class="sxs-lookup"><span data-stu-id="200c0-143">int</span></span>                     |  <span data-ttu-id="200c0-144">タブの並べ替え順序のインデックス。</span><span class="sxs-lookup"><span data-stu-id="200c0-144">Index of the order used for sorting tabs.</span></span>     |
|  <span data-ttu-id="200c0-145">webUrl</span><span class="sxs-lookup"><span data-stu-id="200c0-145">webUrl</span></span>          |   <span data-ttu-id="200c0-146">string</span><span class="sxs-lookup"><span data-stu-id="200c0-146">string</span></span>                  |  <span data-ttu-id="200c0-147">タブのインスタンスの高度なリンクの url です。</span><span class="sxs-lookup"><span data-stu-id="200c0-147">Deep link url of the tab instance.</span></span> <span data-ttu-id="200c0-148">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="200c0-148">Read only.</span></span>     |
|  <span data-ttu-id="200c0-149">configuration</span><span class="sxs-lookup"><span data-stu-id="200c0-149">configuration</span></span>        |   [<span data-ttu-id="200c0-150">teamsTabConfiguration</span><span class="sxs-lookup"><span data-stu-id="200c0-150">teamsTabConfiguration</span></span>](teamstabconfiguration.md) |  <span data-ttu-id="200c0-151">タブに適用するカスタム設定のコンテナーです。タブでは、このプロパティが 1 回だけが構成されていると見なされます。</span><span class="sxs-lookup"><span data-stu-id="200c0-151">Container for custom settings applied to a tab. The tab is considered configured only once this property is set.</span></span>     |

## <a name="relationships"></a><span data-ttu-id="200c0-152">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="200c0-152">Relationships</span></span>

| <span data-ttu-id="200c0-153">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="200c0-153">Relationship</span></span> | <span data-ttu-id="200c0-154">型</span><span class="sxs-lookup"><span data-stu-id="200c0-154">Type</span></span>   | <span data-ttu-id="200c0-155">説明</span><span class="sxs-lookup"><span data-stu-id="200c0-155">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="200c0-156">teamsApp</span><span class="sxs-lookup"><span data-stu-id="200c0-156">teamsApp</span></span>|[<span data-ttu-id="200c0-157">teamsApp</span><span class="sxs-lookup"><span data-stu-id="200c0-157">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="200c0-158">タブにリンクされているアプリケーションです。</span><span class="sxs-lookup"><span data-stu-id="200c0-158">The application that is linked to the tab.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="200c0-159">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="200c0-159">JSON representation</span></span>

<span data-ttu-id="200c0-160">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="200c0-160">The following is a JSON representation of the resource.</span></span>


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

## <a name="see-also"></a><span data-ttu-id="200c0-161">関連項目</span><span class="sxs-lookup"><span data-stu-id="200c0-161">See also</span></span>

[<span data-ttu-id="200c0-162">組み込みタブのタイプを設定します。</span><span class="sxs-lookup"><span data-stu-id="200c0-162">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)
