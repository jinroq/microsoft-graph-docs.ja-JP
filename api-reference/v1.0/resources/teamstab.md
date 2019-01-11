---
title: teamsTab リソースの種類
description: 'タブでは、teamsTab をチーム内でのチャネル (接続) を固定しました。 '
localization_priority: Normal
ms.openlocfilehash: a1c3302251ac9b68be1cd8d6a011b7e0a7d216b1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860845"
---
# <a name="teamstab-resource-type"></a><span data-ttu-id="683bb-103">teamsTab リソースの種類</span><span class="sxs-lookup"><span data-stu-id="683bb-103">teamsTab resource type</span></span>



<span data-ttu-id="683bb-104">[] タブ](../resources/teamstab.md)では、teamsTab を[チーム](team.md)内での[チャネル](channel.md)(接続) を固定しました。</span><span class="sxs-lookup"><span data-stu-id="683bb-104">A teamsTab is a [tab](../resources/teamstab.md) that's pinned (attached) to a [channel](channel.md) within a [team](team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="683bb-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="683bb-105">Methods</span></span>

| <span data-ttu-id="683bb-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="683bb-106">Method</span></span>       | <span data-ttu-id="683bb-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="683bb-107">Return Type</span></span>  |<span data-ttu-id="683bb-108">説明</span><span class="sxs-lookup"><span data-stu-id="683bb-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="683bb-109">[一覧] タブ](../api/teamstab-list.md)</span><span class="sxs-lookup"><span data-stu-id="683bb-109">[List tabs](../api/teamstab-list.md)</span></span> | [<span data-ttu-id="683bb-110">teamsTab</span><span class="sxs-lookup"><span data-stu-id="683bb-110">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="683bb-111">リスト タブは、チャンネルに固定します。</span><span class="sxs-lookup"><span data-stu-id="683bb-111">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="683bb-112">タブを取得します。</span><span class="sxs-lookup"><span data-stu-id="683bb-112">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="683bb-113">teamsTab</span><span class="sxs-lookup"><span data-stu-id="683bb-113">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="683bb-114">チャンネルに固定されているタブを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="683bb-114">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="683bb-115">タブを追加します。</span><span class="sxs-lookup"><span data-stu-id="683bb-115">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="683bb-116">teamsTab</span><span class="sxs-lookup"><span data-stu-id="683bb-116">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="683bb-117">(ピン) を追加するチャンネルをタブします。</span><span class="sxs-lookup"><span data-stu-id="683bb-117">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="683bb-118">タブを削除します。</span><span class="sxs-lookup"><span data-stu-id="683bb-118">Remove tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="683bb-119">なし</span><span class="sxs-lookup"><span data-stu-id="683bb-119">None</span></span> | <span data-ttu-id="683bb-120">削除 (固定解除) チャネルからタブします。</span><span class="sxs-lookup"><span data-stu-id="683bb-120">Removes (unpins) a tab from a channel.</span></span>|
|<span data-ttu-id="683bb-121">[[更新] タブ](../api/teamstab-update.md)</span><span class="sxs-lookup"><span data-stu-id="683bb-121">[Update tab](../api/teamstab-update.md)</span></span> | [<span data-ttu-id="683bb-122">teamsTab</span><span class="sxs-lookup"><span data-stu-id="683bb-122">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="683bb-123">タブのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="683bb-123">Updates the tab properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="683bb-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="683bb-124">Properties</span></span>

|<span data-ttu-id="683bb-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="683bb-125">Property</span></span>|<span data-ttu-id="683bb-126">種類</span><span class="sxs-lookup"><span data-stu-id="683bb-126">Type</span></span>|<span data-ttu-id="683bb-127">説明</span><span class="sxs-lookup"><span data-stu-id="683bb-127">Description</span></span>|
|:---------------|:--------|:----------|
|  <span data-ttu-id="683bb-128">ID</span><span class="sxs-lookup"><span data-stu-id="683bb-128">id</span></span>              |   <span data-ttu-id="683bb-129">文字列</span><span class="sxs-lookup"><span data-stu-id="683bb-129">string</span></span>                  |  <span data-ttu-id="683bb-130">チャネル タブ読み取りのみの特定のインスタンスを一意に識別する識別子です。</span><span class="sxs-lookup"><span data-stu-id="683bb-130">Identifier that uniquely identifies a specific instance of a channel tab. Read only.</span></span>     |
|  <span data-ttu-id="683bb-131">displayName</span><span class="sxs-lookup"><span data-stu-id="683bb-131">displayName</span></span>            |   <span data-ttu-id="683bb-132">string</span><span class="sxs-lookup"><span data-stu-id="683bb-132">string</span></span>                  |  <span data-ttu-id="683bb-133">タブの名前です。</span><span class="sxs-lookup"><span data-stu-id="683bb-133">Name of the tab.</span></span>     |
|  <span data-ttu-id="683bb-134">sortOrderIndex</span><span class="sxs-lookup"><span data-stu-id="683bb-134">sortOrderIndex</span></span>  |   <span data-ttu-id="683bb-135">int</span><span class="sxs-lookup"><span data-stu-id="683bb-135">int</span></span>                     |  <span data-ttu-id="683bb-136">タブの並べ替え順序のインデックス</span><span class="sxs-lookup"><span data-stu-id="683bb-136">Index of the order used for sorting tabs</span></span>     |
|  <span data-ttu-id="683bb-137">webUrl</span><span class="sxs-lookup"><span data-stu-id="683bb-137">webUrl</span></span>          |   <span data-ttu-id="683bb-138">文字列</span><span class="sxs-lookup"><span data-stu-id="683bb-138">string</span></span>                  |  <span data-ttu-id="683bb-139">タブのインスタンスの高度なリンクの url です。</span><span class="sxs-lookup"><span data-stu-id="683bb-139">Deep link url of the tab instance.</span></span> <span data-ttu-id="683bb-140">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="683bb-140">Read only.</span></span>     |
|  <span data-ttu-id="683bb-141">configuration</span><span class="sxs-lookup"><span data-stu-id="683bb-141">configuration</span></span>        |   [<span data-ttu-id="683bb-142">teamsTabConfiguration</span><span class="sxs-lookup"><span data-stu-id="683bb-142">teamsTabConfiguration</span></span>](teamstabconfiguration.md) |  <span data-ttu-id="683bb-143">タブに適用するカスタム設定のコンテナーです。タブでは、このプロパティが 1 回だけが構成されていると見なされます。</span><span class="sxs-lookup"><span data-stu-id="683bb-143">Container for custom settings applied to a tab. The tab is considered configured only once this property is set.</span></span>     |

## <a name="relationships"></a><span data-ttu-id="683bb-144">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="683bb-144">Relationships</span></span>

| <span data-ttu-id="683bb-145">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="683bb-145">Relationship</span></span> | <span data-ttu-id="683bb-146">型</span><span class="sxs-lookup"><span data-stu-id="683bb-146">Type</span></span>   | <span data-ttu-id="683bb-147">説明</span><span class="sxs-lookup"><span data-stu-id="683bb-147">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="683bb-148">teamsApp</span><span class="sxs-lookup"><span data-stu-id="683bb-148">teamsApp</span></span>|[<span data-ttu-id="683bb-149">teamsApp</span><span class="sxs-lookup"><span data-stu-id="683bb-149">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="683bb-150">タブにリンクされているアプリケーションです。タブを作成した後は、これを変更できません。</span><span class="sxs-lookup"><span data-stu-id="683bb-150">The application that is linked to the tab. This cannot be changed after tab creation.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="683bb-151">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="683bb-151">JSON representation</span></span>

<span data-ttu-id="683bb-152">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="683bb-152">The following is a JSON representation of the resource.</span></span>


<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.teamsTab"
}-->

```json
{  
  "id": "string",
  "displayName": "string",
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

## <a name="see-also"></a><span data-ttu-id="683bb-153">関連項目</span><span class="sxs-lookup"><span data-stu-id="683bb-153">See also</span></span>

[<span data-ttu-id="683bb-154">組み込みタブのタイプを設定します。</span><span class="sxs-lookup"><span data-stu-id="683bb-154">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)
