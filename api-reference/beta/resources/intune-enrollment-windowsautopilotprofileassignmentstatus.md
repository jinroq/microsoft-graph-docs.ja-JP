---
title: windowsAutopilotProfileAssignmentStatus 列挙型
description: まだ文書化されていません
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 68612e2f4ccee46612c82237630efafda484b7e9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419122"
---
# <a name="windowsautopilotprofileassignmentstatus-enum-type"></a><span data-ttu-id="b1651-103">windowsAutopilotProfileAssignmentStatus 列挙型</span><span class="sxs-lookup"><span data-stu-id="b1651-103">windowsAutopilotProfileAssignmentStatus enum type</span></span>

> <span data-ttu-id="b1651-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b1651-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b1651-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b1651-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b1651-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b1651-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1651-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="b1651-107">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="b1651-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="b1651-108">Members</span></span>
|<span data-ttu-id="b1651-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="b1651-109">Member</span></span>|<span data-ttu-id="b1651-110">値</span><span class="sxs-lookup"><span data-stu-id="b1651-110">Value</span></span>|<span data-ttu-id="b1651-111">説明</span><span class="sxs-lookup"><span data-stu-id="b1651-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1651-112">不明</span><span class="sxs-lookup"><span data-stu-id="b1651-112">unknown</span></span>|<span data-ttu-id="b1651-113">0</span><span class="sxs-lookup"><span data-stu-id="b1651-113">0</span></span>|<span data-ttu-id="b1651-114">不明な割り当ての状態</span><span class="sxs-lookup"><span data-stu-id="b1651-114">Unknown assignment status</span></span>|
|<span data-ttu-id="b1651-115">assignedInSync</span><span class="sxs-lookup"><span data-stu-id="b1651-115">assignedInSync</span></span>|<span data-ttu-id="b1651-116">1</span><span class="sxs-lookup"><span data-stu-id="b1651-116">1</span></span>|<span data-ttu-id="b1651-117">Intune で正常に割り当てられていると Windows の自動パイロット プログラムとの同期</span><span class="sxs-lookup"><span data-stu-id="b1651-117">Assigned successfully in Intune and in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="b1651-118">assignedOutOfSync</span><span class="sxs-lookup"><span data-stu-id="b1651-118">assignedOutOfSync</span></span>|<span data-ttu-id="b1651-119">2</span><span class="sxs-lookup"><span data-stu-id="b1651-119">2</span></span>|<span data-ttu-id="b1651-120">Intune で正常に割り当てられているといないと同期させる Windows 自動パイロット プログラム</span><span class="sxs-lookup"><span data-stu-id="b1651-120">Assigned successfully in Intune and not in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="b1651-121">assignedUnkownSyncState</span><span class="sxs-lookup"><span data-stu-id="b1651-121">assignedUnkownSyncState</span></span>|<span data-ttu-id="b1651-122">3</span><span class="sxs-lookup"><span data-stu-id="b1651-122">3</span></span>|<span data-ttu-id="b1651-123">Intune といずれかの同期で正常に割り当てられているまたは Windows 自動パイロット プログラムとの同期</span><span class="sxs-lookup"><span data-stu-id="b1651-123">Assigned successfully in Intune and either in-sync or out of sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="b1651-124">notAssigned</span><span class="sxs-lookup"><span data-stu-id="b1651-124">notAssigned</span></span>|<span data-ttu-id="b1651-125">4</span><span class="sxs-lookup"><span data-stu-id="b1651-125">4</span></span>|<span data-ttu-id="b1651-126">割り当てられていません。</span><span class="sxs-lookup"><span data-stu-id="b1651-126">Not assigned</span></span>|
|<span data-ttu-id="b1651-127">保留中</span><span class="sxs-lookup"><span data-stu-id="b1651-127">pending</span></span>|<span data-ttu-id="b1651-128">5</span><span class="sxs-lookup"><span data-stu-id="b1651-128">5</span></span>|<span data-ttu-id="b1651-129">保留中の割り当て</span><span class="sxs-lookup"><span data-stu-id="b1651-129">Pending assignment</span></span>|
|<span data-ttu-id="b1651-130">失敗しました。</span><span class="sxs-lookup"><span data-stu-id="b1651-130">failed</span></span>|<span data-ttu-id="b1651-131">6</span><span class="sxs-lookup"><span data-stu-id="b1651-131">6</span></span>| <span data-ttu-id="b1651-132">割り当てに失敗しました。</span><span class="sxs-lookup"><span data-stu-id="b1651-132">Assignment failed</span></span>|




