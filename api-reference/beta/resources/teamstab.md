---
title: teamsTab リソースの種類
description: 'タブでは、teamsTab をチーム内でのチャネル (接続) を固定しました。 '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 207b9d1d4d27199f07ae22bd47587411f917afae
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574951"
---
# <a name="teamstab-resource-type"></a><span data-ttu-id="a8460-103">teamsTab リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a8460-103">teamsTab resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8460-104">[] タブ](../resources/teamstab.md)では、teamsTab を[チーム](team.md)内での[チャネル](channel.md)(接続) を固定しました。</span><span class="sxs-lookup"><span data-stu-id="a8460-104">A teamsTab is a [tab](../resources/teamstab.md) that's pinned (attached) to a [channel](channel.md) within a [team](team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="a8460-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="a8460-105">Methods</span></span>

| <span data-ttu-id="a8460-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="a8460-106">Method</span></span>       | <span data-ttu-id="a8460-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a8460-107">Return Type</span></span>  |<span data-ttu-id="a8460-108">説明</span><span class="sxs-lookup"><span data-stu-id="a8460-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a8460-109">[一覧] タブ](../api/teamstab-list.md)</span><span class="sxs-lookup"><span data-stu-id="a8460-109">[List tabs](../api/teamstab-list.md)</span></span> | [<span data-ttu-id="a8460-110">teamsTab</span><span class="sxs-lookup"><span data-stu-id="a8460-110">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="a8460-111">リスト タブは、チャンネルに固定します。</span><span class="sxs-lookup"><span data-stu-id="a8460-111">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="a8460-112">タブを取得します。</span><span class="sxs-lookup"><span data-stu-id="a8460-112">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="a8460-113">teamsTab</span><span class="sxs-lookup"><span data-stu-id="a8460-113">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="a8460-114">チャンネルに固定されているタブを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="a8460-114">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="a8460-115">タブを追加します。</span><span class="sxs-lookup"><span data-stu-id="a8460-115">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="a8460-116">teamsTab</span><span class="sxs-lookup"><span data-stu-id="a8460-116">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="a8460-117">(ピン) を追加するチャンネルをタブします。</span><span class="sxs-lookup"><span data-stu-id="a8460-117">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="a8460-118">タブを削除します。</span><span class="sxs-lookup"><span data-stu-id="a8460-118">Remove tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="a8460-119">なし</span><span class="sxs-lookup"><span data-stu-id="a8460-119">None</span></span> | <span data-ttu-id="a8460-120">削除 (固定解除) チャネルからタブします。</span><span class="sxs-lookup"><span data-stu-id="a8460-120">Removes (unpins) a tab from a channel.</span></span>|
|<span data-ttu-id="a8460-121">[[更新] タブ](../api/teamstab-update.md)</span><span class="sxs-lookup"><span data-stu-id="a8460-121">[Update tab](../api/teamstab-update.md)</span></span> | [<span data-ttu-id="a8460-122">teamsTab</span><span class="sxs-lookup"><span data-stu-id="a8460-122">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="a8460-123">タブのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a8460-123">Updates the tab properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="a8460-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a8460-124">Properties</span></span>

|<span data-ttu-id="a8460-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a8460-125">Property</span></span>|<span data-ttu-id="a8460-126">型</span><span class="sxs-lookup"><span data-stu-id="a8460-126">Type</span></span>|<span data-ttu-id="a8460-127">説明</span><span class="sxs-lookup"><span data-stu-id="a8460-127">Description</span></span>|
|:---------------|:--------|:----------|
|  <span data-ttu-id="a8460-128">id</span><span class="sxs-lookup"><span data-stu-id="a8460-128">id</span></span>              |   <span data-ttu-id="a8460-129">文字列</span><span class="sxs-lookup"><span data-stu-id="a8460-129">string</span></span>                  |  <span data-ttu-id="a8460-130">チャネル タブ読み取りのみの特定のインスタンスを一意に識別する識別子です。</span><span class="sxs-lookup"><span data-stu-id="a8460-130">Identifier that uniquely identifies a specific instance of a channel tab. Read only.</span></span>     |
|  <span data-ttu-id="a8460-131">displayName</span><span class="sxs-lookup"><span data-stu-id="a8460-131">displayName</span></span>            |   <span data-ttu-id="a8460-132">string</span><span class="sxs-lookup"><span data-stu-id="a8460-132">string</span></span>                  |  <span data-ttu-id="a8460-133">タブの名前です。</span><span class="sxs-lookup"><span data-stu-id="a8460-133">Name of the tab.</span></span>     |
|  <span data-ttu-id="a8460-134">name</span><span class="sxs-lookup"><span data-stu-id="a8460-134">name</span></span>            |   <span data-ttu-id="a8460-135">文字列</span><span class="sxs-lookup"><span data-stu-id="a8460-135">string</span></span>                  |  <span data-ttu-id="a8460-136">(非推奨)タブの名前です。</span><span class="sxs-lookup"><span data-stu-id="a8460-136">(Deprecated) Name of the tab.</span></span>     |
|  <span data-ttu-id="a8460-137">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="a8460-137">teamsAppId</span></span>           |   <span data-ttu-id="a8460-138">文字列</span><span class="sxs-lookup"><span data-stu-id="a8460-138">string</span></span>             |  <span data-ttu-id="a8460-139">タブのアプリケーション定義の識別子です。タブを作成した後は、この値を変更できません。</span><span class="sxs-lookup"><span data-stu-id="a8460-139">App definition identifier of the tab. This value cannot be changed after tab creation.</span></span>     |
|  <span data-ttu-id="a8460-140">sortOrderIndex</span><span class="sxs-lookup"><span data-stu-id="a8460-140">sortOrderIndex</span></span>  |   <span data-ttu-id="a8460-141">文字列</span><span class="sxs-lookup"><span data-stu-id="a8460-141">string</span></span>                  |  <span data-ttu-id="a8460-142">タブの並べ替え順序のインデックス。</span><span class="sxs-lookup"><span data-stu-id="a8460-142">Index of the order used for sorting tabs.</span></span>     |
|  <span data-ttu-id="a8460-143">webUrl</span><span class="sxs-lookup"><span data-stu-id="a8460-143">webUrl</span></span>          |   <span data-ttu-id="a8460-144">文字列</span><span class="sxs-lookup"><span data-stu-id="a8460-144">string</span></span>                  |  <span data-ttu-id="a8460-145">タブのインスタンスの高度なリンクの url です。</span><span class="sxs-lookup"><span data-stu-id="a8460-145">Deep link url of the tab instance.</span></span> <span data-ttu-id="a8460-146">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a8460-146">Read only.</span></span>     |
|  <span data-ttu-id="a8460-147">configuration</span><span class="sxs-lookup"><span data-stu-id="a8460-147">configuration</span></span>        |   [<span data-ttu-id="a8460-148">teamsTabConfiguration</span><span class="sxs-lookup"><span data-stu-id="a8460-148">teamsTabConfiguration</span></span>](teamstabconfiguration.md) |  <span data-ttu-id="a8460-149">タブに適用するカスタム設定のコンテナーです。タブでは、このプロパティが 1 回だけが構成されていると見なされます。</span><span class="sxs-lookup"><span data-stu-id="a8460-149">Container for custom settings applied to a tab. The tab is considered configured only once this property is set.</span></span>     |

## <a name="relationships"></a><span data-ttu-id="a8460-150">関係</span><span class="sxs-lookup"><span data-stu-id="a8460-150">Relationships</span></span>

| <span data-ttu-id="a8460-151">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a8460-151">Relationship</span></span> | <span data-ttu-id="a8460-152">型</span><span class="sxs-lookup"><span data-stu-id="a8460-152">Type</span></span>   | <span data-ttu-id="a8460-153">説明</span><span class="sxs-lookup"><span data-stu-id="a8460-153">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="a8460-154">teamsApp</span><span class="sxs-lookup"><span data-stu-id="a8460-154">teamsApp</span></span>|[<span data-ttu-id="a8460-155">teamsApp</span><span class="sxs-lookup"><span data-stu-id="a8460-155">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="a8460-156">タブにリンクされているアプリケーションです。</span><span class="sxs-lookup"><span data-stu-id="a8460-156">The application that is linked to the tab.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a8460-157">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a8460-157">JSON representation</span></span>

<span data-ttu-id="a8460-158">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a8460-158">The following is a JSON representation of the resource.</span></span>


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
<!--
{
  "type": "#page.annotation",
  "description": "teamsTab resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamstab.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

## <a name="see-also"></a><span data-ttu-id="a8460-159">関連項目</span><span class="sxs-lookup"><span data-stu-id="a8460-159">See also</span></span>

[<span data-ttu-id="a8460-160">組み込みタブのタイプを設定します。</span><span class="sxs-lookup"><span data-stu-id="a8460-160">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)
