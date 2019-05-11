---
title: subjectNameFormat 列挙型
description: サブジェクト名の形式オプション。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8b1dd107db00ea871c1055e7a17bec1792076c68
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944664"
---
# <a name="subjectnameformat-enum-type"></a><span data-ttu-id="adc15-103">subjectNameFormat 列挙型</span><span class="sxs-lookup"><span data-stu-id="adc15-103">subjectNameFormat enum type</span></span>

> <span data-ttu-id="adc15-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="adc15-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="adc15-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="adc15-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="adc15-106">サブジェクト名の形式オプション。</span><span class="sxs-lookup"><span data-stu-id="adc15-106">Subject Name Format Options.</span></span>

## <a name="members"></a><span data-ttu-id="adc15-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="adc15-107">Members</span></span>
|<span data-ttu-id="adc15-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="adc15-108">Member</span></span>|<span data-ttu-id="adc15-109">値</span><span class="sxs-lookup"><span data-stu-id="adc15-109">Value</span></span>|<span data-ttu-id="adc15-110">説明</span><span class="sxs-lookup"><span data-stu-id="adc15-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="adc15-111">commonName</span><span class="sxs-lookup"><span data-stu-id="adc15-111">commonName</span></span>|<span data-ttu-id="adc15-112">.0</span><span class="sxs-lookup"><span data-stu-id="adc15-112">0</span></span>|<span data-ttu-id="adc15-113">共通名。</span><span class="sxs-lookup"><span data-stu-id="adc15-113">Common name.</span></span>|
|<span data-ttu-id="adc15-114">Commonnamecommon電子メール</span><span class="sxs-lookup"><span data-stu-id="adc15-114">commonNameIncludingEmail</span></span>|<span data-ttu-id="adc15-115">1-d</span><span class="sxs-lookup"><span data-stu-id="adc15-115">1</span></span>|<span data-ttu-id="adc15-116">電子メールを含む共通名。</span><span class="sxs-lookup"><span data-stu-id="adc15-116">Common Name Including Email.</span></span>|
|<span data-ttu-id="adc15-117">commonNameAsEmail</span><span class="sxs-lookup"><span data-stu-id="adc15-117">commonNameAsEmail</span></span>|<span data-ttu-id="adc15-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="adc15-118">2</span></span>|<span data-ttu-id="adc15-119">電子メールとしての共通名。</span><span class="sxs-lookup"><span data-stu-id="adc15-119">Common Name As Email.</span></span>|
|<span data-ttu-id="adc15-120">配色</span><span class="sxs-lookup"><span data-stu-id="adc15-120">custom</span></span>|<span data-ttu-id="adc15-121">1/3</span><span class="sxs-lookup"><span data-stu-id="adc15-121">3</span></span>|<span data-ttu-id="adc15-122">カスタムサブジェクト名の形式。</span><span class="sxs-lookup"><span data-stu-id="adc15-122">Custom subject name format.</span></span>|
|<span data-ttu-id="adc15-123">commonNameAsIMEI</span><span class="sxs-lookup"><span data-stu-id="adc15-123">commonNameAsIMEI</span></span>|<span data-ttu-id="adc15-124">5</span><span class="sxs-lookup"><span data-stu-id="adc15-124">5</span></span>|<span data-ttu-id="adc15-125">IMEI としての共通名。</span><span class="sxs-lookup"><span data-stu-id="adc15-125">Common Name As IMEI.</span></span>|
|<span data-ttu-id="adc15-126">commonNameAsSerialNumber</span><span class="sxs-lookup"><span data-stu-id="adc15-126">commonNameAsSerialNumber</span></span>|<span data-ttu-id="adc15-127">シックス</span><span class="sxs-lookup"><span data-stu-id="adc15-127">6</span></span>|<span data-ttu-id="adc15-128">シリアル番号としての共通名。</span><span class="sxs-lookup"><span data-stu-id="adc15-128">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="adc15-129">commonNameAsAadDeviceId</span><span class="sxs-lookup"><span data-stu-id="adc15-129">commonNameAsAadDeviceId</span></span>|<span data-ttu-id="adc15-130">7</span><span class="sxs-lookup"><span data-stu-id="adc15-130">7</span></span>|<span data-ttu-id="adc15-131">シリアル番号としての共通名。</span><span class="sxs-lookup"><span data-stu-id="adc15-131">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="adc15-132">Commonnameasintアン Deviceid</span><span class="sxs-lookup"><span data-stu-id="adc15-132">commonNameAsIntuneDeviceId</span></span>|<span data-ttu-id="adc15-133">8 </span><span class="sxs-lookup"><span data-stu-id="adc15-133">8</span></span>|<span data-ttu-id="adc15-134">シリアル番号としての共通名。</span><span class="sxs-lookup"><span data-stu-id="adc15-134">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="adc15-135">commonNameAsDurableDeviceId</span><span class="sxs-lookup"><span data-stu-id="adc15-135">commonNameAsDurableDeviceId</span></span>|<span data-ttu-id="adc15-136">9 </span><span class="sxs-lookup"><span data-stu-id="adc15-136">9</span></span>|<span data-ttu-id="adc15-137">シリアル番号としての共通名。</span><span class="sxs-lookup"><span data-stu-id="adc15-137">Common Name As Serial Number.</span></span>|




