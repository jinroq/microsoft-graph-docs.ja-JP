---
title: windowsUpdateType 列挙型
description: 分岐デバイスから更新を受け取ります。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 15d2d46684d38b57690cc9c12d9c49eccd652e6f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27887039"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="50d5e-103">windowsUpdateType 列挙型</span><span class="sxs-lookup"><span data-stu-id="50d5e-103">windowsUpdateType enum type</span></span>

> <span data-ttu-id="50d5e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="50d5e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="50d5e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="50d5e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="50d5e-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="50d5e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="50d5e-107">分岐デバイスから更新を受け取ります。</span><span class="sxs-lookup"><span data-stu-id="50d5e-107">Which branch devices will receive their updates from</span></span>
## <a name="members"></a><span data-ttu-id="50d5e-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="50d5e-108">Members</span></span>
|<span data-ttu-id="50d5e-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="50d5e-109">Member</span></span>|<span data-ttu-id="50d5e-110">値</span><span class="sxs-lookup"><span data-stu-id="50d5e-110">Value</span></span>|<span data-ttu-id="50d5e-111">説明</span><span class="sxs-lookup"><span data-stu-id="50d5e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50d5e-112">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="50d5e-112">userDefined</span></span>|<span data-ttu-id="50d5e-113">0</span><span class="sxs-lookup"><span data-stu-id="50d5e-113">0</span></span>|<span data-ttu-id="50d5e-114">設定するユーザーを許可します。</span><span class="sxs-lookup"><span data-stu-id="50d5e-114">Allow the user to set.</span></span>|
|<span data-ttu-id="50d5e-115">all</span><span class="sxs-lookup"><span data-stu-id="50d5e-115">all</span></span>|<span data-ttu-id="50d5e-116">1</span><span class="sxs-lookup"><span data-stu-id="50d5e-116">1</span></span>|<span data-ttu-id="50d5e-117">半年のチャネル (対象となる)。</span><span class="sxs-lookup"><span data-stu-id="50d5e-117">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="50d5e-118">デバイスでは、半年のチャネル (対象) からすべての適用可能な機能の更新を取得します。</span><span class="sxs-lookup"><span data-stu-id="50d5e-118">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="50d5e-119">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="50d5e-119">businessReadyOnly</span></span>|<span data-ttu-id="50d5e-120">2</span><span class="sxs-lookup"><span data-stu-id="50d5e-120">2</span></span>|<span data-ttu-id="50d5e-121">半年チャンネルです。</span><span class="sxs-lookup"><span data-stu-id="50d5e-121">Semi-annual Channel.</span></span> <span data-ttu-id="50d5e-122">デバイスは、半年のチャネルからの機能の更新を取得します。</span><span class="sxs-lookup"><span data-stu-id="50d5e-122">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="50d5e-123">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="50d5e-123">windowsInsiderBuildFast</span></span>|<span data-ttu-id="50d5e-124">3</span><span class="sxs-lookup"><span data-stu-id="50d5e-124">3</span></span>|<span data-ttu-id="50d5e-125">Windows の内部からのビルド - 高速</span><span class="sxs-lookup"><span data-stu-id="50d5e-125">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="50d5e-126">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="50d5e-126">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="50d5e-127">4</span><span class="sxs-lookup"><span data-stu-id="50d5e-127">4</span></span>|<span data-ttu-id="50d5e-128">Windows 内部からビルド時間がかかる</span><span class="sxs-lookup"><span data-stu-id="50d5e-128">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="50d5e-129">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="50d5e-129">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="50d5e-130">5</span><span class="sxs-lookup"><span data-stu-id="50d5e-130">5</span></span>|<span data-ttu-id="50d5e-131">リリース ビルドの Windows の内部から</span><span class="sxs-lookup"><span data-stu-id="50d5e-131">Release Windows Insider build</span></span>|





