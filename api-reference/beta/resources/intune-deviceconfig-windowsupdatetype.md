---
title: windowsUpdateType 列挙型
description: 更新プログラムを受信するブランチデバイス
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 2eb02ddde8b570a6d68f077ead1123b00e82cfe0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36000124"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="ea2a3-103">windowsUpdateType 列挙型</span><span class="sxs-lookup"><span data-stu-id="ea2a3-103">windowsUpdateType enum type</span></span>

> <span data-ttu-id="ea2a3-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ea2a3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ea2a3-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ea2a3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea2a3-106">更新プログラムを受信するブランチデバイス</span><span class="sxs-lookup"><span data-stu-id="ea2a3-106">Which branch devices will receive their updates from</span></span>

## <a name="members"></a><span data-ttu-id="ea2a3-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="ea2a3-107">Members</span></span>
|<span data-ttu-id="ea2a3-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="ea2a3-108">Member</span></span>|<span data-ttu-id="ea2a3-109">値</span><span class="sxs-lookup"><span data-stu-id="ea2a3-109">Value</span></span>|<span data-ttu-id="ea2a3-110">説明</span><span class="sxs-lookup"><span data-stu-id="ea2a3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea2a3-111">自分のもの</span><span class="sxs-lookup"><span data-stu-id="ea2a3-111">userDefined</span></span>|<span data-ttu-id="ea2a3-112">.0</span><span class="sxs-lookup"><span data-stu-id="ea2a3-112">0</span></span>|<span data-ttu-id="ea2a3-113">ユーザーがを設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="ea2a3-113">Allow the user to set.</span></span>|
|<span data-ttu-id="ea2a3-114">すべての</span><span class="sxs-lookup"><span data-stu-id="ea2a3-114">all</span></span>|<span data-ttu-id="ea2a3-115">1-d</span><span class="sxs-lookup"><span data-stu-id="ea2a3-115">1</span></span>|<span data-ttu-id="ea2a3-116">半期チャネル (対象指定)。</span><span class="sxs-lookup"><span data-stu-id="ea2a3-116">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="ea2a3-117">デバイスは、半期チャネル (対象指定) から、適用可能なすべての機能の更新を取得します。</span><span class="sxs-lookup"><span data-stu-id="ea2a3-117">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="ea2a3-118">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="ea2a3-118">businessReadyOnly</span></span>|<span data-ttu-id="ea2a3-119">pbm-2</span><span class="sxs-lookup"><span data-stu-id="ea2a3-119">2</span></span>|<span data-ttu-id="ea2a3-120">半期チャネル</span><span class="sxs-lookup"><span data-stu-id="ea2a3-120">Semi-annual Channel.</span></span> <span data-ttu-id="ea2a3-121">デバイスは、半期チャネルから機能の更新を取得します。</span><span class="sxs-lookup"><span data-stu-id="ea2a3-121">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="ea2a3-122">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="ea2a3-122">windowsInsiderBuildFast</span></span>|<span data-ttu-id="ea2a3-123">1/3</span><span class="sxs-lookup"><span data-stu-id="ea2a3-123">3</span></span>|<span data-ttu-id="ea2a3-124">Windows Insider ビルド-Fast</span><span class="sxs-lookup"><span data-stu-id="ea2a3-124">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="ea2a3-125">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="ea2a3-125">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="ea2a3-126">2/4</span><span class="sxs-lookup"><span data-stu-id="ea2a3-126">4</span></span>|<span data-ttu-id="ea2a3-127">Windows Insider ビルド-低速</span><span class="sxs-lookup"><span data-stu-id="ea2a3-127">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="ea2a3-128">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="ea2a3-128">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="ea2a3-129">5</span><span class="sxs-lookup"><span data-stu-id="ea2a3-129">5</span></span>|<span data-ttu-id="ea2a3-130">Windows Insider ビルドをリリースする</span><span class="sxs-lookup"><span data-stu-id="ea2a3-130">Release Windows Insider build</span></span>|





