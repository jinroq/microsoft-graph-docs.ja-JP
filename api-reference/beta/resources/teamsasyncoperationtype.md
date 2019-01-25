---
title: teamsAsyncOperationType 列挙型
description: TeamsAsyncOperation のタイプです。 追加するメンバーがここでより多くの非同期操作はサポートされています。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 4de95db194bf41939521b53f06614b46b6afae99
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516568"
---
# <a name="teamsasyncoperationtype-enum-type"></a><span data-ttu-id="8aa93-104">teamsAsyncOperationType 列挙型</span><span class="sxs-lookup"><span data-stu-id="8aa93-104">teamsAsyncOperationType enum type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8aa93-105">[TeamsAsyncOperation](teamsasyncoperation.md)のタイプです。</span><span class="sxs-lookup"><span data-stu-id="8aa93-105">Types of [teamsAsyncOperation](teamsasyncoperation.md).</span></span> <span data-ttu-id="8aa93-106">追加するメンバーがここでより多くの非同期操作はサポートされています。</span><span class="sxs-lookup"><span data-stu-id="8aa93-106">Members will be added here as more async operations are supported.</span></span>

## <a name="members"></a><span data-ttu-id="8aa93-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="8aa93-107">Members</span></span>

| <span data-ttu-id="8aa93-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="8aa93-108">Member</span></span> | <span data-ttu-id="8aa93-109">値</span><span class="sxs-lookup"><span data-stu-id="8aa93-109">Value</span></span>| <span data-ttu-id="8aa93-110">説明</span><span class="sxs-lookup"><span data-stu-id="8aa93-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="8aa93-111">Invalid</span><span class="sxs-lookup"><span data-stu-id="8aa93-111">invalid</span></span>|<span data-ttu-id="8aa93-112">(0)</span><span class="sxs-lookup"><span data-stu-id="8aa93-112">0</span></span>|<span data-ttu-id="8aa93-113">無効な値</span><span class="sxs-lookup"><span data-stu-id="8aa93-113">Invalid value.</span></span>|
|<span data-ttu-id="8aa93-114">cloneTeam</span><span class="sxs-lookup"><span data-stu-id="8aa93-114">cloneTeam</span></span>|<span data-ttu-id="8aa93-115">-1</span><span class="sxs-lookup"><span data-stu-id="8aa93-115">1</span></span>|<span data-ttu-id="8aa93-116">チームのクローンを作成する操作です。</span><span class="sxs-lookup"><span data-stu-id="8aa93-116">Operation to clone a team.</span></span>|
|<span data-ttu-id="8aa93-117">archiveTeam</span><span class="sxs-lookup"><span data-stu-id="8aa93-117">archiveTeam</span></span>|<span data-ttu-id="8aa93-118">-2</span><span class="sxs-lookup"><span data-stu-id="8aa93-118">2</span></span>|<span data-ttu-id="8aa93-119">チームをアーカイブする操作です。</span><span class="sxs-lookup"><span data-stu-id="8aa93-119">Operation to archive a team.</span></span>|
|<span data-ttu-id="8aa93-120">unarchiveTeam</span><span class="sxs-lookup"><span data-stu-id="8aa93-120">unarchiveTeam</span></span>|<span data-ttu-id="8aa93-121">-3</span><span class="sxs-lookup"><span data-stu-id="8aa93-121">3</span></span>|<span data-ttu-id="8aa93-122">アーカイブされたチームを復元する操作です。</span><span class="sxs-lookup"><span data-stu-id="8aa93-122">Operation to restore an archived team.</span></span>|
|<span data-ttu-id="8aa93-123">createTeam</span><span class="sxs-lookup"><span data-stu-id="8aa93-123">createTeam</span></span>|<span data-ttu-id="8aa93-124">-3</span><span class="sxs-lookup"><span data-stu-id="8aa93-124">3</span></span>|<span data-ttu-id="8aa93-125">最初からチームを作成する操作です。</span><span class="sxs-lookup"><span data-stu-id="8aa93-125">Operation to create a team from scratch.</span></span>|

<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsasyncoperationtype.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
