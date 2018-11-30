---
title: windowsUpdateType 列挙型
description: 分岐デバイスから更新を受け取ります。
ms.openlocfilehash: b489f17da5dc02dd7f7e72350eef282e56643dd0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023874"
---
# <a name="windowsupdatetype-enum-type"></a><span data-ttu-id="ee2c9-103">windowsUpdateType 列挙型</span><span class="sxs-lookup"><span data-stu-id="ee2c9-103">windowsUpdateType enum type</span></span>

> <span data-ttu-id="ee2c9-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ee2c9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ee2c9-105">分岐デバイスから更新を受け取ります。</span><span class="sxs-lookup"><span data-stu-id="ee2c9-105">Which branch devices will receive their updates from</span></span>
## <a name="members"></a><span data-ttu-id="ee2c9-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="ee2c9-106">Members</span></span>
|<span data-ttu-id="ee2c9-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="ee2c9-107">Member</span></span>|<span data-ttu-id="ee2c9-108">値</span><span class="sxs-lookup"><span data-stu-id="ee2c9-108">Value</span></span>|<span data-ttu-id="ee2c9-109">説明</span><span class="sxs-lookup"><span data-stu-id="ee2c9-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee2c9-110">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="ee2c9-110">userDefined</span></span>|<span data-ttu-id="ee2c9-111">0</span><span class="sxs-lookup"><span data-stu-id="ee2c9-111">0</span></span>|<span data-ttu-id="ee2c9-112">設定するユーザーを許可します。</span><span class="sxs-lookup"><span data-stu-id="ee2c9-112">Allow the user to set.</span></span>|
|<span data-ttu-id="ee2c9-113">all</span><span class="sxs-lookup"><span data-stu-id="ee2c9-113">all</span></span>|<span data-ttu-id="ee2c9-114">1</span><span class="sxs-lookup"><span data-stu-id="ee2c9-114">1</span></span>|<span data-ttu-id="ee2c9-115">半年のチャネル (対象となる)。</span><span class="sxs-lookup"><span data-stu-id="ee2c9-115">Semi-annual Channel (Targeted).</span></span> <span data-ttu-id="ee2c9-116">デバイスでは、半年のチャネル (対象) からすべての適用可能な機能の更新を取得します。</span><span class="sxs-lookup"><span data-stu-id="ee2c9-116">Device gets all applicable feature updates from Semi-annual Channel (Targeted).</span></span>|
|<span data-ttu-id="ee2c9-117">businessReadyOnly</span><span class="sxs-lookup"><span data-stu-id="ee2c9-117">businessReadyOnly</span></span>|<span data-ttu-id="ee2c9-118">2</span><span class="sxs-lookup"><span data-stu-id="ee2c9-118">2</span></span>|<span data-ttu-id="ee2c9-119">半年チャンネルです。</span><span class="sxs-lookup"><span data-stu-id="ee2c9-119">Semi-annual Channel.</span></span> <span data-ttu-id="ee2c9-120">デバイスは、半年のチャネルからの機能の更新を取得します。</span><span class="sxs-lookup"><span data-stu-id="ee2c9-120">Device gets feature updates from Semi-annual Channel.</span></span>|
|<span data-ttu-id="ee2c9-121">windowsInsiderBuildFast</span><span class="sxs-lookup"><span data-stu-id="ee2c9-121">windowsInsiderBuildFast</span></span>|<span data-ttu-id="ee2c9-122">3</span><span class="sxs-lookup"><span data-stu-id="ee2c9-122">3</span></span>|<span data-ttu-id="ee2c9-123">Windows の内部からのビルド - 高速</span><span class="sxs-lookup"><span data-stu-id="ee2c9-123">Windows Insider build - Fast</span></span>|
|<span data-ttu-id="ee2c9-124">windowsInsiderBuildSlow</span><span class="sxs-lookup"><span data-stu-id="ee2c9-124">windowsInsiderBuildSlow</span></span>|<span data-ttu-id="ee2c9-125">4</span><span class="sxs-lookup"><span data-stu-id="ee2c9-125">4</span></span>|<span data-ttu-id="ee2c9-126">Windows 内部からビルド時間がかかる</span><span class="sxs-lookup"><span data-stu-id="ee2c9-126">Windows Insider build - Slow</span></span>|
|<span data-ttu-id="ee2c9-127">windowsInsiderBuildRelease</span><span class="sxs-lookup"><span data-stu-id="ee2c9-127">windowsInsiderBuildRelease</span></span>|<span data-ttu-id="ee2c9-128">5</span><span class="sxs-lookup"><span data-stu-id="ee2c9-128">5</span></span>|<span data-ttu-id="ee2c9-129">リリース ビルドの Windows の内部から</span><span class="sxs-lookup"><span data-stu-id="ee2c9-129">Release Windows Insider build</span></span>|



