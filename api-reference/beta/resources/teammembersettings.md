---
title: teammembersettings リソースの種類
description: メンバーが特定のアクション (チャネルの作成、ボットの追加など) をチーム内で実行できるかどうかを構成する設定。
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 33f1930096ff63968db39e06ddec26c53ae8bcc9
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341723"
---
# <a name="teammembersettings-resource-type"></a><span data-ttu-id="6427b-103">teammembersettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6427b-103">teamMemberSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6427b-104">[チーム](team.md)内で、メンバーが特定のアクション (チャネルの作成、ボットの追加など) を実行できるかどうかを構成するための設定。</span><span class="sxs-lookup"><span data-stu-id="6427b-104">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="6427b-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6427b-105">Properties</span></span>
| <span data-ttu-id="6427b-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6427b-106">Property</span></span>     | <span data-ttu-id="6427b-107">型</span><span class="sxs-lookup"><span data-stu-id="6427b-107">Type</span></span>   |<span data-ttu-id="6427b-108">説明</span><span class="sxs-lookup"><span data-stu-id="6427b-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6427b-109">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="6427b-109">allowCreateUpdateChannels</span></span>|<span data-ttu-id="6427b-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="6427b-110">Boolean</span></span>|<span data-ttu-id="6427b-111">true に設定されている場合、メンバーはチャネルを追加および更新できます。</span><span class="sxs-lookup"><span data-stu-id="6427b-111">If set to true, members can add and update channels.</span></span>|
|<span data-ttu-id="6427b-112">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="6427b-112">allowDeleteChannels</span></span>|<span data-ttu-id="6427b-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="6427b-113">Boolean</span></span>|<span data-ttu-id="6427b-114">true に設定されている場合、メンバーはチャネルを削除できます。</span><span class="sxs-lookup"><span data-stu-id="6427b-114">If set to true, members can delete channels.</span></span>|
|<span data-ttu-id="6427b-115">allowaddremoveapps</span><span class="sxs-lookup"><span data-stu-id="6427b-115">allowAddRemoveApps</span></span>|<span data-ttu-id="6427b-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="6427b-116">Boolean</span></span>|<span data-ttu-id="6427b-117">true に設定すると、メンバーはアプリを追加および削除できるようになります。</span><span class="sxs-lookup"><span data-stu-id="6427b-117">If set to true, members can add and remove apps.</span></span>|
|<span data-ttu-id="6427b-118">allowCreateUpdateRemoveTabs</span><span class="sxs-lookup"><span data-stu-id="6427b-118">allowCreateUpdateRemoveTabs</span></span>|<span data-ttu-id="6427b-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="6427b-119">Boolean</span></span>|<span data-ttu-id="6427b-120">true に設定されている場合、メンバーはタブの追加、更新、および削除を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="6427b-120">If set to true, members can add, update, and remove tabs.</span></span> |
|<span data-ttu-id="6427b-121">allowCreateUpdateRemoveConnectors</span><span class="sxs-lookup"><span data-stu-id="6427b-121">allowCreateUpdateRemoveConnectors</span></span>|<span data-ttu-id="6427b-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="6427b-122">Boolean</span></span>|<span data-ttu-id="6427b-123">true に設定されている場合、メンバーはコネクタの追加、更新、および削除を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="6427b-123">If set to true, members can add, update, and remove connectors.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6427b-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6427b-124">JSON representation</span></span>

<span data-ttu-id="6427b-125">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6427b-125">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "team's memberSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
