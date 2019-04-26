---
title: teamsAsyncOperationType 列挙型
description: teamsAsyncOperation の種類。 より多くの非同期操作がサポートされているので、メンバーが追加されます。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: ad1fdb80768a6f4c7043b5431bd0ed84bf2f25f6
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341541"
---
# <a name="teamsasyncoperationtype-enum-type"></a><span data-ttu-id="b1b35-104">teamsAsyncOperationType 列挙型</span><span class="sxs-lookup"><span data-stu-id="b1b35-104">teamsAsyncOperationType enum type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1b35-105">[teamsAsyncOperation](teamsasyncoperation.md)の種類。</span><span class="sxs-lookup"><span data-stu-id="b1b35-105">Types of [teamsAsyncOperation](teamsasyncoperation.md).</span></span> <span data-ttu-id="b1b35-106">より多くの非同期操作がサポートされているので、メンバーが追加されます。</span><span class="sxs-lookup"><span data-stu-id="b1b35-106">Members will be added here as more async operations are supported.</span></span>

## <a name="members"></a><span data-ttu-id="b1b35-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="b1b35-107">Members</span></span>

| <span data-ttu-id="b1b35-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="b1b35-108">Member</span></span> | <span data-ttu-id="b1b35-109">値</span><span class="sxs-lookup"><span data-stu-id="b1b35-109">Value</span></span>| <span data-ttu-id="b1b35-110">説明</span><span class="sxs-lookup"><span data-stu-id="b1b35-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="b1b35-111">無効です</span><span class="sxs-lookup"><span data-stu-id="b1b35-111">invalid</span></span>|<span data-ttu-id="b1b35-112">.0</span><span class="sxs-lookup"><span data-stu-id="b1b35-112">0</span></span>|<span data-ttu-id="b1b35-113">無効な値です。</span><span class="sxs-lookup"><span data-stu-id="b1b35-113">Invalid value.</span></span>|
|<span data-ttu-id="b1b35-114">cloneTeam</span><span class="sxs-lookup"><span data-stu-id="b1b35-114">cloneTeam</span></span>|<span data-ttu-id="b1b35-115">1-d</span><span class="sxs-lookup"><span data-stu-id="b1b35-115">1</span></span>|<span data-ttu-id="b1b35-116">チームを複製する操作。</span><span class="sxs-lookup"><span data-stu-id="b1b35-116">Operation to clone a team.</span></span>|
|<span data-ttu-id="b1b35-117">アーカイブチーム</span><span class="sxs-lookup"><span data-stu-id="b1b35-117">archiveTeam</span></span>|<span data-ttu-id="b1b35-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="b1b35-118">2</span></span>|<span data-ttu-id="b1b35-119">チームをアーカイブする操作。</span><span class="sxs-lookup"><span data-stu-id="b1b35-119">Operation to archive a team.</span></span>|
|<span data-ttu-id="b1b35-120">アーカイブなしのチーム</span><span class="sxs-lookup"><span data-stu-id="b1b35-120">unarchiveTeam</span></span>|<span data-ttu-id="b1b35-121">1/3</span><span class="sxs-lookup"><span data-stu-id="b1b35-121">3</span></span>|<span data-ttu-id="b1b35-122">アーカイブされたチームを復元する操作。</span><span class="sxs-lookup"><span data-stu-id="b1b35-122">Operation to restore an archived team.</span></span>|
|<span data-ttu-id="b1b35-123">teamsasyncoperationtype</span><span class="sxs-lookup"><span data-stu-id="b1b35-123">createTeam</span></span>|<span data-ttu-id="b1b35-124">1/3</span><span class="sxs-lookup"><span data-stu-id="b1b35-124">3</span></span>|<span data-ttu-id="b1b35-125">最初からチームを作成する操作。</span><span class="sxs-lookup"><span data-stu-id="b1b35-125">Operation to create a team from scratch.</span></span>|

