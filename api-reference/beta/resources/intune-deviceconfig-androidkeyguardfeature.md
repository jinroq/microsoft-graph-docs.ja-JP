---
title: androidkeygu/feature 列挙型
description: Android keyguard 機能。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b0ff958273d8b39293709b14a960d8bd6b3ea940
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32556236"
---
# <a name="androidkeyguardfeature-enum-type"></a><span data-ttu-id="b825a-103">androidkeygu/feature 列挙型</span><span class="sxs-lookup"><span data-stu-id="b825a-103">androidKeyguardFeature enum type</span></span>

> <span data-ttu-id="b825a-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b825a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b825a-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b825a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b825a-106">Android keyguard 機能。</span><span class="sxs-lookup"><span data-stu-id="b825a-106">Android keyguard feature.</span></span>

## <a name="members"></a><span data-ttu-id="b825a-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="b825a-107">Members</span></span>
|<span data-ttu-id="b825a-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="b825a-108">Member</span></span>|<span data-ttu-id="b825a-109">値</span><span class="sxs-lookup"><span data-stu-id="b825a-109">Value</span></span>|<span data-ttu-id="b825a-110">説明</span><span class="sxs-lookup"><span data-stu-id="b825a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b825a-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="b825a-111">notConfigured</span></span>|<span data-ttu-id="b825a-112">.0</span><span class="sxs-lookup"><span data-stu-id="b825a-112">0</span></span>|<span data-ttu-id="b825a-113">未構成。この値は無視されます。</span><span class="sxs-lookup"><span data-stu-id="b825a-113">Not configured; this value is ignored.</span></span>|
|<span data-ttu-id="b825a-114">デジタル</span><span class="sxs-lookup"><span data-stu-id="b825a-114">camera</span></span>|<span data-ttu-id="b825a-115">1 </span><span class="sxs-lookup"><span data-stu-id="b825a-115">1</span></span>|<span data-ttu-id="b825a-116">セキュリティで保護された keyguard 画面でのカメラの使用状況。</span><span class="sxs-lookup"><span data-stu-id="b825a-116">Camera usage when on secure keyguard screens.</span></span>|
|<span data-ttu-id="b825a-117">受け取る</span><span class="sxs-lookup"><span data-stu-id="b825a-117">notifications</span></span>|<span data-ttu-id="b825a-118">2 </span><span class="sxs-lookup"><span data-stu-id="b825a-118">2</span></span>|<span data-ttu-id="b825a-119">セキュリティで保護された keyguard 画面での通知の表示。</span><span class="sxs-lookup"><span data-stu-id="b825a-119">Showing notifications when on secure keyguard screens.</span></span>|
|<span data-ttu-id="b825a-120">未 redacted通知</span><span class="sxs-lookup"><span data-stu-id="b825a-120">unredactedNotifications</span></span>|<span data-ttu-id="b825a-121">3 </span><span class="sxs-lookup"><span data-stu-id="b825a-121">3</span></span>|<span data-ttu-id="b825a-122">secure keyguard 画面での unredacted 通知の表示。</span><span class="sxs-lookup"><span data-stu-id="b825a-122">Showing unredacted notifications when on secure keyguard screens.</span></span>|
|<span data-ttu-id="b825a-123">trustagents</span><span class="sxs-lookup"><span data-stu-id="b825a-123">trustAgents</span></span>|<span data-ttu-id="b825a-124">4 </span><span class="sxs-lookup"><span data-stu-id="b825a-124">4</span></span>|<span data-ttu-id="b825a-125">secure keyguard 画面の場合にエージェントの状態を信頼します。</span><span class="sxs-lookup"><span data-stu-id="b825a-125">Trust agent state when on secure keyguard screens.</span></span>|
|<span data-ttu-id="b825a-126">デジタル</span><span class="sxs-lookup"><span data-stu-id="b825a-126">fingerprint</span></span>|<span data-ttu-id="b825a-127">5 </span><span class="sxs-lookup"><span data-stu-id="b825a-127">5</span></span>|<span data-ttu-id="b825a-128">セキュリティで保護された keyguard 画面の場合の指紋センサーの使用量。</span><span class="sxs-lookup"><span data-stu-id="b825a-128">Fingerprint sensor usage when on secure keyguard screens.</span></span>|
|<span data-ttu-id="b825a-129">remoteinput</span><span class="sxs-lookup"><span data-stu-id="b825a-129">remoteInput</span></span>|<span data-ttu-id="b825a-130">6 </span><span class="sxs-lookup"><span data-stu-id="b825a-130">6</span></span>|<span data-ttu-id="b825a-131">セキュリティで保護された keyguard 画面での通知テキスト入力。</span><span class="sxs-lookup"><span data-stu-id="b825a-131">Notification text entry when on secure keyguard screens.</span></span>|
|<span data-ttu-id="b825a-132">allfeatures</span><span class="sxs-lookup"><span data-stu-id="b825a-132">allFeatures</span></span>|<span data-ttu-id="b825a-133">7 </span><span class="sxs-lookup"><span data-stu-id="b825a-133">7</span></span>|<span data-ttu-id="b825a-134">セキュリティで保護された keyguard 画面上のすべての keyguard 機能。</span><span class="sxs-lookup"><span data-stu-id="b825a-134">All keyguard features when on secure keyguard screens.</span></span>|





