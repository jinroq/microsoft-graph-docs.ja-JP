---
title: windowsUpdateType 列挙型
description: 分岐デバイスから更新を受け取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 90d1f946dd497e650df5eb07004560dda028e14f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27930342"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="a974b-103">windowsUpdateType 列挙型</span><span class="sxs-lookup"><span data-stu-id="a974b-103">windowsUpdateType enum type</span></span>

> <span data-ttu-id="a974b-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a974b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a974b-105">分岐デバイスから更新を受け取ります。</span><span class="sxs-lookup"><span data-stu-id="a974b-105">Which branch devices will receive their updates from</span></span>
## <a name="members"></a><span data-ttu-id="a974b-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="a974b-106">Members</span></span>
|<span data-ttu-id="a974b-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="a974b-107">Member</span></span>|<span data-ttu-id="a974b-108">値</span><span class="sxs-lookup"><span data-stu-id="a974b-108">Value</span></span>|<span data-ttu-id="a974b-109">説明</span><span class="sxs-lookup"><span data-stu-id="a974b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a974b-110">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="a974b-110">userDefined</span></span>|<span data-ttu-id="a974b-111">0</span><span class="sxs-lookup"><span data-stu-id="a974b-111">0</span></span>|<span data-ttu-id="a974b-112">設定するユーザーを許可します。</span><span class="sxs-lookup"><span data-stu-id="a974b-112">Allow the user to set.</span></span>|
|<span data-ttu-id="a974b-113">all</span><span class="sxs-lookup"><span data-stu-id="a974b-113">all</span></span>|<span data-ttu-id="a974b-114">1</span><span class="sxs-lookup"><span data-stu-id="a974b-114">1</span></span>|<span data-ttu-id="a974b-115">半年のチャネル (対象となる)。</span><span class="sxs-lookup"><span data-stu-id="a974b-115">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="a974b-116">デバイスでは、半年のチャネル (対象) からすべての適用可能な機能の更新を取得します。</span><span class="sxs-lookup"><span data-stu-id="a974b-116">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="a974b-117">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="a974b-117">businessReadyOnly</span></span>|<span data-ttu-id="a974b-118">2</span><span class="sxs-lookup"><span data-stu-id="a974b-118">2</span></span>|<span data-ttu-id="a974b-119">半年チャンネルです。</span><span class="sxs-lookup"><span data-stu-id="a974b-119">Semi-annual Channel.</span></span> <span data-ttu-id="a974b-120">デバイスは、半年のチャネルからの機能の更新を取得します。</span><span class="sxs-lookup"><span data-stu-id="a974b-120">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="a974b-121">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="a974b-121">windowsInsiderBuildFast</span></span>|<span data-ttu-id="a974b-122">3</span><span class="sxs-lookup"><span data-stu-id="a974b-122">3</span></span>|<span data-ttu-id="a974b-123">Windows の内部からのビルド - 高速</span><span class="sxs-lookup"><span data-stu-id="a974b-123">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="a974b-124">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="a974b-124">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="a974b-125">4</span><span class="sxs-lookup"><span data-stu-id="a974b-125">4</span></span>|<span data-ttu-id="a974b-126">Windows 内部からビルド時間がかかる</span><span class="sxs-lookup"><span data-stu-id="a974b-126">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="a974b-127">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="a974b-127">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="a974b-128">5</span><span class="sxs-lookup"><span data-stu-id="a974b-128">5</span></span>|<span data-ttu-id="a974b-129">リリース ビルドの Windows の内部から</span><span class="sxs-lookup"><span data-stu-id="a974b-129">Release Windows Insider build</span></span>|



