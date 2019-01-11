---
title: windowsAutopilotProfileAssignmentStatus 列挙型
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 48d08ad4d4c80c3d5a68cca5af36c958deaac819
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869644"
---
# <a name="windowsautopilotprofileassignmentstatus-enum-type"></a><span data-ttu-id="97382-103">windowsAutopilotProfileAssignmentStatus 列挙型</span><span class="sxs-lookup"><span data-stu-id="97382-103">windowsAutopilotProfileAssignmentStatus enum type</span></span>

> <span data-ttu-id="97382-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="97382-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="97382-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="97382-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="97382-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="97382-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="97382-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="97382-107">Not yet documented</span></span>
## <a name="members"></a><span data-ttu-id="97382-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="97382-108">Members</span></span>
|<span data-ttu-id="97382-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="97382-109">Member</span></span>|<span data-ttu-id="97382-110">値</span><span class="sxs-lookup"><span data-stu-id="97382-110">Value</span></span>|<span data-ttu-id="97382-111">説明</span><span class="sxs-lookup"><span data-stu-id="97382-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97382-112">不明</span><span class="sxs-lookup"><span data-stu-id="97382-112">unknown</span></span>|<span data-ttu-id="97382-113">0</span><span class="sxs-lookup"><span data-stu-id="97382-113">0</span></span>|<span data-ttu-id="97382-114">不明な割り当ての状態</span><span class="sxs-lookup"><span data-stu-id="97382-114">Unknown assignment status</span></span>|
|<span data-ttu-id="97382-115">assignedInSync</span><span class="sxs-lookup"><span data-stu-id="97382-115">assignedInSync</span></span>|<span data-ttu-id="97382-116">1</span><span class="sxs-lookup"><span data-stu-id="97382-116">1</span></span>|<span data-ttu-id="97382-117">Intune で正常に割り当てられていると Windows の自動パイロット プログラムとの同期</span><span class="sxs-lookup"><span data-stu-id="97382-117">Assigned successfully in Intune and in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="97382-118">assignedOutOfSync</span><span class="sxs-lookup"><span data-stu-id="97382-118">assignedOutOfSync</span></span>|<span data-ttu-id="97382-119">2</span><span class="sxs-lookup"><span data-stu-id="97382-119">2</span></span>|<span data-ttu-id="97382-120">Intune で正常に割り当てられているといないと同期させる Windows 自動パイロット プログラム</span><span class="sxs-lookup"><span data-stu-id="97382-120">Assigned successfully in Intune and not in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="97382-121">assignedUnkownSyncState</span><span class="sxs-lookup"><span data-stu-id="97382-121">assignedUnkownSyncState</span></span>|<span data-ttu-id="97382-122">3</span><span class="sxs-lookup"><span data-stu-id="97382-122">3</span></span>|<span data-ttu-id="97382-123">Intune といずれかの同期で正常に割り当てられているまたは Windows 自動パイロット プログラムとの同期</span><span class="sxs-lookup"><span data-stu-id="97382-123">Assigned successfully in Intune and either in-sync or out of sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="97382-124">notAssigned</span><span class="sxs-lookup"><span data-stu-id="97382-124">notAssigned</span></span>|<span data-ttu-id="97382-125">4</span><span class="sxs-lookup"><span data-stu-id="97382-125">4</span></span>|<span data-ttu-id="97382-126">割り当てられていません。</span><span class="sxs-lookup"><span data-stu-id="97382-126">Not assigned</span></span>|
|<span data-ttu-id="97382-127">保留中</span><span class="sxs-lookup"><span data-stu-id="97382-127">pending</span></span>|<span data-ttu-id="97382-128">5</span><span class="sxs-lookup"><span data-stu-id="97382-128">5</span></span>|<span data-ttu-id="97382-129">保留中の割り当て</span><span class="sxs-lookup"><span data-stu-id="97382-129">Pending assignment</span></span>|
|<span data-ttu-id="97382-130">失敗しました。</span><span class="sxs-lookup"><span data-stu-id="97382-130">failed</span></span>|<span data-ttu-id="97382-131">6</span><span class="sxs-lookup"><span data-stu-id="97382-131">6</span></span>| <span data-ttu-id="97382-132">割り当てに失敗しました。</span><span class="sxs-lookup"><span data-stu-id="97382-132">Assignment failed</span></span>|





