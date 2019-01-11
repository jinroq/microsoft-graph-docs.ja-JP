---
title: teamMemberSettings リソースの種類
description: など、メンバーが特定のアクションを実行するかどうかを構成する設定は、チャネルを作成し、チームにボットを追加します。
localization_priority: Normal
ms.openlocfilehash: 85f8794ea3564174c75f38228f3891bcd264df2e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851381"
---
# <a name="teammembersettings-resource-type"></a><span data-ttu-id="a1d80-103">teamMemberSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a1d80-103">teamMemberSettings resource type</span></span>

> <span data-ttu-id="a1d80-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a1d80-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a1d80-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a1d80-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a1d80-106">など、メンバーが特定のアクションを実行するかどうかを構成する設定は、チャネルを作成し、[チーム](team.md)にボットを追加します。</span><span class="sxs-lookup"><span data-stu-id="a1d80-106">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="a1d80-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a1d80-107">Properties</span></span>
| <span data-ttu-id="a1d80-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a1d80-108">Property</span></span>     | <span data-ttu-id="a1d80-109">種類</span><span class="sxs-lookup"><span data-stu-id="a1d80-109">Type</span></span>   |<span data-ttu-id="a1d80-110">説明</span><span class="sxs-lookup"><span data-stu-id="a1d80-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a1d80-111">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="a1d80-111">allowCreateUpdateChannels</span></span>|<span data-ttu-id="a1d80-112">ブール型</span><span class="sxs-lookup"><span data-stu-id="a1d80-112">Boolean</span></span>|<span data-ttu-id="a1d80-113">True の場合、メンバー セットを追加したりチャンネルを更新する場合。</span><span class="sxs-lookup"><span data-stu-id="a1d80-113">If set to true, members can add and update channels.</span></span>|
|<span data-ttu-id="a1d80-114">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="a1d80-114">allowDeleteChannels</span></span>|<span data-ttu-id="a1d80-115">ブール型</span><span class="sxs-lookup"><span data-stu-id="a1d80-115">Boolean</span></span>|<span data-ttu-id="a1d80-116">場合は true の場合、メンバーに設定するには、チャンネルを削除できます。</span><span class="sxs-lookup"><span data-stu-id="a1d80-116">If set to true, members can delete channels.</span></span>|
|<span data-ttu-id="a1d80-117">allowAddRemoveApps</span><span class="sxs-lookup"><span data-stu-id="a1d80-117">allowAddRemoveApps</span></span>|<span data-ttu-id="a1d80-118">ブール型</span><span class="sxs-lookup"><span data-stu-id="a1d80-118">Boolean</span></span>|<span data-ttu-id="a1d80-119">場合は true の場合、メンバー セットは、追加し、アプリケーションを削除できます。</span><span class="sxs-lookup"><span data-stu-id="a1d80-119">If set to true, members can add and remove apps.</span></span>|
|<span data-ttu-id="a1d80-120">allowCreateUpdateRemoveTabs</span><span class="sxs-lookup"><span data-stu-id="a1d80-120">allowCreateUpdateRemoveTabs</span></span>|<span data-ttu-id="a1d80-121">ブール型</span><span class="sxs-lookup"><span data-stu-id="a1d80-121">Boolean</span></span>|<span data-ttu-id="a1d80-122">場合は true の場合、メンバー セットを追加、更新、およびタブを削除します。</span><span class="sxs-lookup"><span data-stu-id="a1d80-122">If set to true, members can add, update, and remove tabs.</span></span> |
|<span data-ttu-id="a1d80-123">allowCreateUpdateRemoveConnectors</span><span class="sxs-lookup"><span data-stu-id="a1d80-123">allowCreateUpdateRemoveConnectors</span></span>|<span data-ttu-id="a1d80-124">ブール型</span><span class="sxs-lookup"><span data-stu-id="a1d80-124">Boolean</span></span>|<span data-ttu-id="a1d80-125">場合は true の場合、メンバー セットを追加、更新、およびコネクタを削除します。</span><span class="sxs-lookup"><span data-stu-id="a1d80-125">If set to true, members can add, update, and remove connectors.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a1d80-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a1d80-126">JSON representation</span></span>

<span data-ttu-id="a1d80-127">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a1d80-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamMemberSettings"
}-->

```json
{
  "allowCreateUpdateChannels": true,
  "allowDeleteChannels": true,
  "allowAddRemoveApps": true,
  "allowCreateUpdateRemoveTabs": true,
  "allowCreateUpdateRemoveConnectors": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's memberSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
