---
title: mobileAppIntent 列挙型
description: デバイス上のモバイルアプリの状態を示します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7f29c035b27a943649d10a3a71512630deb146f7
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34988140"
---
# <a name="mobileappintent-enum-type"></a><span data-ttu-id="0e7a9-103">mobileAppIntent 列挙型</span><span class="sxs-lookup"><span data-stu-id="0e7a9-103">mobileAppIntent enum type</span></span>

> <span data-ttu-id="0e7a9-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0e7a9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0e7a9-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0e7a9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e7a9-106">デバイス上のモバイルアプリの状態を示します。</span><span class="sxs-lookup"><span data-stu-id="0e7a9-106">Indicates the status of the mobile app on the device.</span></span>

## <a name="members"></a><span data-ttu-id="0e7a9-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="0e7a9-107">Members</span></span>
|<span data-ttu-id="0e7a9-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="0e7a9-108">Member</span></span>|<span data-ttu-id="0e7a9-109">値</span><span class="sxs-lookup"><span data-stu-id="0e7a9-109">Value</span></span>|<span data-ttu-id="0e7a9-110">説明</span><span class="sxs-lookup"><span data-stu-id="0e7a9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e7a9-111">使用可能</span><span class="sxs-lookup"><span data-stu-id="0e7a9-111">available</span></span>|<span data-ttu-id="0e7a9-112">.0</span><span class="sxs-lookup"><span data-stu-id="0e7a9-112">0</span></span>|<span data-ttu-id="0e7a9-113">Available</span><span class="sxs-lookup"><span data-stu-id="0e7a9-113">Available</span></span>|
|<span data-ttu-id="0e7a9-114">notAvailable</span><span class="sxs-lookup"><span data-stu-id="0e7a9-114">notAvailable</span></span>|<span data-ttu-id="0e7a9-115">1-d</span><span class="sxs-lookup"><span data-stu-id="0e7a9-115">1</span></span>|<span data-ttu-id="0e7a9-116">インストールしない</span><span class="sxs-lookup"><span data-stu-id="0e7a9-116">Not Available</span></span>|
|<span data-ttu-id="0e7a9-117">requiredInstall</span><span class="sxs-lookup"><span data-stu-id="0e7a9-117">requiredInstall</span></span>|<span data-ttu-id="0e7a9-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="0e7a9-118">2</span></span>|<span data-ttu-id="0e7a9-119">必要なインストール</span><span class="sxs-lookup"><span data-stu-id="0e7a9-119">Required Install</span></span>|
|<span data-ttu-id="0e7a9-120">requiredUninstall</span><span class="sxs-lookup"><span data-stu-id="0e7a9-120">requiredUninstall</span></span>|<span data-ttu-id="0e7a9-121">1/3</span><span class="sxs-lookup"><span data-stu-id="0e7a9-121">3</span></span>|<span data-ttu-id="0e7a9-122">必要なアンインストール</span><span class="sxs-lookup"><span data-stu-id="0e7a9-122">Required Uninstall</span></span>|
|<span data-ttu-id="0e7a9-123">Requiredandのインストール</span><span class="sxs-lookup"><span data-stu-id="0e7a9-123">requiredAndAvailableInstall</span></span>|<span data-ttu-id="0e7a9-124">2/4</span><span class="sxs-lookup"><span data-stu-id="0e7a9-124">4</span></span>|<span data-ttu-id="0e7a9-125">Requiredandのインストール</span><span class="sxs-lookup"><span data-stu-id="0e7a9-125">RequiredAndAvailableInstall</span></span>|
|<span data-ttu-id="0e7a9-126">登録がありません。</span><span class="sxs-lookup"><span data-stu-id="0e7a9-126">availableInstallWithoutEnrollment</span></span>|<span data-ttu-id="0e7a9-127">5</span><span class="sxs-lookup"><span data-stu-id="0e7a9-127">5</span></span>|<span data-ttu-id="0e7a9-128">登録がありません。</span><span class="sxs-lookup"><span data-stu-id="0e7a9-128">AvailableInstallWithoutEnrollment</span></span>|
|<span data-ttu-id="0e7a9-129">削除</span><span class="sxs-lookup"><span data-stu-id="0e7a9-129">exclude</span></span>|<span data-ttu-id="0e7a9-130">シックス</span><span class="sxs-lookup"><span data-stu-id="0e7a9-130">6</span></span>|<span data-ttu-id="0e7a9-131">除外</span><span class="sxs-lookup"><span data-stu-id="0e7a9-131">Exclude</span></span>|





