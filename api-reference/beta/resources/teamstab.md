---
title: teamstab リソースの種類
description: 'teamstab は、チーム内のチャネルに固定 (接続) されたタブです。 '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 6666fbcd69ac46e778ef46380c426c4e94a129fc
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345695"
---
# <a name="teamstab-resource-type"></a><span data-ttu-id="ff594-103">teamstab リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ff594-103">teamsTab resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff594-104">teamstab は、[チーム](team.md)内の[チャネル](channel.md)に固定 (接続) された[タブ](../resources/teamstab.md)です。</span><span class="sxs-lookup"><span data-stu-id="ff594-104">A teamsTab is a [tab](../resources/teamstab.md) that's pinned (attached) to a [channel](channel.md) within a [team](team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="ff594-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="ff594-105">Methods</span></span>

| <span data-ttu-id="ff594-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="ff594-106">Method</span></span>       | <span data-ttu-id="ff594-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ff594-107">Return Type</span></span>  |<span data-ttu-id="ff594-108">説明</span><span class="sxs-lookup"><span data-stu-id="ff594-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ff594-109">タブを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="ff594-109">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="ff594-110">teamsTab</span><span class="sxs-lookup"><span data-stu-id="ff594-110">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="ff594-111">チャネルにピン留めされたタブを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="ff594-111">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="ff594-112">タブを取得する</span><span class="sxs-lookup"><span data-stu-id="ff594-112">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="ff594-113">teamsTab</span><span class="sxs-lookup"><span data-stu-id="ff594-113">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="ff594-114">チャネルにピン留めされたタブを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="ff594-114">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="ff594-115">タブを追加する</span><span class="sxs-lookup"><span data-stu-id="ff594-115">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="ff594-116">teamsTab</span><span class="sxs-lookup"><span data-stu-id="ff594-116">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="ff594-117">チャネルにタブを追加 (ピン留め) します。</span><span class="sxs-lookup"><span data-stu-id="ff594-117">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="ff594-118">タブの削除</span><span class="sxs-lookup"><span data-stu-id="ff594-118">Remove tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="ff594-119">なし</span><span class="sxs-lookup"><span data-stu-id="ff594-119">None</span></span> | <span data-ttu-id="ff594-120">チャネルからタブを削除 (固定解除) します。</span><span class="sxs-lookup"><span data-stu-id="ff594-120">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="ff594-121">タブを更新する</span><span class="sxs-lookup"><span data-stu-id="ff594-121">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="ff594-122">teamsTab</span><span class="sxs-lookup"><span data-stu-id="ff594-122">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="ff594-123">タブのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ff594-123">Updates the tab properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="ff594-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ff594-124">Properties</span></span>

