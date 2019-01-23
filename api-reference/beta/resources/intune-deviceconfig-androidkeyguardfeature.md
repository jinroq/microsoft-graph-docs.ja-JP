---
title: androidKeyguardFeature 列挙型
description: Android keyguard 機能です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: df89e1e9170bf2e3691116e27125514c7e0a6de9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430342"
---
# <a name="androidkeyguardfeature-enum-type"></a><span data-ttu-id="80941-103">androidKeyguardFeature 列挙型</span><span class="sxs-lookup"><span data-stu-id="80941-103">androidKeyguardFeature enum type</span></span>

> <span data-ttu-id="80941-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="80941-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="80941-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="80941-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="80941-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="80941-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="80941-107">Android keyguard 機能です。</span><span class="sxs-lookup"><span data-stu-id="80941-107">Android keyguard feature.</span></span>

## <a name="members"></a><span data-ttu-id="80941-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="80941-108">Members</span></span>
|<span data-ttu-id="80941-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="80941-109">Member</span></span>|<span data-ttu-id="80941-110">値</span><span class="sxs-lookup"><span data-stu-id="80941-110">Value</span></span>|<span data-ttu-id="80941-111">説明</span><span class="sxs-lookup"><span data-stu-id="80941-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80941-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="80941-112">notConfigured</span></span>|<span data-ttu-id="80941-113">0</span><span class="sxs-lookup"><span data-stu-id="80941-113">0</span></span>|<span data-ttu-id="80941-114">次のように構成されません。この値は無視されます。</span><span class="sxs-lookup"><span data-stu-id="80941-114">Not configured; this value is ignored.</span></span>|
|<span data-ttu-id="80941-115">カメラ</span><span class="sxs-lookup"><span data-stu-id="80941-115">camera</span></span>|<span data-ttu-id="80941-116">1</span><span class="sxs-lookup"><span data-stu-id="80941-116">1</span></span>|<span data-ttu-id="80941-117">セキュリティで保護された keyguard の画面上にあるときのカメラの使用法です。</span><span class="sxs-lookup"><span data-stu-id="80941-117">Camera usage when on secure keyguard screens.</span></span>|
|<span data-ttu-id="80941-118">通知</span><span class="sxs-lookup"><span data-stu-id="80941-118">notifications</span></span>|<span data-ttu-id="80941-119">2</span><span class="sxs-lookup"><span data-stu-id="80941-119">2</span></span>|<span data-ttu-id="80941-120">セキュリティで保護された keyguard の画面上にあるときの通知を表示しています。</span><span class="sxs-lookup"><span data-stu-id="80941-120">Showing notifications when on secure keyguard screens.</span></span>|
|<span data-ttu-id="80941-121">unredactedNotifications</span><span class="sxs-lookup"><span data-stu-id="80941-121">unredactedNotifications</span></span>|<span data-ttu-id="80941-122">3</span><span class="sxs-lookup"><span data-stu-id="80941-122">3</span></span>|<span data-ttu-id="80941-123">表示 unredacted、セキュリティで保護された keyguard の画面上にあるときに通知します。</span><span class="sxs-lookup"><span data-stu-id="80941-123">Showing unredacted notifications when on secure keyguard screens.</span></span>|
|<span data-ttu-id="80941-124">trustAgents</span><span class="sxs-lookup"><span data-stu-id="80941-124">trustAgents</span></span>|<span data-ttu-id="80941-125">4</span><span class="sxs-lookup"><span data-stu-id="80941-125">4</span></span>|<span data-ttu-id="80941-126">セキュリティで保護された keyguard の画面上にあるとき、エージェントの状態を信頼します。</span><span class="sxs-lookup"><span data-stu-id="80941-126">Trust agent state when on secure keyguard screens.</span></span>|
|<span data-ttu-id="80941-127">指紋</span><span class="sxs-lookup"><span data-stu-id="80941-127">fingerprint</span></span>|<span data-ttu-id="80941-128">5</span><span class="sxs-lookup"><span data-stu-id="80941-128">5</span></span>|<span data-ttu-id="80941-129">セキュリティで保護された keyguard の画面上にあるときのセンサーの使用状況を指紋します。</span><span class="sxs-lookup"><span data-stu-id="80941-129">Fingerprint sensor usage when on secure keyguard screens.</span></span>|
|<span data-ttu-id="80941-130">remoteInput</span><span class="sxs-lookup"><span data-stu-id="80941-130">remoteInput</span></span>|<span data-ttu-id="80941-131">6</span><span class="sxs-lookup"><span data-stu-id="80941-131">6</span></span>|<span data-ttu-id="80941-132">セキュリティで保護された keyguard の画面上にあるときの通知テキストを入力します。</span><span class="sxs-lookup"><span data-stu-id="80941-132">Notification text entry when on secure keyguard screens.</span></span>|
|<span data-ttu-id="80941-133">allFeatures</span><span class="sxs-lookup"><span data-stu-id="80941-133">allFeatures</span></span>|<span data-ttu-id="80941-134">7</span><span class="sxs-lookup"><span data-stu-id="80941-134">7</span></span>|<span data-ttu-id="80941-135">セキュリティで保護された keyguard の画面上にあるとき、すべての keyguard 機能。</span><span class="sxs-lookup"><span data-stu-id="80941-135">All keyguard features when on secure keyguard screens.</span></span>|




