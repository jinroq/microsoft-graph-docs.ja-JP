---
title: mobileAppIntent 列挙型
description: デバイスのモバイル アプリケーションのステータスを示します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a807e89ec949c2c48f04af46b26f43b393cc4b0a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419262"
---
# <a name="mobileappintent-enum-type"></a><span data-ttu-id="a4979-103">mobileAppIntent 列挙型</span><span class="sxs-lookup"><span data-stu-id="a4979-103">mobileAppIntent enum type</span></span>

> <span data-ttu-id="a4979-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a4979-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a4979-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a4979-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a4979-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a4979-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4979-107">デバイスのモバイル アプリケーションのステータスを示します。</span><span class="sxs-lookup"><span data-stu-id="a4979-107">Indicates the status of the mobile app on the device.</span></span>

## <a name="members"></a><span data-ttu-id="a4979-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="a4979-108">Members</span></span>
|<span data-ttu-id="a4979-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="a4979-109">Member</span></span>|<span data-ttu-id="a4979-110">値</span><span class="sxs-lookup"><span data-stu-id="a4979-110">Value</span></span>|<span data-ttu-id="a4979-111">説明</span><span class="sxs-lookup"><span data-stu-id="a4979-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4979-112">使用可能</span><span class="sxs-lookup"><span data-stu-id="a4979-112">available</span></span>|<span data-ttu-id="a4979-113">0</span><span class="sxs-lookup"><span data-stu-id="a4979-113">0</span></span>|<span data-ttu-id="a4979-114">Available</span><span class="sxs-lookup"><span data-stu-id="a4979-114">Available</span></span>|
|<span data-ttu-id="a4979-115">送出</span><span class="sxs-lookup"><span data-stu-id="a4979-115">notAvailable</span></span>|<span data-ttu-id="a4979-116">1</span><span class="sxs-lookup"><span data-stu-id="a4979-116">1</span></span>|<span data-ttu-id="a4979-117">利用できません。</span><span class="sxs-lookup"><span data-stu-id="a4979-117">Not Available</span></span>|
|<span data-ttu-id="a4979-118">requiredInstall</span><span class="sxs-lookup"><span data-stu-id="a4979-118">requiredInstall</span></span>|<span data-ttu-id="a4979-119">2</span><span class="sxs-lookup"><span data-stu-id="a4979-119">2</span></span>|<span data-ttu-id="a4979-120">必要なインストール</span><span class="sxs-lookup"><span data-stu-id="a4979-120">Required Install</span></span>|
|<span data-ttu-id="a4979-121">requiredUninstall</span><span class="sxs-lookup"><span data-stu-id="a4979-121">requiredUninstall</span></span>|<span data-ttu-id="a4979-122">3</span><span class="sxs-lookup"><span data-stu-id="a4979-122">3</span></span>|<span data-ttu-id="a4979-123">必要なアンインストール</span><span class="sxs-lookup"><span data-stu-id="a4979-123">Required Uninstall</span></span>|
|<span data-ttu-id="a4979-124">requiredAndAvailableInstall</span><span class="sxs-lookup"><span data-stu-id="a4979-124">requiredAndAvailableInstall</span></span>|<span data-ttu-id="a4979-125">4</span><span class="sxs-lookup"><span data-stu-id="a4979-125">4</span></span>|<span data-ttu-id="a4979-126">RequiredAndAvailableInstall</span><span class="sxs-lookup"><span data-stu-id="a4979-126">RequiredAndAvailableInstall</span></span>|
|<span data-ttu-id="a4979-127">availableInstallWithoutEnrollment</span><span class="sxs-lookup"><span data-stu-id="a4979-127">availableInstallWithoutEnrollment</span></span>|<span data-ttu-id="a4979-128">5</span><span class="sxs-lookup"><span data-stu-id="a4979-128">5</span></span>|<span data-ttu-id="a4979-129">AvailableInstallWithoutEnrollment</span><span class="sxs-lookup"><span data-stu-id="a4979-129">AvailableInstallWithoutEnrollment</span></span>|
|<span data-ttu-id="a4979-130">除外</span><span class="sxs-lookup"><span data-stu-id="a4979-130">exclude</span></span>|<span data-ttu-id="a4979-131">6</span><span class="sxs-lookup"><span data-stu-id="a4979-131">6</span></span>|<span data-ttu-id="a4979-132">除外</span><span class="sxs-lookup"><span data-stu-id="a4979-132">Exclude</span></span>|




