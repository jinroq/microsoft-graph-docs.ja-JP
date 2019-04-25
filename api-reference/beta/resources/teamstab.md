---
title: teamstab リソースの種類
description: 'teamstab は、チーム内のチャネルに固定 (接続) されたタブです。 '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 207b9d1d4d27199f07ae22bd47587411f917afae
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32553646"
---
# <a name="teamstab-resource-type"></a><span data-ttu-id="e6d5b-103">teamstab リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e6d5b-103">teamsTab resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6d5b-104">teamstab は、[チーム](team.md)内の[チャネル](channel.md)に固定 (接続) された[タブ](../resources/teamstab.md)です。</span><span class="sxs-lookup"><span data-stu-id="e6d5b-104">A teamsTab is a [tab](../resources/teamstab.md) that's pinned (attached) to a [channel](channel.md) within a [team](team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="e6d5b-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="e6d5b-105">Methods</span></span>

| <span data-ttu-id="e6d5b-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="e6d5b-106">Method</span></span>       | <span data-ttu-id="e6d5b-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e6d5b-107">Return Type</span></span>  |<span data-ttu-id="e6d5b-108">説明</span><span class="sxs-lookup"><span data-stu-id="e6d5b-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e6d5b-109">タブを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="e6d5b-109">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="e6d5b-110">teamsTab</span><span class="sxs-lookup"><span data-stu-id="e6d5b-110">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="e6d5b-111">チャネルにピン留めされたタブを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="e6d5b-111">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="e6d5b-112">タブを取得する</span><span class="sxs-lookup"><span data-stu-id="e6d5b-112">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="e6d5b-113">teamsTab</span><span class="sxs-lookup"><span data-stu-id="e6d5b-113">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="e6d5b-114">チャネルにピン留めされたタブを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e6d5b-114">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="e6d5b-115">タブを追加する</span><span class="sxs-lookup"><span data-stu-id="e6d5b-115">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="e6d5b-116">teamsTab</span><span class="sxs-lookup"><span data-stu-id="e6d5b-116">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="e6d5b-117">チャネルにタブを追加 (ピン留め) します。</span><span class="sxs-lookup"><span data-stu-id="e6d5b-117">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="e6d5b-118">タブの削除</span><span class="sxs-lookup"><span data-stu-id="e6d5b-118">Remove tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="e6d5b-119">なし</span><span class="sxs-lookup"><span data-stu-id="e6d5b-119">None</span></span> | <span data-ttu-id="e6d5b-120">チャネルからタブを削除 (固定解除) します。</span><span class="sxs-lookup"><span data-stu-id="e6d5b-120">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="e6d5b-121">タブを更新する</span><span class="sxs-lookup"><span data-stu-id="e6d5b-121">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="e6d5b-122">teamsTab</span><span class="sxs-lookup"><span data-stu-id="e6d5b-122">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="e6d5b-123">タブのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e6d5b-123">Updates the tab properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="e6d5b-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e6d5b-124">Properties</span></span>

