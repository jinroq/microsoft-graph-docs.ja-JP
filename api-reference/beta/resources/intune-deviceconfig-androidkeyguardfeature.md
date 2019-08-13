---
title: Androidkeygu/Feature 列挙型
description: Android keyguard 機能。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 8ae862f244756e675d121ec9eb20d6830e8dd716
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36334459"
---
# <a name="androidkeyguardfeature-enum-type"></a><span data-ttu-id="66eda-103">Androidkeygu/Feature 列挙型</span><span class="sxs-lookup"><span data-stu-id="66eda-103">androidKeyguardFeature enum type</span></span>

> <span data-ttu-id="66eda-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="66eda-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="66eda-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="66eda-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66eda-106">Android keyguard 機能。</span><span class="sxs-lookup"><span data-stu-id="66eda-106">Android keyguard feature.</span></span>

## <a name="members"></a><span data-ttu-id="66eda-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="66eda-107">Members</span></span>
|<span data-ttu-id="66eda-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="66eda-108">Member</span></span>|<span data-ttu-id="66eda-109">値</span><span class="sxs-lookup"><span data-stu-id="66eda-109">Value</span></span>|<span data-ttu-id="66eda-110">説明</span><span class="sxs-lookup"><span data-stu-id="66eda-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66eda-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="66eda-111">notConfigured</span></span>|<span data-ttu-id="66eda-112">.0</span><span class="sxs-lookup"><span data-stu-id="66eda-112">0</span></span>|<span data-ttu-id="66eda-113">未構成。この値は無視されます。</span><span class="sxs-lookup"><span data-stu-id="66eda-113">Not configured; this value is ignored.</span></span>|
|<span data-ttu-id="66eda-114">デジタル</span><span class="sxs-lookup"><span data-stu-id="66eda-114">camera</span></span>|<span data-ttu-id="66eda-115">1-d</span><span class="sxs-lookup"><span data-stu-id="66eda-115">1</span></span>|<span data-ttu-id="66eda-116">セキュリティで保護された keyguard 画面でのカメラの使用状況。</span><span class="sxs-lookup"><span data-stu-id="66eda-116">Camera usage when on secure keyguard screens.</span></span>|
|<span data-ttu-id="66eda-117">受け取る</span><span class="sxs-lookup"><span data-stu-id="66eda-117">notifications</span></span>|<span data-ttu-id="66eda-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="66eda-118">2</span></span>|<span data-ttu-id="66eda-119">セキュリティで保護された keyguard 画面での通知の表示。</span><span class="sxs-lookup"><span data-stu-id="66eda-119">Showing notifications when on secure keyguard screens.</span></span>|
|<span data-ttu-id="66eda-120">未 Redacted通知</span><span class="sxs-lookup"><span data-stu-id="66eda-120">unredactedNotifications</span></span>|<span data-ttu-id="66eda-121">1/3</span><span class="sxs-lookup"><span data-stu-id="66eda-121">3</span></span>|<span data-ttu-id="66eda-122">Secure keyguard 画面での unredacted 通知の表示。</span><span class="sxs-lookup"><span data-stu-id="66eda-122">Showing unredacted notifications when on secure keyguard screens.</span></span>|
|<span data-ttu-id="66eda-123">trustAgents</span><span class="sxs-lookup"><span data-stu-id="66eda-123">trustAgents</span></span>|<span data-ttu-id="66eda-124">2/4</span><span class="sxs-lookup"><span data-stu-id="66eda-124">4</span></span>|<span data-ttu-id="66eda-125">Secure keyguard 画面の場合にエージェントの状態を信頼します。</span><span class="sxs-lookup"><span data-stu-id="66eda-125">Trust agent state when on secure keyguard screens.</span></span>|
|<span data-ttu-id="66eda-126">デジタル</span><span class="sxs-lookup"><span data-stu-id="66eda-126">fingerprint</span></span>|<span data-ttu-id="66eda-127">5</span><span class="sxs-lookup"><span data-stu-id="66eda-127">5</span></span>|<span data-ttu-id="66eda-128">セキュリティで保護された keyguard 画面の場合の指紋センサーの使用量。</span><span class="sxs-lookup"><span data-stu-id="66eda-128">Fingerprint sensor usage when on secure keyguard screens.</span></span>|
|<span data-ttu-id="66eda-129">remoteInput</span><span class="sxs-lookup"><span data-stu-id="66eda-129">remoteInput</span></span>|<span data-ttu-id="66eda-130">シックス</span><span class="sxs-lookup"><span data-stu-id="66eda-130">6</span></span>|<span data-ttu-id="66eda-131">セキュリティで保護された keyguard 画面での通知テキスト入力。</span><span class="sxs-lookup"><span data-stu-id="66eda-131">Notification text entry when on secure keyguard screens.</span></span>|
|<span data-ttu-id="66eda-132">allFeatures</span><span class="sxs-lookup"><span data-stu-id="66eda-132">allFeatures</span></span>|<span data-ttu-id="66eda-133">7</span><span class="sxs-lookup"><span data-stu-id="66eda-133">7</span></span>|<span data-ttu-id="66eda-134">セキュリティで保護された keyguard 画面上のすべての keyguard 機能。</span><span class="sxs-lookup"><span data-stu-id="66eda-134">All keyguard features when on secure keyguard screens.</span></span>|



