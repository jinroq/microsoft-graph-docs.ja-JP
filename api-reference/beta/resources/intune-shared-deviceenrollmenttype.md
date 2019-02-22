---
title: deviceEnrollmentType 列挙型
description: モバイルデバイスを管理に追加する方法には、次のようなものがあります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b186110c4f69ea7b6f4d12c9fb2a333927f81385
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30173655"
---
# <a name="deviceenrollmenttype-enum-type"></a><span data-ttu-id="185d3-103">deviceEnrollmentType 列挙型</span><span class="sxs-lookup"><span data-stu-id="185d3-103">deviceEnrollmentType enum type</span></span>

> <span data-ttu-id="185d3-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="185d3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="185d3-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="185d3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="185d3-106">モバイルデバイスを管理に追加する方法には、次のようなものがあります。</span><span class="sxs-lookup"><span data-stu-id="185d3-106">Possible ways of adding a mobile device to management.</span></span>

## <a name="members"></a><span data-ttu-id="185d3-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="185d3-107">Members</span></span>
|<span data-ttu-id="185d3-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="185d3-108">Member</span></span>|<span data-ttu-id="185d3-109">値</span><span class="sxs-lookup"><span data-stu-id="185d3-109">Value</span></span>|<span data-ttu-id="185d3-110">説明</span><span class="sxs-lookup"><span data-stu-id="185d3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="185d3-111">不明</span><span class="sxs-lookup"><span data-stu-id="185d3-111">unknown</span></span>|<span data-ttu-id="185d3-112">.0</span><span class="sxs-lookup"><span data-stu-id="185d3-112">0</span></span>|<span data-ttu-id="185d3-113">既定値。登録の種類は収集されませんでした。</span><span class="sxs-lookup"><span data-stu-id="185d3-113">Default value, enrollment type was not collected.</span></span>|
|<span data-ttu-id="185d3-114">userenrollment</span><span class="sxs-lookup"><span data-stu-id="185d3-114">userEnrollment</span></span>|<span data-ttu-id="185d3-115">1-d</span><span class="sxs-lookup"><span data-stu-id="185d3-115">1</span></span>|<span data-ttu-id="185d3-116">byod channel 経由のユーザー主導型の登録。</span><span class="sxs-lookup"><span data-stu-id="185d3-116">User driven enrollment through BYOD channel.</span></span>|
|<span data-ttu-id="185d3-117">deviceEnrollmentManager</span><span class="sxs-lookup"><span data-stu-id="185d3-117">deviceEnrollmentManager</span></span>|<span data-ttu-id="185d3-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="185d3-118">2</span></span>|<span data-ttu-id="185d3-119">デバイス登録マネージャーアカウントを使用したユーザー登録。</span><span class="sxs-lookup"><span data-stu-id="185d3-119">User enrollment with a device enrollment manager account.</span></span>|
|<span data-ttu-id="185d3-120">appleBulkWithUser</span><span class="sxs-lookup"><span data-stu-id="185d3-120">appleBulkWithUser</span></span>|<span data-ttu-id="185d3-121">1/3</span><span class="sxs-lookup"><span data-stu-id="185d3-121">3</span></span>|<span data-ttu-id="185d3-122">ユーザーチャレンジを使用した Apple 一括登録。</span><span class="sxs-lookup"><span data-stu-id="185d3-122">Apple bulk enrollment with user challenge.</span></span> <span data-ttu-id="185d3-123">(DEP、Apple Configurator)</span><span class="sxs-lookup"><span data-stu-id="185d3-123">(DEP, Apple Configurator)</span></span>|
|<span data-ttu-id="185d3-124">appleBulkWithoutUser</span><span class="sxs-lookup"><span data-stu-id="185d3-124">appleBulkWithoutUser</span></span>|<span data-ttu-id="185d3-125">2/4</span><span class="sxs-lookup"><span data-stu-id="185d3-125">4</span></span>|<span data-ttu-id="185d3-126">ユーザーチャレンジなしの Apple 一括登録。</span><span class="sxs-lookup"><span data-stu-id="185d3-126">Apple bulk enrollment without user challenge.</span></span> <span data-ttu-id="185d3-127">(DEP、Apple Configurator、モバイル構成)</span><span class="sxs-lookup"><span data-stu-id="185d3-127">(DEP, Apple Configurator, Mobile Config)</span></span>|
|<span data-ttu-id="185d3-128">windowsAzureADJoin</span><span class="sxs-lookup"><span data-stu-id="185d3-128">windowsAzureADJoin</span></span>|<span data-ttu-id="185d3-129">5</span><span class="sxs-lookup"><span data-stu-id="185d3-129">5</span></span>|<span data-ttu-id="185d3-130">Windows 10 Azure AD Join。</span><span class="sxs-lookup"><span data-stu-id="185d3-130">Windows 10 Azure AD Join.</span></span>|
|<span data-ttu-id="185d3-131">windowsbulkuserless</span><span class="sxs-lookup"><span data-stu-id="185d3-131">windowsBulkUserless</span></span>|<span data-ttu-id="185d3-132">シックス</span><span class="sxs-lookup"><span data-stu-id="185d3-132">6</span></span>|<span data-ttu-id="185d3-133">Windows 10 証明書を使用した ICD による一括登録。</span><span class="sxs-lookup"><span data-stu-id="185d3-133">Windows 10 Bulk enrollment through ICD with certificate.</span></span>|
|<span data-ttu-id="185d3-134">windowsautoenrollment 登録</span><span class="sxs-lookup"><span data-stu-id="185d3-134">windowsAutoEnrollment</span></span>|<span data-ttu-id="185d3-135">7</span><span class="sxs-lookup"><span data-stu-id="185d3-135">7</span></span>|<span data-ttu-id="185d3-136">Windows 10 の自動登録。</span><span class="sxs-lookup"><span data-stu-id="185d3-136">Windows 10 automatic enrollment.</span></span> <span data-ttu-id="185d3-137">(作業アカウントの追加)</span><span class="sxs-lookup"><span data-stu-id="185d3-137">(Add work account)</span></span>|
|<span data-ttu-id="185d3-138">windowsbulkazuredomainjoin</span><span class="sxs-lookup"><span data-stu-id="185d3-138">windowsBulkAzureDomainJoin</span></span>|<span data-ttu-id="185d3-139">~</span><span class="sxs-lookup"><span data-stu-id="185d3-139">8</span></span>|<span data-ttu-id="185d3-140">Windows 10 一括 Azure AD Join。</span><span class="sxs-lookup"><span data-stu-id="185d3-140">Windows 10 bulk Azure AD Join.</span></span>|
|<span data-ttu-id="185d3-141">windowsCoManagement</span><span class="sxs-lookup"><span data-stu-id="185d3-141">windowsCoManagement</span></span>|<span data-ttu-id="185d3-142">i-9</span><span class="sxs-lookup"><span data-stu-id="185d3-142">9</span></span>|<span data-ttu-id="185d3-143">Windows 10 の共同管理は、自動操縦またはグループポリシーによって開始されます。</span><span class="sxs-lookup"><span data-stu-id="185d3-143">Windows 10 Co-Management triggered by AutoPilot or Group Policy.</span></span>|




