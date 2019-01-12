---
title: subjectNameFormat 列挙型
description: サブジェクト名の形式のオプションです。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 259af745567a0fc5de004f5a804d8bab00355f8f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27969591"
---
# <a name="subjectnameformat-enum-type"></a><span data-ttu-id="29522-103">subjectNameFormat 列挙型</span><span class="sxs-lookup"><span data-stu-id="29522-103">subjectNameFormat enum type</span></span>

> <span data-ttu-id="29522-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="29522-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="29522-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="29522-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="29522-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="29522-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="29522-107">サブジェクト名の形式のオプションです。</span><span class="sxs-lookup"><span data-stu-id="29522-107">Subject Name Format Options.</span></span>
## <a name="members"></a><span data-ttu-id="29522-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="29522-108">Members</span></span>
|<span data-ttu-id="29522-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="29522-109">Member</span></span>|<span data-ttu-id="29522-110">値</span><span class="sxs-lookup"><span data-stu-id="29522-110">Value</span></span>|<span data-ttu-id="29522-111">説明</span><span class="sxs-lookup"><span data-stu-id="29522-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29522-112">共通</span><span class="sxs-lookup"><span data-stu-id="29522-112">commonName</span></span>|<span data-ttu-id="29522-113">0</span><span class="sxs-lookup"><span data-stu-id="29522-113">0</span></span>|<span data-ttu-id="29522-114">共通名です。</span><span class="sxs-lookup"><span data-stu-id="29522-114">Common name.</span></span>|
|<span data-ttu-id="29522-115">commonNameIncludingEmail</span><span class="sxs-lookup"><span data-stu-id="29522-115">commonNameIncludingEmail</span></span>|<span data-ttu-id="29522-116">1</span><span class="sxs-lookup"><span data-stu-id="29522-116">1</span></span>|<span data-ttu-id="29522-117">メールを含む共通の名前です。</span><span class="sxs-lookup"><span data-stu-id="29522-117">Common Name Including Email.</span></span>|
|<span data-ttu-id="29522-118">commonNameAsEmail</span><span class="sxs-lookup"><span data-stu-id="29522-118">commonNameAsEmail</span></span>|<span data-ttu-id="29522-119">2</span><span class="sxs-lookup"><span data-stu-id="29522-119">2</span></span>|<span data-ttu-id="29522-120">電子メールとの共通名です。</span><span class="sxs-lookup"><span data-stu-id="29522-120">Common Name As Email.</span></span>|
|<span data-ttu-id="29522-121">custom</span><span class="sxs-lookup"><span data-stu-id="29522-121">custom</span></span>|<span data-ttu-id="29522-122">3</span><span class="sxs-lookup"><span data-stu-id="29522-122">3</span></span>|<span data-ttu-id="29522-123">カスタムのサブジェクト名の形式です。</span><span class="sxs-lookup"><span data-stu-id="29522-123">Custom subject name format.</span></span>|
|<span data-ttu-id="29522-124">commonNameAsIMEI</span><span class="sxs-lookup"><span data-stu-id="29522-124">commonNameAsIMEI</span></span>|<span data-ttu-id="29522-125">5</span><span class="sxs-lookup"><span data-stu-id="29522-125">5</span></span>|<span data-ttu-id="29522-126">IMEI として共通の名前です。</span><span class="sxs-lookup"><span data-stu-id="29522-126">Common Name As IMEI.</span></span>|
|<span data-ttu-id="29522-127">commonNameAsSerialNumber</span><span class="sxs-lookup"><span data-stu-id="29522-127">commonNameAsSerialNumber</span></span>|<span data-ttu-id="29522-128">6</span><span class="sxs-lookup"><span data-stu-id="29522-128">6</span></span>|<span data-ttu-id="29522-129">シリアル番号として共通の名前です。</span><span class="sxs-lookup"><span data-stu-id="29522-129">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="29522-130">commonNameAsAadDeviceId</span><span class="sxs-lookup"><span data-stu-id="29522-130">commonNameAsAadDeviceId</span></span>|<span data-ttu-id="29522-131">7</span><span class="sxs-lookup"><span data-stu-id="29522-131">7</span></span>|<span data-ttu-id="29522-132">シリアル番号として共通の名前です。</span><span class="sxs-lookup"><span data-stu-id="29522-132">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="29522-133">commonNameAsIntuneDeviceId</span><span class="sxs-lookup"><span data-stu-id="29522-133">commonNameAsIntuneDeviceId</span></span>|<span data-ttu-id="29522-134">8</span><span class="sxs-lookup"><span data-stu-id="29522-134">8</span></span>|<span data-ttu-id="29522-135">シリアル番号として共通の名前です。</span><span class="sxs-lookup"><span data-stu-id="29522-135">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="29522-136">commonNameAsDurableDeviceId</span><span class="sxs-lookup"><span data-stu-id="29522-136">commonNameAsDurableDeviceId</span></span>|<span data-ttu-id="29522-137">9</span><span class="sxs-lookup"><span data-stu-id="29522-137">9</span></span>|<span data-ttu-id="29522-138">シリアル番号として共通の名前です。</span><span class="sxs-lookup"><span data-stu-id="29522-138">Common Name As Serial Number.</span></span>|





