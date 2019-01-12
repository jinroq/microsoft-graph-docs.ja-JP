---
title: windowsAutopilotProfileAssignmentStatus 列挙型
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1427ffeb45862312d92fdf02a00a242725894d36
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962633"
---
# <a name="windowsautopilotprofileassignmentstatus-enum-type"></a><span data-ttu-id="9f526-103">windowsAutopilotProfileAssignmentStatus 列挙型</span><span class="sxs-lookup"><span data-stu-id="9f526-103">windowsAutopilotProfileAssignmentStatus enum type</span></span>

> <span data-ttu-id="9f526-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9f526-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9f526-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9f526-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9f526-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9f526-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9f526-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="9f526-107">Not yet documented</span></span>
## <a name="members"></a><span data-ttu-id="9f526-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="9f526-108">Members</span></span>
|<span data-ttu-id="9f526-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="9f526-109">Member</span></span>|<span data-ttu-id="9f526-110">値</span><span class="sxs-lookup"><span data-stu-id="9f526-110">Value</span></span>|<span data-ttu-id="9f526-111">説明</span><span class="sxs-lookup"><span data-stu-id="9f526-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f526-112">不明</span><span class="sxs-lookup"><span data-stu-id="9f526-112">unknown</span></span>|<span data-ttu-id="9f526-113">0</span><span class="sxs-lookup"><span data-stu-id="9f526-113">0</span></span>|<span data-ttu-id="9f526-114">不明な割り当ての状態</span><span class="sxs-lookup"><span data-stu-id="9f526-114">Unknown assignment status</span></span>|
|<span data-ttu-id="9f526-115">assignedInSync</span><span class="sxs-lookup"><span data-stu-id="9f526-115">assignedInSync</span></span>|<span data-ttu-id="9f526-116">1</span><span class="sxs-lookup"><span data-stu-id="9f526-116">1</span></span>|<span data-ttu-id="9f526-117">Intune で正常に割り当てられていると Windows の自動パイロット プログラムとの同期</span><span class="sxs-lookup"><span data-stu-id="9f526-117">Assigned successfully in Intune and in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="9f526-118">assignedOutOfSync</span><span class="sxs-lookup"><span data-stu-id="9f526-118">assignedOutOfSync</span></span>|<span data-ttu-id="9f526-119">2</span><span class="sxs-lookup"><span data-stu-id="9f526-119">2</span></span>|<span data-ttu-id="9f526-120">Intune で正常に割り当てられているといないと同期させる Windows 自動パイロット プログラム</span><span class="sxs-lookup"><span data-stu-id="9f526-120">Assigned successfully in Intune and not in sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="9f526-121">assignedUnkownSyncState</span><span class="sxs-lookup"><span data-stu-id="9f526-121">assignedUnkownSyncState</span></span>|<span data-ttu-id="9f526-122">3</span><span class="sxs-lookup"><span data-stu-id="9f526-122">3</span></span>|<span data-ttu-id="9f526-123">Intune といずれかの同期で正常に割り当てられているまたは Windows 自動パイロット プログラムとの同期</span><span class="sxs-lookup"><span data-stu-id="9f526-123">Assigned successfully in Intune and either in-sync or out of sync with Windows auto pilot program</span></span>|
|<span data-ttu-id="9f526-124">notAssigned</span><span class="sxs-lookup"><span data-stu-id="9f526-124">notAssigned</span></span>|<span data-ttu-id="9f526-125">4</span><span class="sxs-lookup"><span data-stu-id="9f526-125">4</span></span>|<span data-ttu-id="9f526-126">割り当てられていません。</span><span class="sxs-lookup"><span data-stu-id="9f526-126">Not assigned</span></span>|
|<span data-ttu-id="9f526-127">保留中</span><span class="sxs-lookup"><span data-stu-id="9f526-127">pending</span></span>|<span data-ttu-id="9f526-128">5</span><span class="sxs-lookup"><span data-stu-id="9f526-128">5</span></span>|<span data-ttu-id="9f526-129">保留中の割り当て</span><span class="sxs-lookup"><span data-stu-id="9f526-129">Pending assignment</span></span>|
|<span data-ttu-id="9f526-130">失敗しました。</span><span class="sxs-lookup"><span data-stu-id="9f526-130">failed</span></span>|<span data-ttu-id="9f526-131">6</span><span class="sxs-lookup"><span data-stu-id="9f526-131">6</span></span>| <span data-ttu-id="9f526-132">割り当てに失敗しました。</span><span class="sxs-lookup"><span data-stu-id="9f526-132">Assignment failed</span></span>|





