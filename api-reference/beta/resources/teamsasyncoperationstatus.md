---
title: teamsAsyncOperationStatus 列挙型
description: TeamsAsyncOperation の現在の状態について説明します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e136d043cf58480d93888374558a1be06ca9053d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914821"
---
# <a name="teamsasyncoperationstatus-enum-type"></a><span data-ttu-id="da763-103">teamsAsyncOperationStatus 列挙型</span><span class="sxs-lookup"><span data-stu-id="da763-103">teamsAsyncOperationStatus enum type</span></span>

> <span data-ttu-id="da763-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="da763-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="da763-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="da763-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="da763-106">の[teamsAsyncOperation](teamsasyncoperation.md)の現在の状態について説明します。</span><span class="sxs-lookup"><span data-stu-id="da763-106">Describes the current status of a [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="members"></a><span data-ttu-id="da763-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="da763-107">Members</span></span>

| <span data-ttu-id="da763-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="da763-108">Member</span></span> | <span data-ttu-id="da763-109">値</span><span class="sxs-lookup"><span data-stu-id="da763-109">Value</span></span>| <span data-ttu-id="da763-110">説明</span><span class="sxs-lookup"><span data-stu-id="da763-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="da763-111">無効です</span><span class="sxs-lookup"><span data-stu-id="da763-111">invalid</span></span>|<span data-ttu-id="da763-112">0</span><span class="sxs-lookup"><span data-stu-id="da763-112">0</span></span>|<span data-ttu-id="da763-113">値が無効です。</span><span class="sxs-lookup"><span data-stu-id="da763-113">Invalid value.</span></span>|
|<span data-ttu-id="da763-114">未開始</span><span class="sxs-lookup"><span data-stu-id="da763-114">notStarted</span></span>|<span data-ttu-id="da763-115">1</span><span class="sxs-lookup"><span data-stu-id="da763-115">1</span></span>|<span data-ttu-id="da763-116">操作は開始されていません。</span><span class="sxs-lookup"><span data-stu-id="da763-116">The operation has not started.</span></span>|
|<span data-ttu-id="da763-117">inProgress</span><span class="sxs-lookup"><span data-stu-id="da763-117">inProgress</span></span>|<span data-ttu-id="da763-118">2</span><span class="sxs-lookup"><span data-stu-id="da763-118">2</span></span>|<span data-ttu-id="da763-119">操作が行われています。</span><span class="sxs-lookup"><span data-stu-id="da763-119">The operation is running.</span></span>|
|<span data-ttu-id="da763-120">成功しました</span><span class="sxs-lookup"><span data-stu-id="da763-120">succeeded</span></span>|<span data-ttu-id="da763-121">3</span><span class="sxs-lookup"><span data-stu-id="da763-121">3</span></span>|<span data-ttu-id="da763-122">操作が正常に完了しました。</span><span class="sxs-lookup"><span data-stu-id="da763-122">The operation succeeded.</span></span>|
|<span data-ttu-id="da763-123">失敗しました。</span><span class="sxs-lookup"><span data-stu-id="da763-123">failed</span></span>|<span data-ttu-id="da763-124">4</span><span class="sxs-lookup"><span data-stu-id="da763-124">4</span></span>|<span data-ttu-id="da763-125">処理に失敗しました。</span><span class="sxs-lookup"><span data-stu-id="da763-125">The operation failed.</span></span>|
