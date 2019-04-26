---
title: teamsAsyncOperationStatus 列挙型
description: teamsAsyncOperation の現在の状態を表します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: bd44b7e1feabfba75edaa9bbeb88f1f0ed7a00f0
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345748"
---
# <a name="teamsasyncoperationstatus-enum-type"></a><span data-ttu-id="20c79-103">teamsAsyncOperationStatus 列挙型</span><span class="sxs-lookup"><span data-stu-id="20c79-103">teamsAsyncOperationStatus enum type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20c79-104">[teamsAsyncOperation](teamsasyncoperation.md)の現在の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="20c79-104">Describes the current status of a [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="members"></a><span data-ttu-id="20c79-105">メンバー</span><span class="sxs-lookup"><span data-stu-id="20c79-105">Members</span></span>

| <span data-ttu-id="20c79-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="20c79-106">Member</span></span> | <span data-ttu-id="20c79-107">値</span><span class="sxs-lookup"><span data-stu-id="20c79-107">Value</span></span>| <span data-ttu-id="20c79-108">説明</span><span class="sxs-lookup"><span data-stu-id="20c79-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="20c79-109">無効です</span><span class="sxs-lookup"><span data-stu-id="20c79-109">invalid</span></span>|<span data-ttu-id="20c79-110">.0</span><span class="sxs-lookup"><span data-stu-id="20c79-110">0</span></span>|<span data-ttu-id="20c79-111">無効な値です。</span><span class="sxs-lookup"><span data-stu-id="20c79-111">Invalid value.</span></span>|
|<span data-ttu-id="20c79-112">notStarted</span><span class="sxs-lookup"><span data-stu-id="20c79-112">notStarted</span></span>|<span data-ttu-id="20c79-113">1-d</span><span class="sxs-lookup"><span data-stu-id="20c79-113">1</span></span>|<span data-ttu-id="20c79-114">操作は開始されていません。</span><span class="sxs-lookup"><span data-stu-id="20c79-114">The operation has not started.</span></span>|
|<span data-ttu-id="20c79-115">inProgress</span><span class="sxs-lookup"><span data-stu-id="20c79-115">inProgress</span></span>|<span data-ttu-id="20c79-116">pbm-2</span><span class="sxs-lookup"><span data-stu-id="20c79-116">2</span></span>|<span data-ttu-id="20c79-117">操作が実行されています。</span><span class="sxs-lookup"><span data-stu-id="20c79-117">The operation is running.</span></span>|
|<span data-ttu-id="20c79-118">失敗</span><span class="sxs-lookup"><span data-stu-id="20c79-118">succeeded</span></span>|<span data-ttu-id="20c79-119">1/3</span><span class="sxs-lookup"><span data-stu-id="20c79-119">3</span></span>|<span data-ttu-id="20c79-120">操作が正常に完了しました。</span><span class="sxs-lookup"><span data-stu-id="20c79-120">The operation succeeded.</span></span>|
|<span data-ttu-id="20c79-121">フェール</span><span class="sxs-lookup"><span data-stu-id="20c79-121">failed</span></span>|<span data-ttu-id="20c79-122">2/4</span><span class="sxs-lookup"><span data-stu-id="20c79-122">4</span></span>|<span data-ttu-id="20c79-123">操作は失敗しました。</span><span class="sxs-lookup"><span data-stu-id="20c79-123">The operation failed.</span></span>|
