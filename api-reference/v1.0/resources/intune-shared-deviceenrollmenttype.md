---
title: deviceEnrollmentType 列挙型
description: モバイルデバイスを管理に追加する方法には、次のようなものがあります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: afb007893ac0b41d4439635ed78b528058d41364
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036961"
---
# <a name="deviceenrollmenttype-enum-type"></a><span data-ttu-id="75650-103">deviceEnrollmentType 列挙型</span><span class="sxs-lookup"><span data-stu-id="75650-103">deviceEnrollmentType enum type</span></span>

> <span data-ttu-id="75650-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="75650-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75650-105">モバイルデバイスを管理に追加する方法には、次のようなものがあります。</span><span class="sxs-lookup"><span data-stu-id="75650-105">Possible ways of adding a mobile device to management.</span></span>

## <a name="members"></a><span data-ttu-id="75650-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="75650-106">Members</span></span>
|<span data-ttu-id="75650-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="75650-107">Member</span></span>|<span data-ttu-id="75650-108">値</span><span class="sxs-lookup"><span data-stu-id="75650-108">Value</span></span>|<span data-ttu-id="75650-109">説明</span><span class="sxs-lookup"><span data-stu-id="75650-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75650-110">不明</span><span class="sxs-lookup"><span data-stu-id="75650-110">unknown</span></span>|<span data-ttu-id="75650-111">.0</span><span class="sxs-lookup"><span data-stu-id="75650-111">0</span></span>|<span data-ttu-id="75650-112">既定値。登録の種類は収集されませんでした。</span><span class="sxs-lookup"><span data-stu-id="75650-112">Default value, enrollment type was not collected.</span></span>|
|<span data-ttu-id="75650-113">userEnrollment</span><span class="sxs-lookup"><span data-stu-id="75650-113">userEnrollment</span></span>|<span data-ttu-id="75650-114">1-d</span><span class="sxs-lookup"><span data-stu-id="75650-114">1</span></span>|<span data-ttu-id="75650-115">BYOD channel 経由のユーザー主導型の登録。</span><span class="sxs-lookup"><span data-stu-id="75650-115">User driven enrollment through BYOD channel.</span></span>|
|<span data-ttu-id="75650-116">deviceEnrollmentManager</span><span class="sxs-lookup"><span data-stu-id="75650-116">deviceEnrollmentManager</span></span>|<span data-ttu-id="75650-117">pbm-2</span><span class="sxs-lookup"><span data-stu-id="75650-117">2</span></span>|<span data-ttu-id="75650-118">デバイス登録マネージャーアカウントを使用したユーザー登録。</span><span class="sxs-lookup"><span data-stu-id="75650-118">User enrollment with a device enrollment manager account.</span></span>|
|<span data-ttu-id="75650-119">appleBulkWithUser</span><span class="sxs-lookup"><span data-stu-id="75650-119">appleBulkWithUser</span></span>|<span data-ttu-id="75650-120">1/3</span><span class="sxs-lookup"><span data-stu-id="75650-120">3</span></span>|<span data-ttu-id="75650-121">ユーザーチャレンジを使用した Apple 一括登録。</span><span class="sxs-lookup"><span data-stu-id="75650-121">Apple bulk enrollment with user challenge.</span></span> <span data-ttu-id="75650-122">(DEP、Apple Configurator)</span><span class="sxs-lookup"><span data-stu-id="75650-122">(DEP, Apple Configurator)</span></span>|
|<span data-ttu-id="75650-123">appleBulkWithoutUser</span><span class="sxs-lookup"><span data-stu-id="75650-123">appleBulkWithoutUser</span></span>|<span data-ttu-id="75650-124">2/4</span><span class="sxs-lookup"><span data-stu-id="75650-124">4</span></span>|<span data-ttu-id="75650-125">ユーザーチャレンジなしの Apple 一括登録。</span><span class="sxs-lookup"><span data-stu-id="75650-125">Apple bulk enrollment without user challenge.</span></span> <span data-ttu-id="75650-126">(DEP、Apple Configurator、モバイル構成)</span><span class="sxs-lookup"><span data-stu-id="75650-126">(DEP, Apple Configurator, Mobile Config)</span></span>|
|<span data-ttu-id="75650-127">windowsAzureADJoin</span><span class="sxs-lookup"><span data-stu-id="75650-127">windowsAzureADJoin</span></span>|<span data-ttu-id="75650-128">5</span><span class="sxs-lookup"><span data-stu-id="75650-128">5</span></span>|<span data-ttu-id="75650-129">Windows 10 Azure AD Join。</span><span class="sxs-lookup"><span data-stu-id="75650-129">Windows 10 Azure AD Join.</span></span>|
|<span data-ttu-id="75650-130">windowsBulkUserless</span><span class="sxs-lookup"><span data-stu-id="75650-130">windowsBulkUserless</span></span>|<span data-ttu-id="75650-131">シックス</span><span class="sxs-lookup"><span data-stu-id="75650-131">6</span></span>|<span data-ttu-id="75650-132">Windows 10 証明書を使用した ICD による一括登録。</span><span class="sxs-lookup"><span data-stu-id="75650-132">Windows 10 Bulk enrollment through ICD with certificate.</span></span>|
|<span data-ttu-id="75650-133">windowsAutoEnrollment 登録</span><span class="sxs-lookup"><span data-stu-id="75650-133">windowsAutoEnrollment</span></span>|<span data-ttu-id="75650-134">7</span><span class="sxs-lookup"><span data-stu-id="75650-134">7</span></span>|<span data-ttu-id="75650-135">Windows 10 の自動登録。</span><span class="sxs-lookup"><span data-stu-id="75650-135">Windows 10 automatic enrollment.</span></span> <span data-ttu-id="75650-136">(作業アカウントの追加)</span><span class="sxs-lookup"><span data-stu-id="75650-136">(Add work account)</span></span>|
|<span data-ttu-id="75650-137">windowsBulkAzureDomainJoin</span><span class="sxs-lookup"><span data-stu-id="75650-137">windowsBulkAzureDomainJoin</span></span>|<span data-ttu-id="75650-138">8 </span><span class="sxs-lookup"><span data-stu-id="75650-138">8</span></span>|<span data-ttu-id="75650-139">Windows 10 一括 Azure AD Join。</span><span class="sxs-lookup"><span data-stu-id="75650-139">Windows 10 bulk Azure AD Join.</span></span>|
|<span data-ttu-id="75650-140">windowsCoManagement</span><span class="sxs-lookup"><span data-stu-id="75650-140">windowsCoManagement</span></span>|<span data-ttu-id="75650-141">9 </span><span class="sxs-lookup"><span data-stu-id="75650-141">9</span></span>|<span data-ttu-id="75650-142">Windows 10 の共同管理は、自動操縦またはグループポリシーによって開始されます。</span><span class="sxs-lookup"><span data-stu-id="75650-142">Windows 10 Co-Management triggered by AutoPilot or Group Policy.</span></span>|



