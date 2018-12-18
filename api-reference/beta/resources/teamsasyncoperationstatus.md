---
title: teamsAsyncOperationStatus 列挙型
description: TeamsAsyncOperation の現在の状態について説明します。
author: nkramer
ms.openlocfilehash: 49b5b81999714627b1a1acd42df208594123b262
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27332005"
---
# <a name="teamsasyncoperationstatus-enum-type"></a><span data-ttu-id="c4533-103">teamsAsyncOperationStatus 列挙型</span><span class="sxs-lookup"><span data-stu-id="c4533-103">teamsAsyncOperationStatus enum type</span></span>

> <span data-ttu-id="c4533-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c4533-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c4533-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c4533-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c4533-106">の[teamsAsyncOperation](teamsasyncoperation.md)の現在の状態について説明します。</span><span class="sxs-lookup"><span data-stu-id="c4533-106">Describes the current status of a [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="members"></a><span data-ttu-id="c4533-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="c4533-107">Members</span></span>

| <span data-ttu-id="c4533-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="c4533-108">Member</span></span> | <span data-ttu-id="c4533-109">値</span><span class="sxs-lookup"><span data-stu-id="c4533-109">Value</span></span>| <span data-ttu-id="c4533-110">説明</span><span class="sxs-lookup"><span data-stu-id="c4533-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="c4533-111">無効です</span><span class="sxs-lookup"><span data-stu-id="c4533-111">invalid</span></span>|<span data-ttu-id="c4533-112">0</span><span class="sxs-lookup"><span data-stu-id="c4533-112">0</span></span>|<span data-ttu-id="c4533-113">値が無効です。</span><span class="sxs-lookup"><span data-stu-id="c4533-113">Invalid value.</span></span>|
|<span data-ttu-id="c4533-114">未開始</span><span class="sxs-lookup"><span data-stu-id="c4533-114">notStarted</span></span>|<span data-ttu-id="c4533-115">1</span><span class="sxs-lookup"><span data-stu-id="c4533-115">1</span></span>|<span data-ttu-id="c4533-116">操作は開始されていません。</span><span class="sxs-lookup"><span data-stu-id="c4533-116">The operation has not started.</span></span>|
|<span data-ttu-id="c4533-117">inProgress</span><span class="sxs-lookup"><span data-stu-id="c4533-117">inProgress</span></span>|<span data-ttu-id="c4533-118">2</span><span class="sxs-lookup"><span data-stu-id="c4533-118">2</span></span>|<span data-ttu-id="c4533-119">操作が行われています。</span><span class="sxs-lookup"><span data-stu-id="c4533-119">The operation is running.</span></span>|
|<span data-ttu-id="c4533-120">成功しました</span><span class="sxs-lookup"><span data-stu-id="c4533-120">succeeded</span></span>|<span data-ttu-id="c4533-121">3</span><span class="sxs-lookup"><span data-stu-id="c4533-121">3</span></span>|<span data-ttu-id="c4533-122">操作が正常に完了しました。</span><span class="sxs-lookup"><span data-stu-id="c4533-122">The operation succeeded.</span></span>|
|<span data-ttu-id="c4533-123">失敗しました。</span><span class="sxs-lookup"><span data-stu-id="c4533-123">failed</span></span>|<span data-ttu-id="c4533-124">4</span><span class="sxs-lookup"><span data-stu-id="c4533-124">4</span></span>|<span data-ttu-id="c4533-125">処理に失敗しました。</span><span class="sxs-lookup"><span data-stu-id="c4533-125">The operation failed.</span></span>|