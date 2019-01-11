---
title: teamsAsyncOperationStatus 列挙型
description: TeamsAsyncOperation の現在の状態について説明します。
author: nkramer
localization_priority: Normal
ms.openlocfilehash: b6af5c7218a6a9d8c0c5338beb8cdf9944a56c2e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858976"
---
# <a name="teamsasyncoperationstatus-enum-type"></a><span data-ttu-id="77740-103">teamsAsyncOperationStatus 列挙型</span><span class="sxs-lookup"><span data-stu-id="77740-103">teamsAsyncOperationStatus enum type</span></span>

> <span data-ttu-id="77740-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="77740-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="77740-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="77740-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="77740-106">の[teamsAsyncOperation](teamsasyncoperation.md)の現在の状態について説明します。</span><span class="sxs-lookup"><span data-stu-id="77740-106">Describes the current status of a [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="members"></a><span data-ttu-id="77740-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="77740-107">Members</span></span>

| <span data-ttu-id="77740-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="77740-108">Member</span></span> | <span data-ttu-id="77740-109">値</span><span class="sxs-lookup"><span data-stu-id="77740-109">Value</span></span>| <span data-ttu-id="77740-110">説明</span><span class="sxs-lookup"><span data-stu-id="77740-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="77740-111">無効です</span><span class="sxs-lookup"><span data-stu-id="77740-111">invalid</span></span>|<span data-ttu-id="77740-112">0</span><span class="sxs-lookup"><span data-stu-id="77740-112">0</span></span>|<span data-ttu-id="77740-113">値が無効です。</span><span class="sxs-lookup"><span data-stu-id="77740-113">Invalid value.</span></span>|
|<span data-ttu-id="77740-114">未開始</span><span class="sxs-lookup"><span data-stu-id="77740-114">notStarted</span></span>|<span data-ttu-id="77740-115">1</span><span class="sxs-lookup"><span data-stu-id="77740-115">1</span></span>|<span data-ttu-id="77740-116">操作は開始されていません。</span><span class="sxs-lookup"><span data-stu-id="77740-116">The operation has not started.</span></span>|
|<span data-ttu-id="77740-117">inProgress</span><span class="sxs-lookup"><span data-stu-id="77740-117">inProgress</span></span>|<span data-ttu-id="77740-118">2</span><span class="sxs-lookup"><span data-stu-id="77740-118">2</span></span>|<span data-ttu-id="77740-119">操作が行われています。</span><span class="sxs-lookup"><span data-stu-id="77740-119">The operation is running.</span></span>|
|<span data-ttu-id="77740-120">成功しました</span><span class="sxs-lookup"><span data-stu-id="77740-120">succeeded</span></span>|<span data-ttu-id="77740-121">3</span><span class="sxs-lookup"><span data-stu-id="77740-121">3</span></span>|<span data-ttu-id="77740-122">操作が正常に完了しました。</span><span class="sxs-lookup"><span data-stu-id="77740-122">The operation succeeded.</span></span>|
|<span data-ttu-id="77740-123">失敗しました。</span><span class="sxs-lookup"><span data-stu-id="77740-123">failed</span></span>|<span data-ttu-id="77740-124">4</span><span class="sxs-lookup"><span data-stu-id="77740-124">4</span></span>|<span data-ttu-id="77740-125">処理に失敗しました。</span><span class="sxs-lookup"><span data-stu-id="77740-125">The operation failed.</span></span>|
