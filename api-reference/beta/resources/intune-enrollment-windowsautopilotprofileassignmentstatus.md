---
title: windowsAutopilotProfileAssignmentStatus 列挙型
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d241d93924de254af3cb76adfab27b49291b97f2
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941395"
---
# <a name="windowsautopilotprofileassignmentstatus-enum-type"></a><span data-ttu-id="d59ec-103">windowsAutopilotProfileAssignmentStatus 列挙型</span><span class="sxs-lookup"><span data-stu-id="d59ec-103">windowsAutopilotProfileAssignmentStatus enum type</span></span>

> <span data-ttu-id="d59ec-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d59ec-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d59ec-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d59ec-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d59ec-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="d59ec-106">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="d59ec-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="d59ec-107">Members</span></span>
|<span data-ttu-id="d59ec-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="d59ec-108">Member</span></span>|<span data-ttu-id="d59ec-109">値</span><span class="sxs-lookup"><span data-stu-id="d59ec-109">Value</span></span>|<span data-ttu-id="d59ec-110">説明</span><span class="sxs-lookup"><span data-stu-id="d59ec-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d59ec-111">不明</span><span class="sxs-lookup"><span data-stu-id="d59ec-111">unknown</span></span>|<span data-ttu-id="d59ec-112">.0</span><span class="sxs-lookup"><span data-stu-id="d59ec-112">0</span></span>|<span data-ttu-id="d59ec-113">不明な割り当て状態</span><span class="sxs-lookup"><span data-stu-id="d59ec-113">Unknown assignment status</span></span>|
|<span data-ttu-id="d59ec-114">assignedInSync</span><span class="sxs-lookup"><span data-stu-id="d59ec-114">assignedInSync</span></span>|<span data-ttu-id="d59ec-115">1-d</span><span class="sxs-lookup"><span data-stu-id="d59ec-115">1</span></span>|<span data-ttu-id="d59ec-116">Intune で正常に割り当てられ、Windows 自動パイロットプログラムとの同期</span><span class="sxs-lookup"><span data-stu-id="d59ec-116">Assigned successfully in Intune and in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="d59ec-117">assignedOutOfSync</span><span class="sxs-lookup"><span data-stu-id="d59ec-117">assignedOutOfSync</span></span>|<span data-ttu-id="d59ec-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="d59ec-118">2</span></span>|<span data-ttu-id="d59ec-119">Intune で正常に割り当てられ、Windows 自動パイロットプログラムと同期されません</span><span class="sxs-lookup"><span data-stu-id="d59ec-119">Assigned successfully in Intune and not in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="d59ec-120">assignedUnkownSyncState</span><span class="sxs-lookup"><span data-stu-id="d59ec-120">assignedUnkownSyncState</span></span>|<span data-ttu-id="d59ec-121">1/3</span><span class="sxs-lookup"><span data-stu-id="d59ec-121">3</span></span>|<span data-ttu-id="d59ec-122">Intune で正常に割り当てられ、Windows 自動パイロットプログラムとの間で同期されているか、同期されていません</span><span class="sxs-lookup"><span data-stu-id="d59ec-122">Assigned successfully in Intune and either in-sync or out of sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="d59ec-123">notAssigned</span><span class="sxs-lookup"><span data-stu-id="d59ec-123">notAssigned</span></span>|<span data-ttu-id="d59ec-124">2/4</span><span class="sxs-lookup"><span data-stu-id="d59ec-124">4</span></span>|<span data-ttu-id="d59ec-125">未割り当て</span><span class="sxs-lookup"><span data-stu-id="d59ec-125">Not assigned</span></span>|
|<span data-ttu-id="d59ec-126">対する</span><span class="sxs-lookup"><span data-stu-id="d59ec-126">pending</span></span>|<span data-ttu-id="d59ec-127">5</span><span class="sxs-lookup"><span data-stu-id="d59ec-127">5</span></span>|<span data-ttu-id="d59ec-128">保留中の割り当て</span><span class="sxs-lookup"><span data-stu-id="d59ec-128">Pending assignment</span></span>|
|<span data-ttu-id="d59ec-129">フェール</span><span class="sxs-lookup"><span data-stu-id="d59ec-129">failed</span></span>|<span data-ttu-id="d59ec-130">シックス</span><span class="sxs-lookup"><span data-stu-id="d59ec-130">6</span></span>| <span data-ttu-id="d59ec-131">割り当て失敗</span><span class="sxs-lookup"><span data-stu-id="d59ec-131">Assignment failed</span></span>|




