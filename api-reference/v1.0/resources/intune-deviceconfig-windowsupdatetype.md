---
title: windowsUpdateType 列挙型
description: 更新プログラムを受信するブランチデバイス
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f91657cabec59cf1307253d707ba632bf4f99463
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32503598"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="937f1-103">windowsUpdateType 列挙型</span><span class="sxs-lookup"><span data-stu-id="937f1-103">windowsUpdateType enum type</span></span>

> <span data-ttu-id="937f1-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="937f1-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="937f1-105">更新プログラムを受信するブランチデバイス</span><span class="sxs-lookup"><span data-stu-id="937f1-105">Which branch devices will receive their updates from</span></span>

## <a name="members"></a><span data-ttu-id="937f1-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="937f1-106">Members</span></span>
|<span data-ttu-id="937f1-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="937f1-107">Member</span></span>|<span data-ttu-id="937f1-108">値</span><span class="sxs-lookup"><span data-stu-id="937f1-108">Value</span></span>|<span data-ttu-id="937f1-109">説明</span><span class="sxs-lookup"><span data-stu-id="937f1-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="937f1-110">自分のもの</span><span class="sxs-lookup"><span data-stu-id="937f1-110">userDefined</span></span>|<span data-ttu-id="937f1-111">.0</span><span class="sxs-lookup"><span data-stu-id="937f1-111">0</span></span>|<span data-ttu-id="937f1-112">ユーザーがを設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="937f1-112">Allow the user to set.</span></span>|
|<span data-ttu-id="937f1-113">すべての</span><span class="sxs-lookup"><span data-stu-id="937f1-113">all</span></span>|<span data-ttu-id="937f1-114">1 </span><span class="sxs-lookup"><span data-stu-id="937f1-114">1</span></span>|<span data-ttu-id="937f1-115">半期チャネル (対象指定)。</span><span class="sxs-lookup"><span data-stu-id="937f1-115">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="937f1-116">デバイスは、半期チャネル (対象指定) から、適用可能なすべての機能の更新を取得します。</span><span class="sxs-lookup"><span data-stu-id="937f1-116">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="937f1-117">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="937f1-117">businessReadyOnly</span></span>|<span data-ttu-id="937f1-118">2 </span><span class="sxs-lookup"><span data-stu-id="937f1-118">2</span></span>|<span data-ttu-id="937f1-119">半期チャネル</span><span class="sxs-lookup"><span data-stu-id="937f1-119">Semi-annual Channel.</span></span> <span data-ttu-id="937f1-120">デバイスは、半期チャネルから機能の更新を取得します。</span><span class="sxs-lookup"><span data-stu-id="937f1-120">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="937f1-121">windowsinsiderbuildfast</span><span class="sxs-lookup"><span data-stu-id="937f1-121">windowsInsiderBuildFast</span></span>|<span data-ttu-id="937f1-122">3 </span><span class="sxs-lookup"><span data-stu-id="937f1-122">3</span></span>|<span data-ttu-id="937f1-123">Windows Insider ビルド-Fast</span><span class="sxs-lookup"><span data-stu-id="937f1-123">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="937f1-124">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="937f1-124">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="937f1-125">4 </span><span class="sxs-lookup"><span data-stu-id="937f1-125">4</span></span>|<span data-ttu-id="937f1-126">Windows Insider ビルド-低速</span><span class="sxs-lookup"><span data-stu-id="937f1-126">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="937f1-127">windowsinsiderbuildrelease</span><span class="sxs-lookup"><span data-stu-id="937f1-127">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="937f1-128">5 </span><span class="sxs-lookup"><span data-stu-id="937f1-128">5</span></span>|<span data-ttu-id="937f1-129">Windows Insider ビルドをリリースする</span><span class="sxs-lookup"><span data-stu-id="937f1-129">Release Windows Insider build</span></span>|



