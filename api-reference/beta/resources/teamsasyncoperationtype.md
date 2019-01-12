---
title: teamsAsyncOperationType 列挙型
description: TeamsAsyncOperation のタイプです。 追加するメンバーがここでより多くの非同期操作はサポートされています。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 1770f642970575647dd1216038202fca15f82117
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987308"
---
# <a name="teamsasyncoperationtype-enum-type"></a><span data-ttu-id="0905e-104">teamsAsyncOperationType 列挙型</span><span class="sxs-lookup"><span data-stu-id="0905e-104">teamsAsyncOperationType enum type</span></span>

> <span data-ttu-id="0905e-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0905e-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0905e-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0905e-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0905e-107">[TeamsAsyncOperation](teamsasyncoperation.md)のタイプです。</span><span class="sxs-lookup"><span data-stu-id="0905e-107">Types of [teamsAsyncOperation](teamsasyncoperation.md).</span></span> <span data-ttu-id="0905e-108">追加するメンバーがここでより多くの非同期操作はサポートされています。</span><span class="sxs-lookup"><span data-stu-id="0905e-108">Members will be added here as more async operations are supported.</span></span>

## <a name="members"></a><span data-ttu-id="0905e-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="0905e-109">Members</span></span>

| <span data-ttu-id="0905e-110">メンバー</span><span class="sxs-lookup"><span data-stu-id="0905e-110">Member</span></span> | <span data-ttu-id="0905e-111">値</span><span class="sxs-lookup"><span data-stu-id="0905e-111">Value</span></span>| <span data-ttu-id="0905e-112">説明</span><span class="sxs-lookup"><span data-stu-id="0905e-112">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="0905e-113">無効です</span><span class="sxs-lookup"><span data-stu-id="0905e-113">invalid</span></span>|<span data-ttu-id="0905e-114">0</span><span class="sxs-lookup"><span data-stu-id="0905e-114">0</span></span>|<span data-ttu-id="0905e-115">値が無効です。</span><span class="sxs-lookup"><span data-stu-id="0905e-115">Invalid value.</span></span>|
|<span data-ttu-id="0905e-116">cloneTeam</span><span class="sxs-lookup"><span data-stu-id="0905e-116">cloneTeam</span></span>|<span data-ttu-id="0905e-117">1</span><span class="sxs-lookup"><span data-stu-id="0905e-117">1</span></span>|<span data-ttu-id="0905e-118">チームのクローンを作成する操作です。</span><span class="sxs-lookup"><span data-stu-id="0905e-118">Operation to clone a team.</span></span>|
|<span data-ttu-id="0905e-119">archiveTeam</span><span class="sxs-lookup"><span data-stu-id="0905e-119">archiveTeam</span></span>|<span data-ttu-id="0905e-120">2</span><span class="sxs-lookup"><span data-stu-id="0905e-120">2</span></span>|<span data-ttu-id="0905e-121">チームをアーカイブする操作です。</span><span class="sxs-lookup"><span data-stu-id="0905e-121">Operation to archive a team.</span></span>|
|<span data-ttu-id="0905e-122">unarchiveTeam</span><span class="sxs-lookup"><span data-stu-id="0905e-122">unarchiveTeam</span></span>|<span data-ttu-id="0905e-123">3</span><span class="sxs-lookup"><span data-stu-id="0905e-123">3</span></span>|<span data-ttu-id="0905e-124">アーカイブされたチームを復元する操作です。</span><span class="sxs-lookup"><span data-stu-id="0905e-124">Operation to restore an archived team.</span></span>|
|<span data-ttu-id="0905e-125">createTeam</span><span class="sxs-lookup"><span data-stu-id="0905e-125">createTeam</span></span>|<span data-ttu-id="0905e-126">3</span><span class="sxs-lookup"><span data-stu-id="0905e-126">3</span></span>|<span data-ttu-id="0905e-127">最初からチームを作成する操作です。</span><span class="sxs-lookup"><span data-stu-id="0905e-127">Operation to create a team from scratch.</span></span>|

