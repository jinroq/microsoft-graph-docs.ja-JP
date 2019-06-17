---
title: subjectNameFormat 列挙型
description: サブジェクト名の形式オプション。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e3f047571f0cd4874c9542fbc1dda7e83dfae4b6
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34964165"
---
# <a name="subjectnameformat-enum-type"></a><span data-ttu-id="4785b-103">subjectNameFormat 列挙型</span><span class="sxs-lookup"><span data-stu-id="4785b-103">subjectNameFormat enum type</span></span>

> <span data-ttu-id="4785b-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4785b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4785b-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4785b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4785b-106">サブジェクト名の形式オプション。</span><span class="sxs-lookup"><span data-stu-id="4785b-106">Subject Name Format Options.</span></span>

## <a name="members"></a><span data-ttu-id="4785b-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="4785b-107">Members</span></span>
|<span data-ttu-id="4785b-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="4785b-108">Member</span></span>|<span data-ttu-id="4785b-109">値</span><span class="sxs-lookup"><span data-stu-id="4785b-109">Value</span></span>|<span data-ttu-id="4785b-110">説明</span><span class="sxs-lookup"><span data-stu-id="4785b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4785b-111">commonName</span><span class="sxs-lookup"><span data-stu-id="4785b-111">commonName</span></span>|<span data-ttu-id="4785b-112">.0</span><span class="sxs-lookup"><span data-stu-id="4785b-112">0</span></span>|<span data-ttu-id="4785b-113">共通名。</span><span class="sxs-lookup"><span data-stu-id="4785b-113">Common name.</span></span>|
|<span data-ttu-id="4785b-114">Commonnamecommon電子メール</span><span class="sxs-lookup"><span data-stu-id="4785b-114">commonNameIncludingEmail</span></span>|<span data-ttu-id="4785b-115">1-d</span><span class="sxs-lookup"><span data-stu-id="4785b-115">1</span></span>|<span data-ttu-id="4785b-116">電子メールを含む共通名。</span><span class="sxs-lookup"><span data-stu-id="4785b-116">Common Name Including Email.</span></span>|
|<span data-ttu-id="4785b-117">commonNameAsEmail</span><span class="sxs-lookup"><span data-stu-id="4785b-117">commonNameAsEmail</span></span>|<span data-ttu-id="4785b-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="4785b-118">2</span></span>|<span data-ttu-id="4785b-119">電子メールとしての共通名。</span><span class="sxs-lookup"><span data-stu-id="4785b-119">Common Name As Email.</span></span>|
|<span data-ttu-id="4785b-120">配色</span><span class="sxs-lookup"><span data-stu-id="4785b-120">custom</span></span>|<span data-ttu-id="4785b-121">1/3</span><span class="sxs-lookup"><span data-stu-id="4785b-121">3</span></span>|<span data-ttu-id="4785b-122">カスタムサブジェクト名の形式。</span><span class="sxs-lookup"><span data-stu-id="4785b-122">Custom subject name format.</span></span>|
|<span data-ttu-id="4785b-123">commonNameAsIMEI</span><span class="sxs-lookup"><span data-stu-id="4785b-123">commonNameAsIMEI</span></span>|<span data-ttu-id="4785b-124">5</span><span class="sxs-lookup"><span data-stu-id="4785b-124">5</span></span>|<span data-ttu-id="4785b-125">IMEI としての共通名。</span><span class="sxs-lookup"><span data-stu-id="4785b-125">Common Name As IMEI.</span></span>|
|<span data-ttu-id="4785b-126">commonNameAsSerialNumber</span><span class="sxs-lookup"><span data-stu-id="4785b-126">commonNameAsSerialNumber</span></span>|<span data-ttu-id="4785b-127">シックス</span><span class="sxs-lookup"><span data-stu-id="4785b-127">6</span></span>|<span data-ttu-id="4785b-128">シリアル番号としての共通名。</span><span class="sxs-lookup"><span data-stu-id="4785b-128">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="4785b-129">commonNameAsAadDeviceId</span><span class="sxs-lookup"><span data-stu-id="4785b-129">commonNameAsAadDeviceId</span></span>|<span data-ttu-id="4785b-130">7</span><span class="sxs-lookup"><span data-stu-id="4785b-130">7</span></span>|<span data-ttu-id="4785b-131">シリアル番号としての共通名。</span><span class="sxs-lookup"><span data-stu-id="4785b-131">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="4785b-132">Commonnameasintアン Deviceid</span><span class="sxs-lookup"><span data-stu-id="4785b-132">commonNameAsIntuneDeviceId</span></span>|<span data-ttu-id="4785b-133">8 </span><span class="sxs-lookup"><span data-stu-id="4785b-133">8</span></span>|<span data-ttu-id="4785b-134">シリアル番号としての共通名。</span><span class="sxs-lookup"><span data-stu-id="4785b-134">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="4785b-135">commonNameAsDurableDeviceId</span><span class="sxs-lookup"><span data-stu-id="4785b-135">commonNameAsDurableDeviceId</span></span>|<span data-ttu-id="4785b-136">9 </span><span class="sxs-lookup"><span data-stu-id="4785b-136">9</span></span>|<span data-ttu-id="4785b-137">シリアル番号としての共通名。</span><span class="sxs-lookup"><span data-stu-id="4785b-137">Common Name As Serial Number.</span></span>|





