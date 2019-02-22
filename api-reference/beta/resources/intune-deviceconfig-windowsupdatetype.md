---
title: windowsUpdateType 列挙型
description: 更新プログラムを受信するブランチデバイス
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 17aad82b25982b90ecea348d959e2ed2ec94a483
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30169161"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="5c6b9-103">windowsUpdateType 列挙型</span><span class="sxs-lookup"><span data-stu-id="5c6b9-103">windowsUpdateType enum type</span></span>

> <span data-ttu-id="5c6b9-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5c6b9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5c6b9-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="5c6b9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c6b9-106">更新プログラムを受信するブランチデバイス</span><span class="sxs-lookup"><span data-stu-id="5c6b9-106">Which branch devices will receive their updates from</span></span>

## <a name="members"></a><span data-ttu-id="5c6b9-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="5c6b9-107">Members</span></span>
|<span data-ttu-id="5c6b9-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="5c6b9-108">Member</span></span>|<span data-ttu-id="5c6b9-109">値</span><span class="sxs-lookup"><span data-stu-id="5c6b9-109">Value</span></span>|<span data-ttu-id="5c6b9-110">説明</span><span class="sxs-lookup"><span data-stu-id="5c6b9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c6b9-111">自分のもの</span><span class="sxs-lookup"><span data-stu-id="5c6b9-111">userDefined</span></span>|<span data-ttu-id="5c6b9-112">.0</span><span class="sxs-lookup"><span data-stu-id="5c6b9-112">0</span></span>|<span data-ttu-id="5c6b9-113">ユーザーがを設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="5c6b9-113">Allow the user to set.</span></span>|
|<span data-ttu-id="5c6b9-114">all</span><span class="sxs-lookup"><span data-stu-id="5c6b9-114">all</span></span>|<span data-ttu-id="5c6b9-115">1-d</span><span class="sxs-lookup"><span data-stu-id="5c6b9-115">1</span></span>|<span data-ttu-id="5c6b9-116">半期チャネル (対象指定)。</span><span class="sxs-lookup"><span data-stu-id="5c6b9-116">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="5c6b9-117">デバイスは、半期チャネル (対象指定) から、適用可能なすべての機能の更新を取得します。</span><span class="sxs-lookup"><span data-stu-id="5c6b9-117">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="5c6b9-118">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="5c6b9-118">businessReadyOnly</span></span>|<span data-ttu-id="5c6b9-119">pbm-2</span><span class="sxs-lookup"><span data-stu-id="5c6b9-119">2</span></span>|<span data-ttu-id="5c6b9-120">半期チャネル</span><span class="sxs-lookup"><span data-stu-id="5c6b9-120">Semi-annual Channel.</span></span> <span data-ttu-id="5c6b9-121">デバイスは、半期チャネルから機能の更新を取得します。</span><span class="sxs-lookup"><span data-stu-id="5c6b9-121">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="5c6b9-122">windowsinsiderbuildfast</span><span class="sxs-lookup"><span data-stu-id="5c6b9-122">windowsInsiderBuildFast</span></span>|<span data-ttu-id="5c6b9-123">1/3</span><span class="sxs-lookup"><span data-stu-id="5c6b9-123">3</span></span>|<span data-ttu-id="5c6b9-124">Windows Insider ビルド-Fast</span><span class="sxs-lookup"><span data-stu-id="5c6b9-124">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="5c6b9-125">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="5c6b9-125">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="5c6b9-126">2/4</span><span class="sxs-lookup"><span data-stu-id="5c6b9-126">4</span></span>|<span data-ttu-id="5c6b9-127">Windows Insider ビルド-低速</span><span class="sxs-lookup"><span data-stu-id="5c6b9-127">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="5c6b9-128">windowsinsiderbuildrelease</span><span class="sxs-lookup"><span data-stu-id="5c6b9-128">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="5c6b9-129">5</span><span class="sxs-lookup"><span data-stu-id="5c6b9-129">5</span></span>|<span data-ttu-id="5c6b9-130">Windows Insider ビルドをリリースする</span><span class="sxs-lookup"><span data-stu-id="5c6b9-130">Release Windows Insider build</span></span>|




