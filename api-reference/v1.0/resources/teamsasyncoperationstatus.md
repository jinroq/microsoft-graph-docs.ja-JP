---
title: teamsAsyncOperationStatus 列挙型
description: TeamsAsyncOperation の現在の状態について説明します。
author: nkramer
ms.openlocfilehash: fbf66ac0c93fd616793ebb4dc62fb63a2559374f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309969"
---
# <a name="teamsasyncoperationstatus-enum-type"></a><span data-ttu-id="8a1f0-103">teamsAsyncOperationStatus 列挙型</span><span class="sxs-lookup"><span data-stu-id="8a1f0-103">teamsAsyncOperationStatus enum type</span></span>



<span data-ttu-id="8a1f0-104">の[teamsAsyncOperation](teamsasyncoperation.md)の現在の状態について説明します。</span><span class="sxs-lookup"><span data-stu-id="8a1f0-104">Describes the current status of a [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="members"></a><span data-ttu-id="8a1f0-105">メンバー</span><span class="sxs-lookup"><span data-stu-id="8a1f0-105">Members</span></span>

| <span data-ttu-id="8a1f0-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="8a1f0-106">Member</span></span> | <span data-ttu-id="8a1f0-107">値</span><span class="sxs-lookup"><span data-stu-id="8a1f0-107">Value</span></span>| <span data-ttu-id="8a1f0-108">説明</span><span class="sxs-lookup"><span data-stu-id="8a1f0-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="8a1f0-109">無効です</span><span class="sxs-lookup"><span data-stu-id="8a1f0-109">invalid</span></span>|<span data-ttu-id="8a1f0-110">0</span><span class="sxs-lookup"><span data-stu-id="8a1f0-110">0</span></span>|<span data-ttu-id="8a1f0-111">値が無効です。</span><span class="sxs-lookup"><span data-stu-id="8a1f0-111">Invalid value.</span></span>|
|<span data-ttu-id="8a1f0-112">未開始</span><span class="sxs-lookup"><span data-stu-id="8a1f0-112">notStarted</span></span>|<span data-ttu-id="8a1f0-113">1</span><span class="sxs-lookup"><span data-stu-id="8a1f0-113">1</span></span>|<span data-ttu-id="8a1f0-114">操作は開始されていません。</span><span class="sxs-lookup"><span data-stu-id="8a1f0-114">The operation has not started.</span></span>|
|<span data-ttu-id="8a1f0-115">inProgress</span><span class="sxs-lookup"><span data-stu-id="8a1f0-115">inProgress</span></span>|<span data-ttu-id="8a1f0-116">2</span><span class="sxs-lookup"><span data-stu-id="8a1f0-116">2</span></span>|<span data-ttu-id="8a1f0-117">操作が行われています。</span><span class="sxs-lookup"><span data-stu-id="8a1f0-117">The operation is running.</span></span>|
|<span data-ttu-id="8a1f0-118">成功しました</span><span class="sxs-lookup"><span data-stu-id="8a1f0-118">succeeded</span></span>|<span data-ttu-id="8a1f0-119">3</span><span class="sxs-lookup"><span data-stu-id="8a1f0-119">3</span></span>|<span data-ttu-id="8a1f0-120">操作が正常に完了しました。</span><span class="sxs-lookup"><span data-stu-id="8a1f0-120">The operation succeeded.</span></span>|
|<span data-ttu-id="8a1f0-121">失敗しました。</span><span class="sxs-lookup"><span data-stu-id="8a1f0-121">failed</span></span>|<span data-ttu-id="8a1f0-122">4</span><span class="sxs-lookup"><span data-stu-id="8a1f0-122">4</span></span>|<span data-ttu-id="8a1f0-123">処理に失敗しました。</span><span class="sxs-lookup"><span data-stu-id="8a1f0-123">The operation failed.</span></span>|