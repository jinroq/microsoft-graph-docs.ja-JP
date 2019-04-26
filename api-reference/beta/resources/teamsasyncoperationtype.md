---
title: teamsAsyncOperationType 列挙型
description: teamsAsyncOperation の種類。 より多くの非同期操作がサポートされているので、メンバーが追加されます。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 4de95db194bf41939521b53f06614b46b6afae99
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32553639"
---
# <a name="teamsasyncoperationtype-enum-type"></a><span data-ttu-id="8f9d1-104">teamsAsyncOperationType 列挙型</span><span class="sxs-lookup"><span data-stu-id="8f9d1-104">teamsAsyncOperationType enum type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f9d1-105">[teamsAsyncOperation](teamsasyncoperation.md)の種類。</span><span class="sxs-lookup"><span data-stu-id="8f9d1-105">Types of [teamsAsyncOperation](teamsasyncoperation.md).</span></span> <span data-ttu-id="8f9d1-106">より多くの非同期操作がサポートされているので、メンバーが追加されます。</span><span class="sxs-lookup"><span data-stu-id="8f9d1-106">Members will be added here as more async operations are supported.</span></span>

## <a name="members"></a><span data-ttu-id="8f9d1-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="8f9d1-107">Members</span></span>

| <span data-ttu-id="8f9d1-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="8f9d1-108">Member</span></span> | <span data-ttu-id="8f9d1-109">値</span><span class="sxs-lookup"><span data-stu-id="8f9d1-109">Value</span></span>| <span data-ttu-id="8f9d1-110">説明</span><span class="sxs-lookup"><span data-stu-id="8f9d1-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="8f9d1-111">無効です</span><span class="sxs-lookup"><span data-stu-id="8f9d1-111">invalid</span></span>|<span data-ttu-id="8f9d1-112">.0</span><span class="sxs-lookup"><span data-stu-id="8f9d1-112">0</span></span>|<span data-ttu-id="8f9d1-113">無効な値です。</span><span class="sxs-lookup"><span data-stu-id="8f9d1-113">Invalid value.</span></span>|
|<span data-ttu-id="8f9d1-114">cloneTeam</span><span class="sxs-lookup"><span data-stu-id="8f9d1-114">cloneTeam</span></span>|<span data-ttu-id="8f9d1-115">1 </span><span class="sxs-lookup"><span data-stu-id="8f9d1-115">1</span></span>|<span data-ttu-id="8f9d1-116">チームを複製する操作。</span><span class="sxs-lookup"><span data-stu-id="8f9d1-116">Operation to clone a team.</span></span>|
|<span data-ttu-id="8f9d1-117">アーカイブチーム</span><span class="sxs-lookup"><span data-stu-id="8f9d1-117">archiveTeam</span></span>|<span data-ttu-id="8f9d1-118">2 </span><span class="sxs-lookup"><span data-stu-id="8f9d1-118">2</span></span>|<span data-ttu-id="8f9d1-119">チームをアーカイブする操作。</span><span class="sxs-lookup"><span data-stu-id="8f9d1-119">Operation to archive a team.</span></span>|
|<span data-ttu-id="8f9d1-120">アーカイブなしのチーム</span><span class="sxs-lookup"><span data-stu-id="8f9d1-120">unarchiveTeam</span></span>|<span data-ttu-id="8f9d1-121">3 </span><span class="sxs-lookup"><span data-stu-id="8f9d1-121">3</span></span>|<span data-ttu-id="8f9d1-122">アーカイブされたチームを復元する操作。</span><span class="sxs-lookup"><span data-stu-id="8f9d1-122">Operation to restore an archived team.</span></span>|
|<span data-ttu-id="8f9d1-123">teamsasyncoperationtype</span><span class="sxs-lookup"><span data-stu-id="8f9d1-123">createTeam</span></span>|<span data-ttu-id="8f9d1-124">3 </span><span class="sxs-lookup"><span data-stu-id="8f9d1-124">3</span></span>|<span data-ttu-id="8f9d1-125">最初からチームを作成する操作。</span><span class="sxs-lookup"><span data-stu-id="8f9d1-125">Operation to create a team from scratch.</span></span>|

<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsasyncoperationtype.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
