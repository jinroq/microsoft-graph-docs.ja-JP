---
title: mobileAppIntent 列挙型
description: デバイス上のモバイルアプリの状態を示します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 472fd157ed26b8b446e272d37baa135584cbbe0b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32558257"
---
# <a name="mobileappintent-enum-type"></a><span data-ttu-id="4d15d-103">mobileAppIntent 列挙型</span><span class="sxs-lookup"><span data-stu-id="4d15d-103">mobileAppIntent enum type</span></span>

> <span data-ttu-id="4d15d-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4d15d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4d15d-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4d15d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4d15d-106">デバイス上のモバイルアプリの状態を示します。</span><span class="sxs-lookup"><span data-stu-id="4d15d-106">Indicates the status of the mobile app on the device.</span></span>

## <a name="members"></a><span data-ttu-id="4d15d-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="4d15d-107">Members</span></span>
|<span data-ttu-id="4d15d-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="4d15d-108">Member</span></span>|<span data-ttu-id="4d15d-109">値</span><span class="sxs-lookup"><span data-stu-id="4d15d-109">Value</span></span>|<span data-ttu-id="4d15d-110">説明</span><span class="sxs-lookup"><span data-stu-id="4d15d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d15d-111">使用可能</span><span class="sxs-lookup"><span data-stu-id="4d15d-111">available</span></span>|<span data-ttu-id="4d15d-112">.0</span><span class="sxs-lookup"><span data-stu-id="4d15d-112">0</span></span>|<span data-ttu-id="4d15d-113">Available</span><span class="sxs-lookup"><span data-stu-id="4d15d-113">Available</span></span>|
|<span data-ttu-id="4d15d-114">notavailable</span><span class="sxs-lookup"><span data-stu-id="4d15d-114">notAvailable</span></span>|<span data-ttu-id="4d15d-115">1 </span><span class="sxs-lookup"><span data-stu-id="4d15d-115">1</span></span>|<span data-ttu-id="4d15d-116">インストールしない</span><span class="sxs-lookup"><span data-stu-id="4d15d-116">Not Available</span></span>|
|<span data-ttu-id="4d15d-117">requiredinstall</span><span class="sxs-lookup"><span data-stu-id="4d15d-117">requiredInstall</span></span>|<span data-ttu-id="4d15d-118">2 </span><span class="sxs-lookup"><span data-stu-id="4d15d-118">2</span></span>|<span data-ttu-id="4d15d-119">必要なインストール</span><span class="sxs-lookup"><span data-stu-id="4d15d-119">Required Install</span></span>|
|<span data-ttu-id="4d15d-120">requireduninstall</span><span class="sxs-lookup"><span data-stu-id="4d15d-120">requiredUninstall</span></span>|<span data-ttu-id="4d15d-121">3 </span><span class="sxs-lookup"><span data-stu-id="4d15d-121">3</span></span>|<span data-ttu-id="4d15d-122">必要なアンインストール</span><span class="sxs-lookup"><span data-stu-id="4d15d-122">Required Uninstall</span></span>|
|<span data-ttu-id="4d15d-123">requiredandのインストール</span><span class="sxs-lookup"><span data-stu-id="4d15d-123">requiredAndAvailableInstall</span></span>|<span data-ttu-id="4d15d-124">4 </span><span class="sxs-lookup"><span data-stu-id="4d15d-124">4</span></span>|<span data-ttu-id="4d15d-125">requiredandのインストール</span><span class="sxs-lookup"><span data-stu-id="4d15d-125">RequiredAndAvailableInstall</span></span>|
|<span data-ttu-id="4d15d-126">登録がありません。</span><span class="sxs-lookup"><span data-stu-id="4d15d-126">availableInstallWithoutEnrollment</span></span>|<span data-ttu-id="4d15d-127">5 </span><span class="sxs-lookup"><span data-stu-id="4d15d-127">5</span></span>|<span data-ttu-id="4d15d-128">登録がありません。</span><span class="sxs-lookup"><span data-stu-id="4d15d-128">AvailableInstallWithoutEnrollment</span></span>|
|<span data-ttu-id="4d15d-129">削除</span><span class="sxs-lookup"><span data-stu-id="4d15d-129">exclude</span></span>|<span data-ttu-id="4d15d-130">6 </span><span class="sxs-lookup"><span data-stu-id="4d15d-130">6</span></span>|<span data-ttu-id="4d15d-131">除外</span><span class="sxs-lookup"><span data-stu-id="4d15d-131">Exclude</span></span>|



