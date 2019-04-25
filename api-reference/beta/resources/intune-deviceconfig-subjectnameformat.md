---
title: subjectNameFormat 列挙型
description: サブジェクト名の形式オプション。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6202deb0a225da136216eddbb44818cb3ba3a3c5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32548678"
---
# <a name="subjectnameformat-enum-type"></a><span data-ttu-id="d18be-103">subjectNameFormat 列挙型</span><span class="sxs-lookup"><span data-stu-id="d18be-103">subjectNameFormat enum type</span></span>

> <span data-ttu-id="d18be-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d18be-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d18be-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d18be-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d18be-106">サブジェクト名の形式オプション。</span><span class="sxs-lookup"><span data-stu-id="d18be-106">Subject Name Format Options.</span></span>

## <a name="members"></a><span data-ttu-id="d18be-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="d18be-107">Members</span></span>
|<span data-ttu-id="d18be-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="d18be-108">Member</span></span>|<span data-ttu-id="d18be-109">値</span><span class="sxs-lookup"><span data-stu-id="d18be-109">Value</span></span>|<span data-ttu-id="d18be-110">説明</span><span class="sxs-lookup"><span data-stu-id="d18be-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d18be-111">commonname</span><span class="sxs-lookup"><span data-stu-id="d18be-111">commonName</span></span>|<span data-ttu-id="d18be-112">.0</span><span class="sxs-lookup"><span data-stu-id="d18be-112">0</span></span>|<span data-ttu-id="d18be-113">共通名。</span><span class="sxs-lookup"><span data-stu-id="d18be-113">Common name.</span></span>|
|<span data-ttu-id="d18be-114">commonnamecommon電子メール</span><span class="sxs-lookup"><span data-stu-id="d18be-114">commonNameIncludingEmail</span></span>|<span data-ttu-id="d18be-115">1 </span><span class="sxs-lookup"><span data-stu-id="d18be-115">1</span></span>|<span data-ttu-id="d18be-116">電子メールを含む共通名。</span><span class="sxs-lookup"><span data-stu-id="d18be-116">Common Name Including Email.</span></span>|
|<span data-ttu-id="d18be-117">commonnameasemail</span><span class="sxs-lookup"><span data-stu-id="d18be-117">commonNameAsEmail</span></span>|<span data-ttu-id="d18be-118">2 </span><span class="sxs-lookup"><span data-stu-id="d18be-118">2</span></span>|<span data-ttu-id="d18be-119">電子メールとしての共通名。</span><span class="sxs-lookup"><span data-stu-id="d18be-119">Common Name As Email.</span></span>|
|<span data-ttu-id="d18be-120">配色</span><span class="sxs-lookup"><span data-stu-id="d18be-120">custom</span></span>|<span data-ttu-id="d18be-121">3 </span><span class="sxs-lookup"><span data-stu-id="d18be-121">3</span></span>|<span data-ttu-id="d18be-122">カスタムサブジェクト名の形式。</span><span class="sxs-lookup"><span data-stu-id="d18be-122">Custom subject name format.</span></span>|
|<span data-ttu-id="d18be-123">commonnameasimei</span><span class="sxs-lookup"><span data-stu-id="d18be-123">commonNameAsIMEI</span></span>|<span data-ttu-id="d18be-124">5 </span><span class="sxs-lookup"><span data-stu-id="d18be-124">5</span></span>|<span data-ttu-id="d18be-125">IMEI としての共通名。</span><span class="sxs-lookup"><span data-stu-id="d18be-125">Common Name As IMEI.</span></span>|
|<span data-ttu-id="d18be-126">commonnameasserialnumber</span><span class="sxs-lookup"><span data-stu-id="d18be-126">commonNameAsSerialNumber</span></span>|<span data-ttu-id="d18be-127">6 </span><span class="sxs-lookup"><span data-stu-id="d18be-127">6</span></span>|<span data-ttu-id="d18be-128">シリアル番号としての共通名。</span><span class="sxs-lookup"><span data-stu-id="d18be-128">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="d18be-129">commonNameAsAadDeviceId</span><span class="sxs-lookup"><span data-stu-id="d18be-129">commonNameAsAadDeviceId</span></span>|<span data-ttu-id="d18be-130">7 </span><span class="sxs-lookup"><span data-stu-id="d18be-130">7</span></span>|<span data-ttu-id="d18be-131">シリアル番号としての共通名。</span><span class="sxs-lookup"><span data-stu-id="d18be-131">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="d18be-132">commonnameasintアン deviceid</span><span class="sxs-lookup"><span data-stu-id="d18be-132">commonNameAsIntuneDeviceId</span></span>|<span data-ttu-id="d18be-133">8 </span><span class="sxs-lookup"><span data-stu-id="d18be-133">8</span></span>|<span data-ttu-id="d18be-134">シリアル番号としての共通名。</span><span class="sxs-lookup"><span data-stu-id="d18be-134">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="d18be-135">commonNameAsDurableDeviceId</span><span class="sxs-lookup"><span data-stu-id="d18be-135">commonNameAsDurableDeviceId</span></span>|<span data-ttu-id="d18be-136">9 </span><span class="sxs-lookup"><span data-stu-id="d18be-136">9</span></span>|<span data-ttu-id="d18be-137">シリアル番号としての共通名。</span><span class="sxs-lookup"><span data-stu-id="d18be-137">Common Name As Serial Number.</span></span>|





