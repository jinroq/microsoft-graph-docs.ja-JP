---
title: mobileAppIntent 列挙型
description: デバイスのモバイル アプリケーションのステータスを示します。
ms.openlocfilehash: 52d704f19379e2ac6232a37926185fd5d78c2e72
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072295"
---
# <a name="mobileappintent-enum-type"></a><span data-ttu-id="7ce86-103">mobileAppIntent 列挙型</span><span class="sxs-lookup"><span data-stu-id="7ce86-103">mobileAppIntent enum type</span></span>

> <span data-ttu-id="7ce86-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7ce86-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7ce86-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7ce86-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7ce86-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7ce86-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7ce86-107">デバイスのモバイル アプリケーションのステータスを示します。</span><span class="sxs-lookup"><span data-stu-id="7ce86-107">Indicates the status of the mobile app on the device.</span></span>
## <a name="members"></a><span data-ttu-id="7ce86-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="7ce86-108">Members</span></span>
|<span data-ttu-id="7ce86-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="7ce86-109">Member</span></span>|<span data-ttu-id="7ce86-110">値</span><span class="sxs-lookup"><span data-stu-id="7ce86-110">Value</span></span>|<span data-ttu-id="7ce86-111">説明</span><span class="sxs-lookup"><span data-stu-id="7ce86-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ce86-112">使用可能</span><span class="sxs-lookup"><span data-stu-id="7ce86-112">available</span></span>|<span data-ttu-id="7ce86-113">0</span><span class="sxs-lookup"><span data-stu-id="7ce86-113">0</span></span>|<span data-ttu-id="7ce86-114">Available</span><span class="sxs-lookup"><span data-stu-id="7ce86-114">Available</span></span>|
|<span data-ttu-id="7ce86-115">送出</span><span class="sxs-lookup"><span data-stu-id="7ce86-115">notAvailable</span></span>|<span data-ttu-id="7ce86-116">1</span><span class="sxs-lookup"><span data-stu-id="7ce86-116">1</span></span>|<span data-ttu-id="7ce86-117">利用できません。</span><span class="sxs-lookup"><span data-stu-id="7ce86-117">Not Available</span></span>|
|<span data-ttu-id="7ce86-118">requiredInstall</span><span class="sxs-lookup"><span data-stu-id="7ce86-118">requiredInstall</span></span>|<span data-ttu-id="7ce86-119">2</span><span class="sxs-lookup"><span data-stu-id="7ce86-119">2</span></span>|<span data-ttu-id="7ce86-120">必要なインストール</span><span class="sxs-lookup"><span data-stu-id="7ce86-120">Required Install</span></span>|
|<span data-ttu-id="7ce86-121">requiredUninstall</span><span class="sxs-lookup"><span data-stu-id="7ce86-121">requiredUninstall</span></span>|<span data-ttu-id="7ce86-122">3</span><span class="sxs-lookup"><span data-stu-id="7ce86-122">3</span></span>|<span data-ttu-id="7ce86-123">必要なアンインストール</span><span class="sxs-lookup"><span data-stu-id="7ce86-123">Required Uninstall</span></span>|
|<span data-ttu-id="7ce86-124">requiredAndAvailableInstall</span><span class="sxs-lookup"><span data-stu-id="7ce86-124">requiredAndAvailableInstall</span></span>|<span data-ttu-id="7ce86-125">4</span><span class="sxs-lookup"><span data-stu-id="7ce86-125">4</span></span>|<span data-ttu-id="7ce86-126">RequiredAndAvailableInstall</span><span class="sxs-lookup"><span data-stu-id="7ce86-126">RequiredAndAvailableInstall</span></span>|
|<span data-ttu-id="7ce86-127">availableInstallWithoutEnrollment</span><span class="sxs-lookup"><span data-stu-id="7ce86-127">availableInstallWithoutEnrollment</span></span>|<span data-ttu-id="7ce86-128">5</span><span class="sxs-lookup"><span data-stu-id="7ce86-128">5</span></span>|<span data-ttu-id="7ce86-129">AvailableInstallWithoutEnrollment</span><span class="sxs-lookup"><span data-stu-id="7ce86-129">AvailableInstallWithoutEnrollment</span></span>|
|<span data-ttu-id="7ce86-130">除外</span><span class="sxs-lookup"><span data-stu-id="7ce86-130">exclude</span></span>|<span data-ttu-id="7ce86-131">6</span><span class="sxs-lookup"><span data-stu-id="7ce86-131">6</span></span>|<span data-ttu-id="7ce86-132">除外</span><span class="sxs-lookup"><span data-stu-id="7ce86-132">Exclude</span></span>|