|<span data-ttu-id="e6d5b-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e6d5b-125">Property</span></span>|<span data-ttu-id="e6d5b-126">型</span><span class="sxs-lookup"><span data-stu-id="e6d5b-126">Type</span></span>|<span data-ttu-id="e6d5b-127">説明</span><span class="sxs-lookup"><span data-stu-id="e6d5b-127">Description</span></span>|
|:---------------|:--------|:----------|
|  <span data-ttu-id="e6d5b-128">id</span><span class="sxs-lookup"><span data-stu-id="e6d5b-128">id</span></span>              |   <span data-ttu-id="e6d5b-129">string</span><span class="sxs-lookup"><span data-stu-id="e6d5b-129">string</span></span>                  |  <span data-ttu-id="e6d5b-130">チャネルタブの特定のインスタンスを一意に識別する識別子。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="e6d5b-130">Identifier that uniquely identifies a specific instance of a channel tab. Read only.</span></span>     |
|  <span data-ttu-id="e6d5b-131">displayName</span><span class="sxs-lookup"><span data-stu-id="e6d5b-131">displayName</span></span>            |   <span data-ttu-id="e6d5b-132">string</span><span class="sxs-lookup"><span data-stu-id="e6d5b-132">string</span></span>                  |  <span data-ttu-id="e6d5b-133">タブの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="e6d5b-133">Name of the tab.</span></span>     |
|  <span data-ttu-id="e6d5b-134">name</span><span class="sxs-lookup"><span data-stu-id="e6d5b-134">name</span></span>            |   <span data-ttu-id="e6d5b-135">string</span><span class="sxs-lookup"><span data-stu-id="e6d5b-135">string</span></span>                  |  <span data-ttu-id="e6d5b-136">予定タブの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="e6d5b-136">(Deprecated) Name of the tab.</span></span>     |
|  <span data-ttu-id="e6d5b-137">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="e6d5b-137">teamsAppId</span></span>           |   <span data-ttu-id="e6d5b-138">string</span><span class="sxs-lookup"><span data-stu-id="e6d5b-138">string</span></span>             |  <span data-ttu-id="e6d5b-139">タブのアプリ定義識別子。この値は、タブの作成後に変更することはできません。</span><span class="sxs-lookup"><span data-stu-id="e6d5b-139">App definition identifier of the tab. This value cannot be changed after tab creation.</span></span>     |
|  <span data-ttu-id="e6d5b-140">sortorderindex</span><span class="sxs-lookup"><span data-stu-id="e6d5b-140">sortOrderIndex</span></span>  |   <span data-ttu-id="e6d5b-141">string</span><span class="sxs-lookup"><span data-stu-id="e6d5b-141">string</span></span>                  |  <span data-ttu-id="e6d5b-142">タブの並べ替えに使用される順序のインデックスです。</span><span class="sxs-lookup"><span data-stu-id="e6d5b-142">Index of the order used for sorting tabs.</span></span>     |
|  <span data-ttu-id="e6d5b-143">webUrl</span><span class="sxs-lookup"><span data-stu-id="e6d5b-143">webUrl</span></span>          |   <span data-ttu-id="e6d5b-144">string</span><span class="sxs-lookup"><span data-stu-id="e6d5b-144">string</span></span>                  |  <span data-ttu-id="e6d5b-145">tab インスタンスのディープリンク url。</span><span class="sxs-lookup"><span data-stu-id="e6d5b-145">Deep link url of the tab instance.</span></span> <span data-ttu-id="e6d5b-146">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="e6d5b-146">Read only.</span></span>     |
|  <span data-ttu-id="e6d5b-147">環境</span><span class="sxs-lookup"><span data-stu-id="e6d5b-147">configuration</span></span>        |   [<span data-ttu-id="e6d5b-148">teamstabconfiguration</span><span class="sxs-lookup"><span data-stu-id="e6d5b-148">teamsTabConfiguration</span></span>](teamstabconfiguration.md) |  <span data-ttu-id="e6d5b-149">タブに適用されるカスタム設定のコンテナーです。このプロパティが設定されると、タブは構成されたことを示します。</span><span class="sxs-lookup"><span data-stu-id="e6d5b-149">Container for custom settings applied to a tab. The tab is considered configured only once this property is set.</span></span>     |

## <a name="relationships"></a><span data-ttu-id="e6d5b-150">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e6d5b-150">Relationships</span></span>

| <span data-ttu-id="e6d5b-151">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e6d5b-151">Relationship</span></span> | <span data-ttu-id="e6d5b-152">型</span><span class="sxs-lookup"><span data-stu-id="e6d5b-152">Type</span></span>   | <span data-ttu-id="e6d5b-153">説明</span><span class="sxs-lookup"><span data-stu-id="e6d5b-153">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="e6d5b-154">teamsApp</span><span class="sxs-lookup"><span data-stu-id="e6d5b-154">teamsApp</span></span>|[<span data-ttu-id="e6d5b-155">teamsApp</span><span class="sxs-lookup"><span data-stu-id="e6d5b-155">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="e6d5b-156">タブにリンクされているアプリケーション。</span><span class="sxs-lookup"><span data-stu-id="e6d5b-156">The application that is linked to the tab.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e6d5b-157">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e6d5b-157">JSON representation</span></span>

<span data-ttu-id="e6d5b-158">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e6d5b-158">The following is a JSON representation of the resource.</span></span>


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

## <a name="see-also"></a><span data-ttu-id="e6d5b-159">関連項目</span><span class="sxs-lookup"><span data-stu-id="e6d5b-159">See also</span></span>

[<span data-ttu-id="e6d5b-160">組み込みタブ タイプの構成</span><span class="sxs-lookup"><span data-stu-id="e6d5b-160">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)
