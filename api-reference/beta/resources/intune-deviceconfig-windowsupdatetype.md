---
title: windowsUpdateType 列挙型
description: 更新プログラムを受信するブランチデバイス
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5869bcfaa3949a8463d2625c4e7de48897a62daf
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943607"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="963d4-103">windowsUpdateType 列挙型</span><span class="sxs-lookup"><span data-stu-id="963d4-103">windowsUpdateType enum type</span></span>

> <span data-ttu-id="963d4-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="963d4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="963d4-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="963d4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="963d4-106">更新プログラムを受信するブランチデバイス</span><span class="sxs-lookup"><span data-stu-id="963d4-106">Which branch devices will receive their updates from</span></span>

## <a name="members"></a><span data-ttu-id="963d4-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="963d4-107">Members</span></span>
|<span data-ttu-id="963d4-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="963d4-108">Member</span></span>|<span data-ttu-id="963d4-109">値</span><span class="sxs-lookup"><span data-stu-id="963d4-109">Value</span></span>|<span data-ttu-id="963d4-110">説明</span><span class="sxs-lookup"><span data-stu-id="963d4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="963d4-111">自分のもの</span><span class="sxs-lookup"><span data-stu-id="963d4-111">userDefined</span></span>|<span data-ttu-id="963d4-112">.0</span><span class="sxs-lookup"><span data-stu-id="963d4-112">0</span></span>|<span data-ttu-id="963d4-113">ユーザーがを設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="963d4-113">Allow the user to set.</span></span>|
|<span data-ttu-id="963d4-114">すべての</span><span class="sxs-lookup"><span data-stu-id="963d4-114">all</span></span>|<span data-ttu-id="963d4-115">1-d</span><span class="sxs-lookup"><span data-stu-id="963d4-115">1</span></span>|<span data-ttu-id="963d4-116">半期チャネル (対象指定)。</span><span class="sxs-lookup"><span data-stu-id="963d4-116">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="963d4-117">デバイスは、半期チャネル (対象指定) から、適用可能なすべての機能の更新を取得します。</span><span class="sxs-lookup"><span data-stu-id="963d4-117">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="963d4-118">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="963d4-118">businessReadyOnly</span></span>|<span data-ttu-id="963d4-119">pbm-2</span><span class="sxs-lookup"><span data-stu-id="963d4-119">2</span></span>|<span data-ttu-id="963d4-120">半期チャネル</span><span class="sxs-lookup"><span data-stu-id="963d4-120">Semi-annual Channel.</span></span> <span data-ttu-id="963d4-121">デバイスは、半期チャネルから機能の更新を取得します。</span><span class="sxs-lookup"><span data-stu-id="963d4-121">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="963d4-122">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="963d4-122">windowsInsiderBuildFast</span></span>|<span data-ttu-id="963d4-123">1/3</span><span class="sxs-lookup"><span data-stu-id="963d4-123">3</span></span>|<span data-ttu-id="963d4-124">Windows Insider ビルド-Fast</span><span class="sxs-lookup"><span data-stu-id="963d4-124">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="963d4-125">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="963d4-125">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="963d4-126">2/4</span><span class="sxs-lookup"><span data-stu-id="963d4-126">4</span></span>|<span data-ttu-id="963d4-127">Windows Insider ビルド-低速</span><span class="sxs-lookup"><span data-stu-id="963d4-127">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="963d4-128">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="963d4-128">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="963d4-129">5</span><span class="sxs-lookup"><span data-stu-id="963d4-129">5</span></span>|<span data-ttu-id="963d4-130">Windows Insider ビルドをリリースする</span><span class="sxs-lookup"><span data-stu-id="963d4-130">Release Windows Insider build</span></span>|




