---
title: mobileAppIntent 列挙型
description: デバイス上のモバイルアプリの状態を示します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 135800266a2737c6c6dc3931b2a78990c059ef2c
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33939687"
---
# <a name="mobileappintent-enum-type"></a><span data-ttu-id="ce01f-103">mobileAppIntent 列挙型</span><span class="sxs-lookup"><span data-stu-id="ce01f-103">mobileAppIntent enum type</span></span>

> <span data-ttu-id="ce01f-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ce01f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ce01f-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ce01f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce01f-106">デバイス上のモバイルアプリの状態を示します。</span><span class="sxs-lookup"><span data-stu-id="ce01f-106">Indicates the status of the mobile app on the device.</span></span>

## <a name="members"></a><span data-ttu-id="ce01f-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="ce01f-107">Members</span></span>
|<span data-ttu-id="ce01f-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="ce01f-108">Member</span></span>|<span data-ttu-id="ce01f-109">値</span><span class="sxs-lookup"><span data-stu-id="ce01f-109">Value</span></span>|<span data-ttu-id="ce01f-110">説明</span><span class="sxs-lookup"><span data-stu-id="ce01f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce01f-111">使用可能</span><span class="sxs-lookup"><span data-stu-id="ce01f-111">available</span></span>|<span data-ttu-id="ce01f-112">.0</span><span class="sxs-lookup"><span data-stu-id="ce01f-112">0</span></span>|<span data-ttu-id="ce01f-113">Available</span><span class="sxs-lookup"><span data-stu-id="ce01f-113">Available</span></span>|
|<span data-ttu-id="ce01f-114">notAvailable</span><span class="sxs-lookup"><span data-stu-id="ce01f-114">notAvailable</span></span>|<span data-ttu-id="ce01f-115">1-d</span><span class="sxs-lookup"><span data-stu-id="ce01f-115">1</span></span>|<span data-ttu-id="ce01f-116">インストールしない</span><span class="sxs-lookup"><span data-stu-id="ce01f-116">Not Available</span></span>|
|<span data-ttu-id="ce01f-117">requiredInstall</span><span class="sxs-lookup"><span data-stu-id="ce01f-117">requiredInstall</span></span>|<span data-ttu-id="ce01f-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="ce01f-118">2</span></span>|<span data-ttu-id="ce01f-119">必要なインストール</span><span class="sxs-lookup"><span data-stu-id="ce01f-119">Required Install</span></span>|
|<span data-ttu-id="ce01f-120">requiredUninstall</span><span class="sxs-lookup"><span data-stu-id="ce01f-120">requiredUninstall</span></span>|<span data-ttu-id="ce01f-121">1/3</span><span class="sxs-lookup"><span data-stu-id="ce01f-121">3</span></span>|<span data-ttu-id="ce01f-122">必要なアンインストール</span><span class="sxs-lookup"><span data-stu-id="ce01f-122">Required Uninstall</span></span>|
|<span data-ttu-id="ce01f-123">Requiredandのインストール</span><span class="sxs-lookup"><span data-stu-id="ce01f-123">requiredAndAvailableInstall</span></span>|<span data-ttu-id="ce01f-124">2/4</span><span class="sxs-lookup"><span data-stu-id="ce01f-124">4</span></span>|<span data-ttu-id="ce01f-125">Requiredandのインストール</span><span class="sxs-lookup"><span data-stu-id="ce01f-125">RequiredAndAvailableInstall</span></span>|
|<span data-ttu-id="ce01f-126">登録がありません。</span><span class="sxs-lookup"><span data-stu-id="ce01f-126">availableInstallWithoutEnrollment</span></span>|<span data-ttu-id="ce01f-127">5</span><span class="sxs-lookup"><span data-stu-id="ce01f-127">5</span></span>|<span data-ttu-id="ce01f-128">登録がありません。</span><span class="sxs-lookup"><span data-stu-id="ce01f-128">AvailableInstallWithoutEnrollment</span></span>|
|<span data-ttu-id="ce01f-129">削除</span><span class="sxs-lookup"><span data-stu-id="ce01f-129">exclude</span></span>|<span data-ttu-id="ce01f-130">シックス</span><span class="sxs-lookup"><span data-stu-id="ce01f-130">6</span></span>|<span data-ttu-id="ce01f-131">除外</span><span class="sxs-lookup"><span data-stu-id="ce01f-131">Exclude</span></span>|




