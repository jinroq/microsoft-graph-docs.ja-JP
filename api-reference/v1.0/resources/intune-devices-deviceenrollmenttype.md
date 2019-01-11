---
title: deviceEnrollmentType 列挙型
description: 管理するモバイル デバイスを追加するための方法です。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5ba559b9f217f0af5fd64262693f0c7446e43c5b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826482"
---
# <a name="deviceenrollmenttype-enum-type"></a><span data-ttu-id="e4693-103">deviceEnrollmentType 列挙型</span><span class="sxs-lookup"><span data-stu-id="e4693-103">deviceEnrollmentType enum type</span></span>

> <span data-ttu-id="e4693-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e4693-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e4693-105">管理するモバイル デバイスを追加するための方法です。</span><span class="sxs-lookup"><span data-stu-id="e4693-105">Possible ways of adding a mobile device to management.</span></span>
## <a name="members"></a><span data-ttu-id="e4693-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="e4693-106">Members</span></span>
|<span data-ttu-id="e4693-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="e4693-107">Member</span></span>|<span data-ttu-id="e4693-108">値</span><span class="sxs-lookup"><span data-stu-id="e4693-108">Value</span></span>|<span data-ttu-id="e4693-109">説明</span><span class="sxs-lookup"><span data-stu-id="e4693-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4693-110">不明</span><span class="sxs-lookup"><span data-stu-id="e4693-110">unknown</span></span>|<span data-ttu-id="e4693-111">0</span><span class="sxs-lookup"><span data-stu-id="e4693-111">0</span></span>|<span data-ttu-id="e4693-112">登録型の既定値は収集されませんでした。</span><span class="sxs-lookup"><span data-stu-id="e4693-112">Default value, enrollment type was not collected.</span></span>|
|<span data-ttu-id="e4693-113">userEnrollment</span><span class="sxs-lookup"><span data-stu-id="e4693-113">userEnrollment</span></span>|<span data-ttu-id="e4693-114">1</span><span class="sxs-lookup"><span data-stu-id="e4693-114">1</span></span>|<span data-ttu-id="e4693-115">BYOD チャネルを通じてユーザー駆動の登録します。</span><span class="sxs-lookup"><span data-stu-id="e4693-115">User driven enrollment through BYOD channel.</span></span>|
|<span data-ttu-id="e4693-116">deviceEnrollmentManager</span><span class="sxs-lookup"><span data-stu-id="e4693-116">deviceEnrollmentManager</span></span>|<span data-ttu-id="e4693-117">2</span><span class="sxs-lookup"><span data-stu-id="e4693-117">2</span></span>|<span data-ttu-id="e4693-118">デバイス登録の管理者アカウントとユーザー登録します。</span><span class="sxs-lookup"><span data-stu-id="e4693-118">User enrollment with a device enrollment manager account.</span></span>|
|<span data-ttu-id="e4693-119">appleBulkWithUser</span><span class="sxs-lookup"><span data-stu-id="e4693-119">appleBulkWithUser</span></span>|<span data-ttu-id="e4693-120">3</span><span class="sxs-lookup"><span data-stu-id="e4693-120">3</span></span>|<span data-ttu-id="e4693-121">アップル一括登録はユーザーの課題です。</span><span class="sxs-lookup"><span data-stu-id="e4693-121">Apple bulk enrollment with user challenge.</span></span> <span data-ttu-id="e4693-122">(DEP、Apple の構成ウィザード)</span><span class="sxs-lookup"><span data-stu-id="e4693-122">(DEP, Apple Configurator)</span></span>|
|<span data-ttu-id="e4693-123">appleBulkWithoutUser</span><span class="sxs-lookup"><span data-stu-id="e4693-123">appleBulkWithoutUser</span></span>|<span data-ttu-id="e4693-124">4</span><span class="sxs-lookup"><span data-stu-id="e4693-124">4</span></span>|<span data-ttu-id="e4693-125">ユーザーの課題に Apple の一括登録します。</span><span class="sxs-lookup"><span data-stu-id="e4693-125">Apple bulk enrollment without user challenge.</span></span> <span data-ttu-id="e4693-126">(DEP では、Apple の構成ウィザードは、モバイルの設定)</span><span class="sxs-lookup"><span data-stu-id="e4693-126">(DEP, Apple Configurator, Mobile Config)</span></span>|
|<span data-ttu-id="e4693-127">windowsAzureADJoin</span><span class="sxs-lookup"><span data-stu-id="e4693-127">windowsAzureADJoin</span></span>|<span data-ttu-id="e4693-128">5</span><span class="sxs-lookup"><span data-stu-id="e4693-128">5</span></span>|<span data-ttu-id="e4693-129">Windows Azure AD を 10 に参加します。</span><span class="sxs-lookup"><span data-stu-id="e4693-129">Windows 10 Azure AD Join.</span></span>|
|<span data-ttu-id="e4693-130">windowsBulkUserless</span><span class="sxs-lookup"><span data-stu-id="e4693-130">windowsBulkUserless</span></span>|<span data-ttu-id="e4693-131">6</span><span class="sxs-lookup"><span data-stu-id="e4693-131">6</span></span>|<span data-ttu-id="e4693-132">証明書で ICD を Windows 10 一括登録します。</span><span class="sxs-lookup"><span data-stu-id="e4693-132">Windows 10 Bulk enrollment through ICD with certificate.</span></span>|
|<span data-ttu-id="e4693-133">windowsAutoEnrollment</span><span class="sxs-lookup"><span data-stu-id="e4693-133">windowsAutoEnrollment</span></span>|<span data-ttu-id="e4693-134">7</span><span class="sxs-lookup"><span data-stu-id="e4693-134">7</span></span>|<span data-ttu-id="e4693-135">10 の Windows の自動登録します。</span><span class="sxs-lookup"><span data-stu-id="e4693-135">Windows 10 automatic enrollment.</span></span> <span data-ttu-id="e4693-136">(勤務先のアカウントを追加)</span><span class="sxs-lookup"><span data-stu-id="e4693-136">(Add work account)</span></span>|
|<span data-ttu-id="e4693-137">windowsBulkAzureDomainJoin</span><span class="sxs-lookup"><span data-stu-id="e4693-137">windowsBulkAzureDomainJoin</span></span>|<span data-ttu-id="e4693-138">8</span><span class="sxs-lookup"><span data-stu-id="e4693-138">8</span></span>|<span data-ttu-id="e4693-139">10 の windows Azure AD に参加を一括します。</span><span class="sxs-lookup"><span data-stu-id="e4693-139">Windows 10 bulk Azure AD Join.</span></span>|
|<span data-ttu-id="e4693-140">windowsCoManagement</span><span class="sxs-lookup"><span data-stu-id="e4693-140">windowsCoManagement</span></span>|<span data-ttu-id="e4693-141">9</span><span class="sxs-lookup"><span data-stu-id="e4693-141">9</span></span>|<span data-ttu-id="e4693-142">Windows 10 共同管理自動操縦装置、またはグループ ポリシーによって発生します。</span><span class="sxs-lookup"><span data-stu-id="e4693-142">Windows 10 Co-Management triggered by AutoPilot or Group Policy.</span></span>|



