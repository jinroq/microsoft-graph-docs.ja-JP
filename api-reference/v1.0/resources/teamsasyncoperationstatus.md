---
title: teamsAsyncOperationStatus 列挙型
description: TeamsAsyncOperation の現在の状態を表します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: enumPageType
ms.openlocfilehash: 4ffd6653752968c16d469ade39fc0e399fbee37c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033734"
---
# <a name="teamsasyncoperationstatus-enum-type"></a><span data-ttu-id="afbfa-103">teamsAsyncOperationStatus 列挙型</span><span class="sxs-lookup"><span data-stu-id="afbfa-103">teamsAsyncOperationStatus enum type</span></span>



<span data-ttu-id="afbfa-104">[TeamsAsyncOperation](teamsasyncoperation.md)の現在の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="afbfa-104">Describes the current status of a [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="members"></a><span data-ttu-id="afbfa-105">メンバー</span><span class="sxs-lookup"><span data-stu-id="afbfa-105">Members</span></span>

| <span data-ttu-id="afbfa-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="afbfa-106">Member</span></span> | <span data-ttu-id="afbfa-107">値</span><span class="sxs-lookup"><span data-stu-id="afbfa-107">Value</span></span>| <span data-ttu-id="afbfa-108">説明</span><span class="sxs-lookup"><span data-stu-id="afbfa-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="afbfa-109">無効です</span><span class="sxs-lookup"><span data-stu-id="afbfa-109">invalid</span></span>|<span data-ttu-id="afbfa-110">.0</span><span class="sxs-lookup"><span data-stu-id="afbfa-110">0</span></span>|<span data-ttu-id="afbfa-111">無効な値です。</span><span class="sxs-lookup"><span data-stu-id="afbfa-111">Invalid value.</span></span>|
|<span data-ttu-id="afbfa-112">notStarted</span><span class="sxs-lookup"><span data-stu-id="afbfa-112">notStarted</span></span>|<span data-ttu-id="afbfa-113">1-d</span><span class="sxs-lookup"><span data-stu-id="afbfa-113">1</span></span>|<span data-ttu-id="afbfa-114">操作は開始されていません。</span><span class="sxs-lookup"><span data-stu-id="afbfa-114">The operation has not started.</span></span>|
|<span data-ttu-id="afbfa-115">inProgress</span><span class="sxs-lookup"><span data-stu-id="afbfa-115">inProgress</span></span>|<span data-ttu-id="afbfa-116">pbm-2</span><span class="sxs-lookup"><span data-stu-id="afbfa-116">2</span></span>|<span data-ttu-id="afbfa-117">操作が実行されています。</span><span class="sxs-lookup"><span data-stu-id="afbfa-117">The operation is running.</span></span>|
|<span data-ttu-id="afbfa-118">失敗</span><span class="sxs-lookup"><span data-stu-id="afbfa-118">succeeded</span></span>|<span data-ttu-id="afbfa-119">1/3</span><span class="sxs-lookup"><span data-stu-id="afbfa-119">3</span></span>|<span data-ttu-id="afbfa-120">操作が正常に完了しました。</span><span class="sxs-lookup"><span data-stu-id="afbfa-120">The operation succeeded.</span></span>|
|<span data-ttu-id="afbfa-121">フェール</span><span class="sxs-lookup"><span data-stu-id="afbfa-121">failed</span></span>|<span data-ttu-id="afbfa-122">2/4</span><span class="sxs-lookup"><span data-stu-id="afbfa-122">4</span></span>|<span data-ttu-id="afbfa-123">操作は失敗しました。</span><span class="sxs-lookup"><span data-stu-id="afbfa-123">The operation failed.</span></span>|
