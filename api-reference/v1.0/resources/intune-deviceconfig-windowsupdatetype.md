---
title: windowsUpdateType 列挙型
description: 更新プログラムを受信するブランチデバイス
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: d7630e3cac3702380da07c2a92857d9f2786810a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36027574"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="3afb6-103">windowsUpdateType 列挙型</span><span class="sxs-lookup"><span data-stu-id="3afb6-103">windowsUpdateType enum type</span></span>

> <span data-ttu-id="3afb6-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3afb6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3afb6-105">更新プログラムを受信するブランチデバイス</span><span class="sxs-lookup"><span data-stu-id="3afb6-105">Which branch devices will receive their updates from</span></span>

## <a name="members"></a><span data-ttu-id="3afb6-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="3afb6-106">Members</span></span>
|<span data-ttu-id="3afb6-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="3afb6-107">Member</span></span>|<span data-ttu-id="3afb6-108">値</span><span class="sxs-lookup"><span data-stu-id="3afb6-108">Value</span></span>|<span data-ttu-id="3afb6-109">説明</span><span class="sxs-lookup"><span data-stu-id="3afb6-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3afb6-110">自分のもの</span><span class="sxs-lookup"><span data-stu-id="3afb6-110">userDefined</span></span>|<span data-ttu-id="3afb6-111">.0</span><span class="sxs-lookup"><span data-stu-id="3afb6-111">0</span></span>|<span data-ttu-id="3afb6-112">ユーザーがを設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="3afb6-112">Allow the user to set.</span></span>|
|<span data-ttu-id="3afb6-113">すべての</span><span class="sxs-lookup"><span data-stu-id="3afb6-113">all</span></span>|<span data-ttu-id="3afb6-114">1-d</span><span class="sxs-lookup"><span data-stu-id="3afb6-114">1</span></span>|<span data-ttu-id="3afb6-115">半期チャネル (対象指定)。</span><span class="sxs-lookup"><span data-stu-id="3afb6-115">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="3afb6-116">デバイスは、半期チャネル (対象指定) から、適用可能なすべての機能の更新を取得します。</span><span class="sxs-lookup"><span data-stu-id="3afb6-116">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="3afb6-117">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="3afb6-117">businessReadyOnly</span></span>|<span data-ttu-id="3afb6-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="3afb6-118">2</span></span>|<span data-ttu-id="3afb6-119">半期チャネル</span><span class="sxs-lookup"><span data-stu-id="3afb6-119">Semi-annual Channel.</span></span> <span data-ttu-id="3afb6-120">デバイスは、半期チャネルから機能の更新を取得します。</span><span class="sxs-lookup"><span data-stu-id="3afb6-120">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="3afb6-121">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="3afb6-121">windowsInsiderBuildFast</span></span>|<span data-ttu-id="3afb6-122">1/3</span><span class="sxs-lookup"><span data-stu-id="3afb6-122">3</span></span>|<span data-ttu-id="3afb6-123">Windows Insider ビルド-Fast</span><span class="sxs-lookup"><span data-stu-id="3afb6-123">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="3afb6-124">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="3afb6-124">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="3afb6-125">2/4</span><span class="sxs-lookup"><span data-stu-id="3afb6-125">4</span></span>|<span data-ttu-id="3afb6-126">Windows Insider ビルド-低速</span><span class="sxs-lookup"><span data-stu-id="3afb6-126">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="3afb6-127">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="3afb6-127">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="3afb6-128">5</span><span class="sxs-lookup"><span data-stu-id="3afb6-128">5</span></span>|<span data-ttu-id="3afb6-129">Windows Insider ビルドをリリースする</span><span class="sxs-lookup"><span data-stu-id="3afb6-129">Release Windows Insider build</span></span>|



