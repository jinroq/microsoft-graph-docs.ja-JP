---
title: teamsAsyncOperationType 列挙型
description: TeamsAsyncOperation のタイプです。 追加するメンバーがここでより多くの非同期操作はサポートされています。
author: nkramer
ms.openlocfilehash: 4ae7f070ffcce377fb4112ed5a54b4ad22d7973f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27346852"
---
# <a name="teamsasyncoperationtype-enum-type"></a><span data-ttu-id="57c95-104">teamsAsyncOperationType 列挙型</span><span class="sxs-lookup"><span data-stu-id="57c95-104">teamsAsyncOperationType enum type</span></span>

> <span data-ttu-id="57c95-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="57c95-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="57c95-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="57c95-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="57c95-107">[TeamsAsyncOperation](teamsasyncoperation.md)のタイプです。</span><span class="sxs-lookup"><span data-stu-id="57c95-107">Types of [teamsAsyncOperation](teamsasyncoperation.md).</span></span> <span data-ttu-id="57c95-108">追加するメンバーがここでより多くの非同期操作はサポートされています。</span><span class="sxs-lookup"><span data-stu-id="57c95-108">Members will be added here as more async operations are supported.</span></span>

## <a name="members"></a><span data-ttu-id="57c95-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="57c95-109">Members</span></span>

| <span data-ttu-id="57c95-110">メンバー</span><span class="sxs-lookup"><span data-stu-id="57c95-110">Member</span></span> | <span data-ttu-id="57c95-111">値</span><span class="sxs-lookup"><span data-stu-id="57c95-111">Value</span></span>| <span data-ttu-id="57c95-112">説明</span><span class="sxs-lookup"><span data-stu-id="57c95-112">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="57c95-113">無効です</span><span class="sxs-lookup"><span data-stu-id="57c95-113">invalid</span></span>|<span data-ttu-id="57c95-114">0</span><span class="sxs-lookup"><span data-stu-id="57c95-114">0</span></span>|<span data-ttu-id="57c95-115">値が無効です。</span><span class="sxs-lookup"><span data-stu-id="57c95-115">Invalid value.</span></span>|
|<span data-ttu-id="57c95-116">cloneTeam</span><span class="sxs-lookup"><span data-stu-id="57c95-116">cloneTeam</span></span>|<span data-ttu-id="57c95-117">1</span><span class="sxs-lookup"><span data-stu-id="57c95-117">1</span></span>|<span data-ttu-id="57c95-118">チームのクローンを作成する操作です。</span><span class="sxs-lookup"><span data-stu-id="57c95-118">Operation to clone a team.</span></span>|
|<span data-ttu-id="57c95-119">archiveTeam</span><span class="sxs-lookup"><span data-stu-id="57c95-119">archiveTeam</span></span>|<span data-ttu-id="57c95-120">2</span><span class="sxs-lookup"><span data-stu-id="57c95-120">2</span></span>|<span data-ttu-id="57c95-121">チームをアーカイブする操作です。</span><span class="sxs-lookup"><span data-stu-id="57c95-121">Operation to archive a team.</span></span>|
|<span data-ttu-id="57c95-122">unarchiveTeam</span><span class="sxs-lookup"><span data-stu-id="57c95-122">unarchiveTeam</span></span>|<span data-ttu-id="57c95-123">3</span><span class="sxs-lookup"><span data-stu-id="57c95-123">3</span></span>|<span data-ttu-id="57c95-124">アーカイブされたチームを復元する操作です。</span><span class="sxs-lookup"><span data-stu-id="57c95-124">Operation to restore an archived team.</span></span>|
|<span data-ttu-id="57c95-125">createTeam</span><span class="sxs-lookup"><span data-stu-id="57c95-125">createTeam</span></span>|<span data-ttu-id="57c95-126">3</span><span class="sxs-lookup"><span data-stu-id="57c95-126">3</span></span>|<span data-ttu-id="57c95-127">最初からチームを作成する操作です。</span><span class="sxs-lookup"><span data-stu-id="57c95-127">Operation to create a team from scratch.</span></span>|

