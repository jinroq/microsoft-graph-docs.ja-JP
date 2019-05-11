---
title: Resultの重要 Appstate 列挙型
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 904d47ebc2efe08a06f1d228b93788b47aea5144
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33939792"
---
# <a name="resultantappstate-enum-type"></a><span data-ttu-id="929e9-103">Resultの重要 Appstate 列挙型</span><span class="sxs-lookup"><span data-stu-id="929e9-103">resultantAppState enum type</span></span>

> <span data-ttu-id="929e9-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="929e9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="929e9-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="929e9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="929e9-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="929e9-106">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="929e9-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="929e9-107">Members</span></span>
|<span data-ttu-id="929e9-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="929e9-108">Member</span></span>|<span data-ttu-id="929e9-109">値</span><span class="sxs-lookup"><span data-stu-id="929e9-109">Value</span></span>|<span data-ttu-id="929e9-110">説明</span><span class="sxs-lookup"><span data-stu-id="929e9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="929e9-111">れる</span><span class="sxs-lookup"><span data-stu-id="929e9-111">installed</span></span>|<span data-ttu-id="929e9-112">1-d</span><span class="sxs-lookup"><span data-stu-id="929e9-112">1</span></span>|<span data-ttu-id="929e9-113">アプリケーションはエラーなしでインストールされます。</span><span class="sxs-lookup"><span data-stu-id="929e9-113">The application is installed with no errors</span></span>|
|<span data-ttu-id="929e9-114">フェール</span><span class="sxs-lookup"><span data-stu-id="929e9-114">failed</span></span>|<span data-ttu-id="929e9-115">pbm-2</span><span class="sxs-lookup"><span data-stu-id="929e9-115">2</span></span>|<span data-ttu-id="929e9-116">アプリケーションをインストールできませんでした。</span><span class="sxs-lookup"><span data-stu-id="929e9-116">The application failed to install.</span></span>|
|<span data-ttu-id="929e9-117">notInstalled</span><span class="sxs-lookup"><span data-stu-id="929e9-117">notInstalled</span></span>|<span data-ttu-id="929e9-118">1/3</span><span class="sxs-lookup"><span data-stu-id="929e9-118">3</span></span>|<span data-ttu-id="929e9-119">アプリケーションがインストールされていません。</span><span class="sxs-lookup"><span data-stu-id="929e9-119">The application is not installed.</span></span>|
|<span data-ttu-id="929e9-120">アンインストールの失敗</span><span class="sxs-lookup"><span data-stu-id="929e9-120">uninstallFailed</span></span>|<span data-ttu-id="929e9-121">2/4</span><span class="sxs-lookup"><span data-stu-id="929e9-121">4</span></span>|<span data-ttu-id="929e9-122">アプリケーションをアンインストールできませんでした。</span><span class="sxs-lookup"><span data-stu-id="929e9-122">The application failed to uninstall.</span></span>|
|<span data-ttu-id="929e9-123">pendingInstall</span><span class="sxs-lookup"><span data-stu-id="929e9-123">pendingInstall</span></span>|<span data-ttu-id="929e9-124">5</span><span class="sxs-lookup"><span data-stu-id="929e9-124">5</span></span>|<span data-ttu-id="929e9-125">アプリケーションのインストールが進行中です。</span><span class="sxs-lookup"><span data-stu-id="929e9-125">The installation of the application is in progress.</span></span>|
|<span data-ttu-id="929e9-126">不明</span><span class="sxs-lookup"><span data-stu-id="929e9-126">unknown</span></span>|<span data-ttu-id="929e9-127">99</span><span class="sxs-lookup"><span data-stu-id="929e9-127">99</span></span>|<span data-ttu-id="929e9-128">アプリケーションの状態が不明です。</span><span class="sxs-lookup"><span data-stu-id="929e9-128">The status of the application is unknown.</span></span>|
|<span data-ttu-id="929e9-129">notApplicable</span><span class="sxs-lookup"><span data-stu-id="929e9-129">notApplicable</span></span>|<span data-ttu-id="929e9-130">-1</span><span class="sxs-lookup"><span data-stu-id="929e9-130">-1</span></span>|<span data-ttu-id="929e9-131">アプリケーションは適用されません。</span><span class="sxs-lookup"><span data-stu-id="929e9-131">The application is not applicable.</span></span>|




