---
title: mobileAppIntent 列挙型
description: デバイスのモバイル アプリケーションのステータスを示します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8b8119cd188823beabf5b273e5324d0098e5b9ff
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875412"
---
# <a name="mobileappintent-enum-type"></a><span data-ttu-id="d6e9e-103">mobileAppIntent 列挙型</span><span class="sxs-lookup"><span data-stu-id="d6e9e-103">mobileAppIntent enum type</span></span>

> <span data-ttu-id="d6e9e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d6e9e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d6e9e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d6e9e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d6e9e-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d6e9e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d6e9e-107">デバイスのモバイル アプリケーションのステータスを示します。</span><span class="sxs-lookup"><span data-stu-id="d6e9e-107">Indicates the status of the mobile app on the device.</span></span>
## <a name="members"></a><span data-ttu-id="d6e9e-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="d6e9e-108">Members</span></span>
|<span data-ttu-id="d6e9e-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="d6e9e-109">Member</span></span>|<span data-ttu-id="d6e9e-110">値</span><span class="sxs-lookup"><span data-stu-id="d6e9e-110">Value</span></span>|<span data-ttu-id="d6e9e-111">説明</span><span class="sxs-lookup"><span data-stu-id="d6e9e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6e9e-112">使用可能</span><span class="sxs-lookup"><span data-stu-id="d6e9e-112">available</span></span>|<span data-ttu-id="d6e9e-113">0</span><span class="sxs-lookup"><span data-stu-id="d6e9e-113">0</span></span>|<span data-ttu-id="d6e9e-114">Available</span><span class="sxs-lookup"><span data-stu-id="d6e9e-114">Available</span></span>|
|<span data-ttu-id="d6e9e-115">送出</span><span class="sxs-lookup"><span data-stu-id="d6e9e-115">notAvailable</span></span>|<span data-ttu-id="d6e9e-116">1</span><span class="sxs-lookup"><span data-stu-id="d6e9e-116">1</span></span>|<span data-ttu-id="d6e9e-117">利用できません。</span><span class="sxs-lookup"><span data-stu-id="d6e9e-117">Not Available</span></span>|
|<span data-ttu-id="d6e9e-118">requiredInstall</span><span class="sxs-lookup"><span data-stu-id="d6e9e-118">requiredInstall</span></span>|<span data-ttu-id="d6e9e-119">2</span><span class="sxs-lookup"><span data-stu-id="d6e9e-119">2</span></span>|<span data-ttu-id="d6e9e-120">必要なインストール</span><span class="sxs-lookup"><span data-stu-id="d6e9e-120">Required Install</span></span>|
|<span data-ttu-id="d6e9e-121">requiredUninstall</span><span class="sxs-lookup"><span data-stu-id="d6e9e-121">requiredUninstall</span></span>|<span data-ttu-id="d6e9e-122">3</span><span class="sxs-lookup"><span data-stu-id="d6e9e-122">3</span></span>|<span data-ttu-id="d6e9e-123">必要なアンインストール</span><span class="sxs-lookup"><span data-stu-id="d6e9e-123">Required Uninstall</span></span>|
|<span data-ttu-id="d6e9e-124">requiredAndAvailableInstall</span><span class="sxs-lookup"><span data-stu-id="d6e9e-124">requiredAndAvailableInstall</span></span>|<span data-ttu-id="d6e9e-125">4</span><span class="sxs-lookup"><span data-stu-id="d6e9e-125">4</span></span>|<span data-ttu-id="d6e9e-126">RequiredAndAvailableInstall</span><span class="sxs-lookup"><span data-stu-id="d6e9e-126">RequiredAndAvailableInstall</span></span>|
|<span data-ttu-id="d6e9e-127">availableInstallWithoutEnrollment</span><span class="sxs-lookup"><span data-stu-id="d6e9e-127">availableInstallWithoutEnrollment</span></span>|<span data-ttu-id="d6e9e-128">5</span><span class="sxs-lookup"><span data-stu-id="d6e9e-128">5</span></span>|<span data-ttu-id="d6e9e-129">AvailableInstallWithoutEnrollment</span><span class="sxs-lookup"><span data-stu-id="d6e9e-129">AvailableInstallWithoutEnrollment</span></span>|
|<span data-ttu-id="d6e9e-130">除外</span><span class="sxs-lookup"><span data-stu-id="d6e9e-130">exclude</span></span>|<span data-ttu-id="d6e9e-131">6</span><span class="sxs-lookup"><span data-stu-id="d6e9e-131">6</span></span>|<span data-ttu-id="d6e9e-132">除外</span><span class="sxs-lookup"><span data-stu-id="d6e9e-132">Exclude</span></span>|





