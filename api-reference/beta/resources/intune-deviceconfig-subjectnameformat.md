---
title: subjectNameFormat 列挙型
description: サブジェクト名の形式のオプションです。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 22bbc03da6fd3e48925634704e78ffb22abef3bc
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410330"
---
# <a name="subjectnameformat-enum-type"></a><span data-ttu-id="dd683-103">subjectNameFormat 列挙型</span><span class="sxs-lookup"><span data-stu-id="dd683-103">subjectNameFormat enum type</span></span>

> <span data-ttu-id="dd683-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="dd683-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="dd683-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dd683-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dd683-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="dd683-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dd683-107">サブジェクト名の形式のオプションです。</span><span class="sxs-lookup"><span data-stu-id="dd683-107">Subject Name Format Options.</span></span>

## <a name="members"></a><span data-ttu-id="dd683-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="dd683-108">Members</span></span>
|<span data-ttu-id="dd683-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="dd683-109">Member</span></span>|<span data-ttu-id="dd683-110">値</span><span class="sxs-lookup"><span data-stu-id="dd683-110">Value</span></span>|<span data-ttu-id="dd683-111">説明</span><span class="sxs-lookup"><span data-stu-id="dd683-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd683-112">共通</span><span class="sxs-lookup"><span data-stu-id="dd683-112">commonName</span></span>|<span data-ttu-id="dd683-113">0</span><span class="sxs-lookup"><span data-stu-id="dd683-113">0</span></span>|<span data-ttu-id="dd683-114">共通名です。</span><span class="sxs-lookup"><span data-stu-id="dd683-114">Common name.</span></span>|
|<span data-ttu-id="dd683-115">commonNameIncludingEmail</span><span class="sxs-lookup"><span data-stu-id="dd683-115">commonNameIncludingEmail</span></span>|<span data-ttu-id="dd683-116">1</span><span class="sxs-lookup"><span data-stu-id="dd683-116">1</span></span>|<span data-ttu-id="dd683-117">メールを含む共通の名前です。</span><span class="sxs-lookup"><span data-stu-id="dd683-117">Common Name Including Email.</span></span>|
|<span data-ttu-id="dd683-118">commonNameAsEmail</span><span class="sxs-lookup"><span data-stu-id="dd683-118">commonNameAsEmail</span></span>|<span data-ttu-id="dd683-119">2</span><span class="sxs-lookup"><span data-stu-id="dd683-119">2</span></span>|<span data-ttu-id="dd683-120">電子メールとの共通名です。</span><span class="sxs-lookup"><span data-stu-id="dd683-120">Common Name As Email.</span></span>|
|<span data-ttu-id="dd683-121">custom</span><span class="sxs-lookup"><span data-stu-id="dd683-121">custom</span></span>|<span data-ttu-id="dd683-122">3</span><span class="sxs-lookup"><span data-stu-id="dd683-122">3</span></span>|<span data-ttu-id="dd683-123">カスタムのサブジェクト名の形式です。</span><span class="sxs-lookup"><span data-stu-id="dd683-123">Custom subject name format.</span></span>|
|<span data-ttu-id="dd683-124">commonNameAsIMEI</span><span class="sxs-lookup"><span data-stu-id="dd683-124">commonNameAsIMEI</span></span>|<span data-ttu-id="dd683-125">5</span><span class="sxs-lookup"><span data-stu-id="dd683-125">5</span></span>|<span data-ttu-id="dd683-126">IMEI として共通の名前です。</span><span class="sxs-lookup"><span data-stu-id="dd683-126">Common Name As IMEI.</span></span>|
|<span data-ttu-id="dd683-127">commonNameAsSerialNumber</span><span class="sxs-lookup"><span data-stu-id="dd683-127">commonNameAsSerialNumber</span></span>|<span data-ttu-id="dd683-128">6</span><span class="sxs-lookup"><span data-stu-id="dd683-128">6</span></span>|<span data-ttu-id="dd683-129">シリアル番号として共通の名前です。</span><span class="sxs-lookup"><span data-stu-id="dd683-129">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="dd683-130">commonNameAsAadDeviceId</span><span class="sxs-lookup"><span data-stu-id="dd683-130">commonNameAsAadDeviceId</span></span>|<span data-ttu-id="dd683-131">7</span><span class="sxs-lookup"><span data-stu-id="dd683-131">7</span></span>|<span data-ttu-id="dd683-132">シリアル番号として共通の名前です。</span><span class="sxs-lookup"><span data-stu-id="dd683-132">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="dd683-133">commonNameAsIntuneDeviceId</span><span class="sxs-lookup"><span data-stu-id="dd683-133">commonNameAsIntuneDeviceId</span></span>|<span data-ttu-id="dd683-134">8</span><span class="sxs-lookup"><span data-stu-id="dd683-134">8</span></span>|<span data-ttu-id="dd683-135">シリアル番号として共通の名前です。</span><span class="sxs-lookup"><span data-stu-id="dd683-135">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="dd683-136">commonNameAsDurableDeviceId</span><span class="sxs-lookup"><span data-stu-id="dd683-136">commonNameAsDurableDeviceId</span></span>|<span data-ttu-id="dd683-137">9</span><span class="sxs-lookup"><span data-stu-id="dd683-137">9</span></span>|<span data-ttu-id="dd683-138">シリアル番号として共通の名前です。</span><span class="sxs-lookup"><span data-stu-id="dd683-138">Common Name As Serial Number.</span></span>|




