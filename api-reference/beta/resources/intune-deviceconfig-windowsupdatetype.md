---
title: windowsUpdateType 列挙型
description: 分岐デバイスから更新を受け取ります。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3d3dd0f6d8ba46d7f1cc803b217a98a862602149
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400138"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="9489a-103">windowsUpdateType 列挙型</span><span class="sxs-lookup"><span data-stu-id="9489a-103">windowsUpdateType enum type</span></span>

> <span data-ttu-id="9489a-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9489a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9489a-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9489a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9489a-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9489a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9489a-107">分岐デバイスから更新を受け取ります。</span><span class="sxs-lookup"><span data-stu-id="9489a-107">Which branch devices will receive their updates from</span></span>

## <a name="members"></a><span data-ttu-id="9489a-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="9489a-108">Members</span></span>
|<span data-ttu-id="9489a-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="9489a-109">Member</span></span>|<span data-ttu-id="9489a-110">値</span><span class="sxs-lookup"><span data-stu-id="9489a-110">Value</span></span>|<span data-ttu-id="9489a-111">説明</span><span class="sxs-lookup"><span data-stu-id="9489a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9489a-112">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="9489a-112">userDefined</span></span>|<span data-ttu-id="9489a-113">0</span><span class="sxs-lookup"><span data-stu-id="9489a-113">0</span></span>|<span data-ttu-id="9489a-114">設定するユーザーを許可します。</span><span class="sxs-lookup"><span data-stu-id="9489a-114">Allow the user to set.</span></span>|
|<span data-ttu-id="9489a-115">all</span><span class="sxs-lookup"><span data-stu-id="9489a-115">all</span></span>|<span data-ttu-id="9489a-116">1</span><span class="sxs-lookup"><span data-stu-id="9489a-116">1</span></span>|<span data-ttu-id="9489a-117">半年のチャネル (対象となる)。</span><span class="sxs-lookup"><span data-stu-id="9489a-117">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="9489a-118">デバイスでは、半年のチャネル (対象) からすべての適用可能な機能の更新を取得します。</span><span class="sxs-lookup"><span data-stu-id="9489a-118">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="9489a-119">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="9489a-119">businessReadyOnly</span></span>|<span data-ttu-id="9489a-120">2</span><span class="sxs-lookup"><span data-stu-id="9489a-120">2</span></span>|<span data-ttu-id="9489a-121">半年チャンネルです。</span><span class="sxs-lookup"><span data-stu-id="9489a-121">Semi-annual Channel.</span></span> <span data-ttu-id="9489a-122">デバイスは、半年のチャネルからの機能の更新を取得します。</span><span class="sxs-lookup"><span data-stu-id="9489a-122">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="9489a-123">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="9489a-123">windowsInsiderBuildFast</span></span>|<span data-ttu-id="9489a-124">3</span><span class="sxs-lookup"><span data-stu-id="9489a-124">3</span></span>|<span data-ttu-id="9489a-125">Windows の内部からのビルド - 高速</span><span class="sxs-lookup"><span data-stu-id="9489a-125">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="9489a-126">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="9489a-126">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="9489a-127">4</span><span class="sxs-lookup"><span data-stu-id="9489a-127">4</span></span>|<span data-ttu-id="9489a-128">Windows 内部からビルド時間がかかる</span><span class="sxs-lookup"><span data-stu-id="9489a-128">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="9489a-129">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="9489a-129">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="9489a-130">5</span><span class="sxs-lookup"><span data-stu-id="9489a-130">5</span></span>|<span data-ttu-id="9489a-131">リリース ビルドの Windows の内部から</span><span class="sxs-lookup"><span data-stu-id="9489a-131">Release Windows Insider build</span></span>|




