---
title: subjectNameFormat 列挙型
description: サブジェクト名の形式のオプションです。
ms.openlocfilehash: 7299558011c471f02e5c1149da6ac23183faa150
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066643"
---
# <a name="subjectnameformat-enum-type"></a><span data-ttu-id="fffdb-103">subjectNameFormat 列挙型</span><span class="sxs-lookup"><span data-stu-id="fffdb-103">subjectNameFormat enum type</span></span>

> <span data-ttu-id="fffdb-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fffdb-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fffdb-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fffdb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fffdb-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="fffdb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fffdb-107">サブジェクト名の形式のオプションです。</span><span class="sxs-lookup"><span data-stu-id="fffdb-107">Subject Name Format Options.</span></span>
## <a name="members"></a><span data-ttu-id="fffdb-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="fffdb-108">Members</span></span>
|<span data-ttu-id="fffdb-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="fffdb-109">Member</span></span>|<span data-ttu-id="fffdb-110">値</span><span class="sxs-lookup"><span data-stu-id="fffdb-110">Value</span></span>|<span data-ttu-id="fffdb-111">説明</span><span class="sxs-lookup"><span data-stu-id="fffdb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fffdb-112">共通</span><span class="sxs-lookup"><span data-stu-id="fffdb-112">commonName</span></span>|<span data-ttu-id="fffdb-113">0</span><span class="sxs-lookup"><span data-stu-id="fffdb-113">0</span></span>|<span data-ttu-id="fffdb-114">共通名です。</span><span class="sxs-lookup"><span data-stu-id="fffdb-114">Common name.</span></span>|
|<span data-ttu-id="fffdb-115">commonNameIncludingEmail</span><span class="sxs-lookup"><span data-stu-id="fffdb-115">commonNameIncludingEmail</span></span>|<span data-ttu-id="fffdb-116">1</span><span class="sxs-lookup"><span data-stu-id="fffdb-116">1</span></span>|<span data-ttu-id="fffdb-117">メールを含む共通の名前です。</span><span class="sxs-lookup"><span data-stu-id="fffdb-117">Common Name Including Email.</span></span>|
|<span data-ttu-id="fffdb-118">commonNameAsEmail</span><span class="sxs-lookup"><span data-stu-id="fffdb-118">commonNameAsEmail</span></span>|<span data-ttu-id="fffdb-119">2</span><span class="sxs-lookup"><span data-stu-id="fffdb-119">2</span></span>|<span data-ttu-id="fffdb-120">電子メールとの共通名です。</span><span class="sxs-lookup"><span data-stu-id="fffdb-120">Common Name As Email.</span></span>|
|<span data-ttu-id="fffdb-121">custom</span><span class="sxs-lookup"><span data-stu-id="fffdb-121">custom</span></span>|<span data-ttu-id="fffdb-122">3</span><span class="sxs-lookup"><span data-stu-id="fffdb-122">3</span></span>|<span data-ttu-id="fffdb-123">カスタムのサブジェクト名の形式です。</span><span class="sxs-lookup"><span data-stu-id="fffdb-123">Custom subject name format.</span></span>|
|<span data-ttu-id="fffdb-124">commonNameAsIMEI</span><span class="sxs-lookup"><span data-stu-id="fffdb-124">commonNameAsIMEI</span></span>|<span data-ttu-id="fffdb-125">5</span><span class="sxs-lookup"><span data-stu-id="fffdb-125">5</span></span>|<span data-ttu-id="fffdb-126">IMEI として共通の名前です。</span><span class="sxs-lookup"><span data-stu-id="fffdb-126">Common Name As IMEI.</span></span>|
|<span data-ttu-id="fffdb-127">commonNameAsSerialNumber</span><span class="sxs-lookup"><span data-stu-id="fffdb-127">commonNameAsSerialNumber</span></span>|<span data-ttu-id="fffdb-128">6</span><span class="sxs-lookup"><span data-stu-id="fffdb-128">6</span></span>|<span data-ttu-id="fffdb-129">シリアル番号として共通の名前です。</span><span class="sxs-lookup"><span data-stu-id="fffdb-129">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="fffdb-130">commonNameAsAadDeviceId</span><span class="sxs-lookup"><span data-stu-id="fffdb-130">commonNameAsAadDeviceId</span></span>|<span data-ttu-id="fffdb-131">7</span><span class="sxs-lookup"><span data-stu-id="fffdb-131">7</span></span>|<span data-ttu-id="fffdb-132">シリアル番号として共通の名前です。</span><span class="sxs-lookup"><span data-stu-id="fffdb-132">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="fffdb-133">commonNameAsIntuneDeviceId</span><span class="sxs-lookup"><span data-stu-id="fffdb-133">commonNameAsIntuneDeviceId</span></span>|<span data-ttu-id="fffdb-134">8</span><span class="sxs-lookup"><span data-stu-id="fffdb-134">8</span></span>|<span data-ttu-id="fffdb-135">シリアル番号として共通の名前です。</span><span class="sxs-lookup"><span data-stu-id="fffdb-135">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="fffdb-136">commonNameAsDurableDeviceId</span><span class="sxs-lookup"><span data-stu-id="fffdb-136">commonNameAsDurableDeviceId</span></span>|<span data-ttu-id="fffdb-137">9</span><span class="sxs-lookup"><span data-stu-id="fffdb-137">9</span></span>|<span data-ttu-id="fffdb-138">シリアル番号として共通の名前です。</span><span class="sxs-lookup"><span data-stu-id="fffdb-138">Common Name As Serial Number.</span></span>|





