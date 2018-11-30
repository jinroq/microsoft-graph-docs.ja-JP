---
title: teamsAsyncOperationStatus 列挙型
description: TeamsAsyncOperation の現在の状態について説明します。
ms.openlocfilehash: f553242ace983651b8d4fda77370de712f9d08b6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067431"
---
# <a name="teamsasyncoperationstatus-enum-type"></a><span data-ttu-id="05e23-103">teamsAsyncOperationStatus 列挙型</span><span class="sxs-lookup"><span data-stu-id="05e23-103">teamsAsyncOperationStatus enum type</span></span>

> <span data-ttu-id="05e23-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="05e23-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="05e23-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="05e23-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="05e23-106">の[teamsAsyncOperation](teamsasyncoperation.md)の現在の状態について説明します。</span><span class="sxs-lookup"><span data-stu-id="05e23-106">Describes the current status of a [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="members"></a><span data-ttu-id="05e23-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="05e23-107">Members</span></span>

| <span data-ttu-id="05e23-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="05e23-108">Member</span></span> | <span data-ttu-id="05e23-109">値</span><span class="sxs-lookup"><span data-stu-id="05e23-109">Value</span></span>| <span data-ttu-id="05e23-110">説明</span><span class="sxs-lookup"><span data-stu-id="05e23-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="05e23-111">無効です</span><span class="sxs-lookup"><span data-stu-id="05e23-111">invalid</span></span>|<span data-ttu-id="05e23-112">0</span><span class="sxs-lookup"><span data-stu-id="05e23-112">0</span></span>|<span data-ttu-id="05e23-113">値が無効です。</span><span class="sxs-lookup"><span data-stu-id="05e23-113">Invalid value.</span></span>|
|<span data-ttu-id="05e23-114">未開始</span><span class="sxs-lookup"><span data-stu-id="05e23-114">notStarted</span></span>|<span data-ttu-id="05e23-115">1</span><span class="sxs-lookup"><span data-stu-id="05e23-115">1</span></span>|<span data-ttu-id="05e23-116">操作は開始されていません。</span><span class="sxs-lookup"><span data-stu-id="05e23-116">The operation has not started.</span></span>|
|<span data-ttu-id="05e23-117">inProgress</span><span class="sxs-lookup"><span data-stu-id="05e23-117">inProgress</span></span>|<span data-ttu-id="05e23-118">2</span><span class="sxs-lookup"><span data-stu-id="05e23-118">2</span></span>|<span data-ttu-id="05e23-119">操作が行われています。</span><span class="sxs-lookup"><span data-stu-id="05e23-119">The operation is running.</span></span>|
|<span data-ttu-id="05e23-120">成功しました</span><span class="sxs-lookup"><span data-stu-id="05e23-120">succeeded</span></span>|<span data-ttu-id="05e23-121">3</span><span class="sxs-lookup"><span data-stu-id="05e23-121">3</span></span>|<span data-ttu-id="05e23-122">操作が正常に完了しました。</span><span class="sxs-lookup"><span data-stu-id="05e23-122">The operation succeeded.</span></span>|
|<span data-ttu-id="05e23-123">失敗しました。</span><span class="sxs-lookup"><span data-stu-id="05e23-123">failed</span></span>|<span data-ttu-id="05e23-124">4</span><span class="sxs-lookup"><span data-stu-id="05e23-124">4</span></span>|<span data-ttu-id="05e23-125">処理に失敗しました。</span><span class="sxs-lookup"><span data-stu-id="05e23-125">The operation failed.</span></span>|