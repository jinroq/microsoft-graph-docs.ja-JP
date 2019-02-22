---
title: subjectNameFormat 列挙型
description: サブジェクト名の形式オプション。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6f12068576ff78d74f2e1b6119a2030ff7835a7d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30158556"
---
# <a name="subjectnameformat-enum-type"></a><span data-ttu-id="a6fc5-103">subjectNameFormat 列挙型</span><span class="sxs-lookup"><span data-stu-id="a6fc5-103">subjectNameFormat enum type</span></span>

> <span data-ttu-id="a6fc5-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a6fc5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a6fc5-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a6fc5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6fc5-106">サブジェクト名の形式オプション。</span><span class="sxs-lookup"><span data-stu-id="a6fc5-106">Subject Name Format Options.</span></span>

## <a name="members"></a><span data-ttu-id="a6fc5-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="a6fc5-107">Members</span></span>
|<span data-ttu-id="a6fc5-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="a6fc5-108">Member</span></span>|<span data-ttu-id="a6fc5-109">値</span><span class="sxs-lookup"><span data-stu-id="a6fc5-109">Value</span></span>|<span data-ttu-id="a6fc5-110">説明</span><span class="sxs-lookup"><span data-stu-id="a6fc5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6fc5-111">commonname</span><span class="sxs-lookup"><span data-stu-id="a6fc5-111">commonName</span></span>|<span data-ttu-id="a6fc5-112">.0</span><span class="sxs-lookup"><span data-stu-id="a6fc5-112">0</span></span>|<span data-ttu-id="a6fc5-113">共通名。</span><span class="sxs-lookup"><span data-stu-id="a6fc5-113">Common name.</span></span>|
|<span data-ttu-id="a6fc5-114">commonnamecommon電子メール</span><span class="sxs-lookup"><span data-stu-id="a6fc5-114">commonNameIncludingEmail</span></span>|<span data-ttu-id="a6fc5-115">1-d</span><span class="sxs-lookup"><span data-stu-id="a6fc5-115">1</span></span>|<span data-ttu-id="a6fc5-116">電子メールを含む共通名。</span><span class="sxs-lookup"><span data-stu-id="a6fc5-116">Common Name Including Email.</span></span>|
|<span data-ttu-id="a6fc5-117">commonnameasemail</span><span class="sxs-lookup"><span data-stu-id="a6fc5-117">commonNameAsEmail</span></span>|<span data-ttu-id="a6fc5-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="a6fc5-118">2</span></span>|<span data-ttu-id="a6fc5-119">電子メールとしての共通名。</span><span class="sxs-lookup"><span data-stu-id="a6fc5-119">Common Name As Email.</span></span>|
|<span data-ttu-id="a6fc5-120">custom</span><span class="sxs-lookup"><span data-stu-id="a6fc5-120">custom</span></span>|<span data-ttu-id="a6fc5-121">1/3</span><span class="sxs-lookup"><span data-stu-id="a6fc5-121">3</span></span>|<span data-ttu-id="a6fc5-122">カスタムサブジェクト名の形式。</span><span class="sxs-lookup"><span data-stu-id="a6fc5-122">Custom subject name format.</span></span>|
|<span data-ttu-id="a6fc5-123">commonnameasimei</span><span class="sxs-lookup"><span data-stu-id="a6fc5-123">commonNameAsIMEI</span></span>|<span data-ttu-id="a6fc5-124">5</span><span class="sxs-lookup"><span data-stu-id="a6fc5-124">5</span></span>|<span data-ttu-id="a6fc5-125">IMEI としての共通名。</span><span class="sxs-lookup"><span data-stu-id="a6fc5-125">Common Name As IMEI.</span></span>|
|<span data-ttu-id="a6fc5-126">commonnameasserialnumber</span><span class="sxs-lookup"><span data-stu-id="a6fc5-126">commonNameAsSerialNumber</span></span>|<span data-ttu-id="a6fc5-127">シックス</span><span class="sxs-lookup"><span data-stu-id="a6fc5-127">6</span></span>|<span data-ttu-id="a6fc5-128">シリアル番号としての共通名。</span><span class="sxs-lookup"><span data-stu-id="a6fc5-128">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="a6fc5-129">commonNameAsAadDeviceId</span><span class="sxs-lookup"><span data-stu-id="a6fc5-129">commonNameAsAadDeviceId</span></span>|<span data-ttu-id="a6fc5-130">7</span><span class="sxs-lookup"><span data-stu-id="a6fc5-130">7</span></span>|<span data-ttu-id="a6fc5-131">シリアル番号としての共通名。</span><span class="sxs-lookup"><span data-stu-id="a6fc5-131">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="a6fc5-132">commonnameasintアン deviceid</span><span class="sxs-lookup"><span data-stu-id="a6fc5-132">commonNameAsIntuneDeviceId</span></span>|<span data-ttu-id="a6fc5-133">~</span><span class="sxs-lookup"><span data-stu-id="a6fc5-133">8</span></span>|<span data-ttu-id="a6fc5-134">シリアル番号としての共通名。</span><span class="sxs-lookup"><span data-stu-id="a6fc5-134">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="a6fc5-135">commonNameAsDurableDeviceId</span><span class="sxs-lookup"><span data-stu-id="a6fc5-135">commonNameAsDurableDeviceId</span></span>|<span data-ttu-id="a6fc5-136">i-9</span><span class="sxs-lookup"><span data-stu-id="a6fc5-136">9</span></span>|<span data-ttu-id="a6fc5-137">シリアル番号としての共通名。</span><span class="sxs-lookup"><span data-stu-id="a6fc5-137">Common Name As Serial Number.</span></span>|




