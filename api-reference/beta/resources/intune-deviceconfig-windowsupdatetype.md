---
title: windowsUpdateType 列挙型
description: 更新プログラムを受信するブランチデバイス
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 228cc5ba4b50681bfe78a15ef214d6f3ab2ebb17
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523596"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="92e75-103">windowsUpdateType 列挙型</span><span class="sxs-lookup"><span data-stu-id="92e75-103">windowsUpdateType enum type</span></span>

> <span data-ttu-id="92e75-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="92e75-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92e75-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="92e75-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92e75-106">更新プログラムを受信するブランチデバイス</span><span class="sxs-lookup"><span data-stu-id="92e75-106">Which branch devices will receive their updates from</span></span>

## <a name="members"></a><span data-ttu-id="92e75-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="92e75-107">Members</span></span>
|<span data-ttu-id="92e75-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="92e75-108">Member</span></span>|<span data-ttu-id="92e75-109">値</span><span class="sxs-lookup"><span data-stu-id="92e75-109">Value</span></span>|<span data-ttu-id="92e75-110">説明</span><span class="sxs-lookup"><span data-stu-id="92e75-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92e75-111">自分のもの</span><span class="sxs-lookup"><span data-stu-id="92e75-111">userDefined</span></span>|<span data-ttu-id="92e75-112">.0</span><span class="sxs-lookup"><span data-stu-id="92e75-112">0</span></span>|<span data-ttu-id="92e75-113">ユーザーがを設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="92e75-113">Allow the user to set.</span></span>|
|<span data-ttu-id="92e75-114">すべての</span><span class="sxs-lookup"><span data-stu-id="92e75-114">all</span></span>|<span data-ttu-id="92e75-115">1 </span><span class="sxs-lookup"><span data-stu-id="92e75-115">1</span></span>|<span data-ttu-id="92e75-116">半期チャネル (対象指定)。</span><span class="sxs-lookup"><span data-stu-id="92e75-116">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="92e75-117">デバイスは、半期チャネル (対象指定) から、適用可能なすべての機能の更新を取得します。</span><span class="sxs-lookup"><span data-stu-id="92e75-117">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="92e75-118">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="92e75-118">businessReadyOnly</span></span>|<span data-ttu-id="92e75-119">2 </span><span class="sxs-lookup"><span data-stu-id="92e75-119">2</span></span>|<span data-ttu-id="92e75-120">半期チャネル</span><span class="sxs-lookup"><span data-stu-id="92e75-120">Semi-annual Channel.</span></span> <span data-ttu-id="92e75-121">デバイスは、半期チャネルから機能の更新を取得します。</span><span class="sxs-lookup"><span data-stu-id="92e75-121">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="92e75-122">windowsinsiderbuildfast</span><span class="sxs-lookup"><span data-stu-id="92e75-122">windowsInsiderBuildFast</span></span>|<span data-ttu-id="92e75-123">3 </span><span class="sxs-lookup"><span data-stu-id="92e75-123">3</span></span>|<span data-ttu-id="92e75-124">Windows Insider ビルド-Fast</span><span class="sxs-lookup"><span data-stu-id="92e75-124">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="92e75-125">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="92e75-125">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="92e75-126">4 </span><span class="sxs-lookup"><span data-stu-id="92e75-126">4</span></span>|<span data-ttu-id="92e75-127">Windows Insider ビルド-低速</span><span class="sxs-lookup"><span data-stu-id="92e75-127">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="92e75-128">windowsinsiderbuildrelease</span><span class="sxs-lookup"><span data-stu-id="92e75-128">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="92e75-129">5 </span><span class="sxs-lookup"><span data-stu-id="92e75-129">5</span></span>|<span data-ttu-id="92e75-130">Windows Insider ビルドをリリースする</span><span class="sxs-lookup"><span data-stu-id="92e75-130">Release Windows Insider build</span></span>|





