---
title: windowsAutopilotProfileAssignmentStatus 列挙型
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5f4c6fbfcbefd88af31f2875cf33755b3be21e06
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31773190"
---
# <a name="windowsautopilotprofileassignmentstatus-enum-type"></a><span data-ttu-id="9d86a-103">windowsAutopilotProfileAssignmentStatus 列挙型</span><span class="sxs-lookup"><span data-stu-id="9d86a-103">windowsAutopilotProfileAssignmentStatus enum type</span></span>

> <span data-ttu-id="9d86a-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9d86a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9d86a-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9d86a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9d86a-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="9d86a-106">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="9d86a-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="9d86a-107">Members</span></span>
|<span data-ttu-id="9d86a-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="9d86a-108">Member</span></span>|<span data-ttu-id="9d86a-109">値</span><span class="sxs-lookup"><span data-stu-id="9d86a-109">Value</span></span>|<span data-ttu-id="9d86a-110">説明</span><span class="sxs-lookup"><span data-stu-id="9d86a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d86a-111">不明</span><span class="sxs-lookup"><span data-stu-id="9d86a-111">unknown</span></span>|<span data-ttu-id="9d86a-112">.0</span><span class="sxs-lookup"><span data-stu-id="9d86a-112">0</span></span>|<span data-ttu-id="9d86a-113">不明な割り当て状態</span><span class="sxs-lookup"><span data-stu-id="9d86a-113">Unknown assignment status</span></span>|
|<span data-ttu-id="9d86a-114">assignedInSync</span><span class="sxs-lookup"><span data-stu-id="9d86a-114">assignedInSync</span></span>|<span data-ttu-id="9d86a-115">1-d</span><span class="sxs-lookup"><span data-stu-id="9d86a-115">1</span></span>|<span data-ttu-id="9d86a-116">Intune で正常に割り当てられ、Windows 自動パイロットプログラムとの同期</span><span class="sxs-lookup"><span data-stu-id="9d86a-116">Assigned successfully in Intune and in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="9d86a-117">assignedOutOfSync</span><span class="sxs-lookup"><span data-stu-id="9d86a-117">assignedOutOfSync</span></span>|<span data-ttu-id="9d86a-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="9d86a-118">2</span></span>|<span data-ttu-id="9d86a-119">Intune で正常に割り当てられ、Windows 自動パイロットプログラムと同期されません</span><span class="sxs-lookup"><span data-stu-id="9d86a-119">Assigned successfully in Intune and not in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="9d86a-120">assignedUnkownSyncState</span><span class="sxs-lookup"><span data-stu-id="9d86a-120">assignedUnkownSyncState</span></span>|<span data-ttu-id="9d86a-121">1/3</span><span class="sxs-lookup"><span data-stu-id="9d86a-121">3</span></span>|<span data-ttu-id="9d86a-122">Intune で正常に割り当てられ、Windows 自動パイロットプログラムとの間で同期されているか、同期されていません</span><span class="sxs-lookup"><span data-stu-id="9d86a-122">Assigned successfully in Intune and either in-sync or out of sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="9d86a-123">notAssigned</span><span class="sxs-lookup"><span data-stu-id="9d86a-123">notAssigned</span></span>|<span data-ttu-id="9d86a-124">2/4</span><span class="sxs-lookup"><span data-stu-id="9d86a-124">4</span></span>|<span data-ttu-id="9d86a-125">未割り当て</span><span class="sxs-lookup"><span data-stu-id="9d86a-125">Not assigned</span></span>|
|<span data-ttu-id="9d86a-126">対する</span><span class="sxs-lookup"><span data-stu-id="9d86a-126">pending</span></span>|<span data-ttu-id="9d86a-127">5</span><span class="sxs-lookup"><span data-stu-id="9d86a-127">5</span></span>|<span data-ttu-id="9d86a-128">保留中の割り当て</span><span class="sxs-lookup"><span data-stu-id="9d86a-128">Pending assignment</span></span>|
|<span data-ttu-id="9d86a-129">フェール</span><span class="sxs-lookup"><span data-stu-id="9d86a-129">failed</span></span>|<span data-ttu-id="9d86a-130">シックス</span><span class="sxs-lookup"><span data-stu-id="9d86a-130">6</span></span>| <span data-ttu-id="9d86a-131">割り当て失敗</span><span class="sxs-lookup"><span data-stu-id="9d86a-131">Assignment failed</span></span>|





