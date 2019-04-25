---
title: deviceEnrollmentType 列挙型
description: モバイルデバイスを管理に追加する方法には、次のようなものがあります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b186110c4f69ea7b6f4d12c9fb2a333927f81385
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32524590"
---
# <a name="deviceenrollmenttype-enum-type"></a><span data-ttu-id="e3a9c-103">deviceEnrollmentType 列挙型</span><span class="sxs-lookup"><span data-stu-id="e3a9c-103">deviceEnrollmentType enum type</span></span>

> <span data-ttu-id="e3a9c-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e3a9c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e3a9c-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e3a9c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3a9c-106">モバイルデバイスを管理に追加する方法には、次のようなものがあります。</span><span class="sxs-lookup"><span data-stu-id="e3a9c-106">Possible ways of adding a mobile device to management.</span></span>

## <a name="members"></a><span data-ttu-id="e3a9c-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="e3a9c-107">Members</span></span>
|<span data-ttu-id="e3a9c-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="e3a9c-108">Member</span></span>|<span data-ttu-id="e3a9c-109">値</span><span class="sxs-lookup"><span data-stu-id="e3a9c-109">Value</span></span>|<span data-ttu-id="e3a9c-110">説明</span><span class="sxs-lookup"><span data-stu-id="e3a9c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3a9c-111">不明</span><span class="sxs-lookup"><span data-stu-id="e3a9c-111">unknown</span></span>|<span data-ttu-id="e3a9c-112">.0</span><span class="sxs-lookup"><span data-stu-id="e3a9c-112">0</span></span>|<span data-ttu-id="e3a9c-113">既定値。登録の種類は収集されませんでした。</span><span class="sxs-lookup"><span data-stu-id="e3a9c-113">Default value, enrollment type was not collected.</span></span>|
|<span data-ttu-id="e3a9c-114">userenrollment</span><span class="sxs-lookup"><span data-stu-id="e3a9c-114">userEnrollment</span></span>|<span data-ttu-id="e3a9c-115">1 </span><span class="sxs-lookup"><span data-stu-id="e3a9c-115">1</span></span>|<span data-ttu-id="e3a9c-116">byod channel 経由のユーザー主導型の登録。</span><span class="sxs-lookup"><span data-stu-id="e3a9c-116">User driven enrollment through BYOD channel.</span></span>|
|<span data-ttu-id="e3a9c-117">deviceEnrollmentManager</span><span class="sxs-lookup"><span data-stu-id="e3a9c-117">deviceEnrollmentManager</span></span>|<span data-ttu-id="e3a9c-118">2 </span><span class="sxs-lookup"><span data-stu-id="e3a9c-118">2</span></span>|<span data-ttu-id="e3a9c-119">デバイス登録マネージャーアカウントを使用したユーザー登録。</span><span class="sxs-lookup"><span data-stu-id="e3a9c-119">User enrollment with a device enrollment manager account.</span></span>|
|<span data-ttu-id="e3a9c-120">appleBulkWithUser</span><span class="sxs-lookup"><span data-stu-id="e3a9c-120">appleBulkWithUser</span></span>|<span data-ttu-id="e3a9c-121">3 </span><span class="sxs-lookup"><span data-stu-id="e3a9c-121">3</span></span>|<span data-ttu-id="e3a9c-122">ユーザーチャレンジを使用した Apple 一括登録。</span><span class="sxs-lookup"><span data-stu-id="e3a9c-122">Apple bulk enrollment with user challenge.</span></span> <span data-ttu-id="e3a9c-123">(DEP、Apple Configurator)</span><span class="sxs-lookup"><span data-stu-id="e3a9c-123">(DEP, Apple Configurator)</span></span>|
|<span data-ttu-id="e3a9c-124">appleBulkWithoutUser</span><span class="sxs-lookup"><span data-stu-id="e3a9c-124">appleBulkWithoutUser</span></span>|<span data-ttu-id="e3a9c-125">4 </span><span class="sxs-lookup"><span data-stu-id="e3a9c-125">4</span></span>|<span data-ttu-id="e3a9c-126">ユーザーチャレンジなしの Apple 一括登録。</span><span class="sxs-lookup"><span data-stu-id="e3a9c-126">Apple bulk enrollment without user challenge.</span></span> <span data-ttu-id="e3a9c-127">(DEP、Apple Configurator、モバイル構成)</span><span class="sxs-lookup"><span data-stu-id="e3a9c-127">(DEP, Apple Configurator, Mobile Config)</span></span>|
|<span data-ttu-id="e3a9c-128">windowsAzureADJoin</span><span class="sxs-lookup"><span data-stu-id="e3a9c-128">windowsAzureADJoin</span></span>|<span data-ttu-id="e3a9c-129">5 </span><span class="sxs-lookup"><span data-stu-id="e3a9c-129">5</span></span>|<span data-ttu-id="e3a9c-130">Windows 10 Azure AD Join。</span><span class="sxs-lookup"><span data-stu-id="e3a9c-130">Windows 10 Azure AD Join.</span></span>|
|<span data-ttu-id="e3a9c-131">windowsbulkuserless</span><span class="sxs-lookup"><span data-stu-id="e3a9c-131">windowsBulkUserless</span></span>|<span data-ttu-id="e3a9c-132">6 </span><span class="sxs-lookup"><span data-stu-id="e3a9c-132">6</span></span>|<span data-ttu-id="e3a9c-133">Windows 10 証明書を使用した ICD による一括登録。</span><span class="sxs-lookup"><span data-stu-id="e3a9c-133">Windows 10 Bulk enrollment through ICD with certificate.</span></span>|
|<span data-ttu-id="e3a9c-134">windowsautoenrollment 登録</span><span class="sxs-lookup"><span data-stu-id="e3a9c-134">windowsAutoEnrollment</span></span>|<span data-ttu-id="e3a9c-135">7 </span><span class="sxs-lookup"><span data-stu-id="e3a9c-135">7</span></span>|<span data-ttu-id="e3a9c-136">Windows 10 の自動登録。</span><span class="sxs-lookup"><span data-stu-id="e3a9c-136">Windows 10 automatic enrollment.</span></span> <span data-ttu-id="e3a9c-137">(作業アカウントの追加)</span><span class="sxs-lookup"><span data-stu-id="e3a9c-137">(Add work account)</span></span>|
|<span data-ttu-id="e3a9c-138">windowsbulkazuredomainjoin</span><span class="sxs-lookup"><span data-stu-id="e3a9c-138">windowsBulkAzureDomainJoin</span></span>|<span data-ttu-id="e3a9c-139">8 </span><span class="sxs-lookup"><span data-stu-id="e3a9c-139">8</span></span>|<span data-ttu-id="e3a9c-140">Windows 10 一括 Azure AD Join。</span><span class="sxs-lookup"><span data-stu-id="e3a9c-140">Windows 10 bulk Azure AD Join.</span></span>|
|<span data-ttu-id="e3a9c-141">windowsCoManagement</span><span class="sxs-lookup"><span data-stu-id="e3a9c-141">windowsCoManagement</span></span>|<span data-ttu-id="e3a9c-142">9 </span><span class="sxs-lookup"><span data-stu-id="e3a9c-142">9</span></span>|<span data-ttu-id="e3a9c-143">Windows 10 の共同管理は、自動操縦またはグループポリシーによって開始されます。</span><span class="sxs-lookup"><span data-stu-id="e3a9c-143">Windows 10 Co-Management triggered by AutoPilot or Group Policy.</span></span>|




