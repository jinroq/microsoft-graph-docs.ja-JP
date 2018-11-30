---
title: windowsUpdateType 列挙型
description: 分岐デバイスから更新を受け取ります。
ms.openlocfilehash: 7669caa27be93786d381266f88b41ae456314bb4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074251"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="6bff3-103">windowsUpdateType 列挙型</span><span class="sxs-lookup"><span data-stu-id="6bff3-103">windowsUpdateType enum type</span></span>

> <span data-ttu-id="6bff3-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6bff3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6bff3-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6bff3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6bff3-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6bff3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6bff3-107">分岐デバイスから更新を受け取ります。</span><span class="sxs-lookup"><span data-stu-id="6bff3-107">Which branch devices will receive their updates from</span></span>
## <a name="members"></a><span data-ttu-id="6bff3-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="6bff3-108">Members</span></span>
|<span data-ttu-id="6bff3-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="6bff3-109">Member</span></span>|<span data-ttu-id="6bff3-110">値</span><span class="sxs-lookup"><span data-stu-id="6bff3-110">Value</span></span>|<span data-ttu-id="6bff3-111">説明</span><span class="sxs-lookup"><span data-stu-id="6bff3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6bff3-112">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="6bff3-112">userDefined</span></span>|<span data-ttu-id="6bff3-113">0</span><span class="sxs-lookup"><span data-stu-id="6bff3-113">0</span></span>|<span data-ttu-id="6bff3-114">設定するユーザーを許可します。</span><span class="sxs-lookup"><span data-stu-id="6bff3-114">Allow the user to set.</span></span>|
|<span data-ttu-id="6bff3-115">all</span><span class="sxs-lookup"><span data-stu-id="6bff3-115">all</span></span>|<span data-ttu-id="6bff3-116">1</span><span class="sxs-lookup"><span data-stu-id="6bff3-116">1</span></span>|<span data-ttu-id="6bff3-117">半年のチャネル (対象となる)。</span><span class="sxs-lookup"><span data-stu-id="6bff3-117">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="6bff3-118">デバイスでは、半年のチャネル (対象) からすべての適用可能な機能の更新を取得します。</span><span class="sxs-lookup"><span data-stu-id="6bff3-118">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="6bff3-119">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="6bff3-119">businessReadyOnly</span></span>|<span data-ttu-id="6bff3-120">2</span><span class="sxs-lookup"><span data-stu-id="6bff3-120">2</span></span>|<span data-ttu-id="6bff3-121">半年チャンネルです。</span><span class="sxs-lookup"><span data-stu-id="6bff3-121">Semi-annual Channel.</span></span> <span data-ttu-id="6bff3-122">デバイスは、半年のチャネルからの機能の更新を取得します。</span><span class="sxs-lookup"><span data-stu-id="6bff3-122">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="6bff3-123">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="6bff3-123">windowsInsiderBuildFast</span></span>|<span data-ttu-id="6bff3-124">3</span><span class="sxs-lookup"><span data-stu-id="6bff3-124">3</span></span>|<span data-ttu-id="6bff3-125">Windows の内部からのビルド - 高速</span><span class="sxs-lookup"><span data-stu-id="6bff3-125">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="6bff3-126">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="6bff3-126">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="6bff3-127">4</span><span class="sxs-lookup"><span data-stu-id="6bff3-127">4</span></span>|<span data-ttu-id="6bff3-128">Windows 内部からビルド時間がかかる</span><span class="sxs-lookup"><span data-stu-id="6bff3-128">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="6bff3-129">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="6bff3-129">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="6bff3-130">5</span><span class="sxs-lookup"><span data-stu-id="6bff3-130">5</span></span>|<span data-ttu-id="6bff3-131">リリース ビルドの Windows の内部から</span><span class="sxs-lookup"><span data-stu-id="6bff3-131">Release Windows Insider build</span></span>|