|<span data-ttu-id="ff594-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ff594-125">Property</span></span>|<span data-ttu-id="ff594-126">型</span><span class="sxs-lookup"><span data-stu-id="ff594-126">Type</span></span>|<span data-ttu-id="ff594-127">説明</span><span class="sxs-lookup"><span data-stu-id="ff594-127">Description</span></span>|
|:---------------|:--------|:----------|
|  <span data-ttu-id="ff594-128">id</span><span class="sxs-lookup"><span data-stu-id="ff594-128">id</span></span>              |   <span data-ttu-id="ff594-129">string</span><span class="sxs-lookup"><span data-stu-id="ff594-129">string</span></span>                  |  <span data-ttu-id="ff594-130">チャネルタブの特定のインスタンスを一意に識別する識別子。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="ff594-130">Identifier that uniquely identifies a specific instance of a channel tab. Read only.</span></span>     |
|  <span data-ttu-id="ff594-131">displayName</span><span class="sxs-lookup"><span data-stu-id="ff594-131">displayName</span></span>            |   <span data-ttu-id="ff594-132">string</span><span class="sxs-lookup"><span data-stu-id="ff594-132">string</span></span>                  |  <span data-ttu-id="ff594-133">タブの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="ff594-133">Name of the tab.</span></span>     |
|  <span data-ttu-id="ff594-134">name</span><span class="sxs-lookup"><span data-stu-id="ff594-134">name</span></span>            |   <span data-ttu-id="ff594-135">string</span><span class="sxs-lookup"><span data-stu-id="ff594-135">string</span></span>                  |  <span data-ttu-id="ff594-136">予定タブの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="ff594-136">(Deprecated) Name of the tab.</span></span>     |
|  <span data-ttu-id="ff594-137">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="ff594-137">teamsAppId</span></span>           |   <span data-ttu-id="ff594-138">string</span><span class="sxs-lookup"><span data-stu-id="ff594-138">string</span></span>             |  <span data-ttu-id="ff594-139">タブのアプリ定義識別子。この値は、タブの作成後に変更することはできません。</span><span class="sxs-lookup"><span data-stu-id="ff594-139">App definition identifier of the tab. This value cannot be changed after tab creation.</span></span>     |
|  <span data-ttu-id="ff594-140">sortorderindex</span><span class="sxs-lookup"><span data-stu-id="ff594-140">sortOrderIndex</span></span>  |   <span data-ttu-id="ff594-141">string</span><span class="sxs-lookup"><span data-stu-id="ff594-141">string</span></span>                  |  <span data-ttu-id="ff594-142">タブの並べ替えに使用される順序のインデックスです。</span><span class="sxs-lookup"><span data-stu-id="ff594-142">Index of the order used for sorting tabs.</span></span>     |
|  <span data-ttu-id="ff594-143">webUrl</span><span class="sxs-lookup"><span data-stu-id="ff594-143">webUrl</span></span>          |   <span data-ttu-id="ff594-144">string</span><span class="sxs-lookup"><span data-stu-id="ff594-144">string</span></span>                  |  <span data-ttu-id="ff594-145">tab インスタンスのディープリンク url。</span><span class="sxs-lookup"><span data-stu-id="ff594-145">Deep link url of the tab instance.</span></span> <span data-ttu-id="ff594-146">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ff594-146">Read only.</span></span>     |
|  <span data-ttu-id="ff594-147">環境</span><span class="sxs-lookup"><span data-stu-id="ff594-147">configuration</span></span>        |   [<span data-ttu-id="ff594-148">teamstabconfiguration</span><span class="sxs-lookup"><span data-stu-id="ff594-148">teamsTabConfiguration</span></span>](teamstabconfiguration.md) |  <span data-ttu-id="ff594-149">タブに適用されるカスタム設定のコンテナーです。このプロパティが設定されると、タブは構成されたことを示します。</span><span class="sxs-lookup"><span data-stu-id="ff594-149">Container for custom settings applied to a tab. The tab is considered configured only once this property is set.</span></span>     |

## <a name="relationships"></a><span data-ttu-id="ff594-150">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ff594-150">Relationships</span></span>

| <span data-ttu-id="ff594-151">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ff594-151">Relationship</span></span> | <span data-ttu-id="ff594-152">型</span><span class="sxs-lookup"><span data-stu-id="ff594-152">Type</span></span>   | <span data-ttu-id="ff594-153">説明</span><span class="sxs-lookup"><span data-stu-id="ff594-153">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="ff594-154">teamsApp</span><span class="sxs-lookup"><span data-stu-id="ff594-154">teamsApp</span></span>|[<span data-ttu-id="ff594-155">teamsApp</span><span class="sxs-lookup"><span data-stu-id="ff594-155">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="ff594-156">タブにリンクされているアプリケーション。</span><span class="sxs-lookup"><span data-stu-id="ff594-156">The application that is linked to the tab.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ff594-157">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ff594-157">JSON representation</span></span>

<span data-ttu-id="ff594-158">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ff594-158">The following is a JSON representation of the resource.</span></span>


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
  "configuration": "teamsTabConfiguration",
  "name": "string"
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
  "suppressions": []
}
-->

## <a name="see-also"></a><span data-ttu-id="ff594-159">関連項目</span><span class="sxs-lookup"><span data-stu-id="ff594-159">See also</span></span>

[<span data-ttu-id="ff594-160">組み込みタブ タイプの構成</span><span class="sxs-lookup"><span data-stu-id="ff594-160">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)
