---
title: deviceEnrollmentType 列挙型
description: モバイルデバイスを管理に追加する方法には、次のようなものがあります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 62ff257e2f758776265f52a0d64cde52dbc26115
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32585364"
---
# <a name="deviceenrollmenttype-enum-type"></a><span data-ttu-id="103e1-103">deviceEnrollmentType 列挙型</span><span class="sxs-lookup"><span data-stu-id="103e1-103">deviceEnrollmentType enum type</span></span>

> <span data-ttu-id="103e1-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="103e1-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="103e1-105">モバイルデバイスを管理に追加する方法には、次のようなものがあります。</span><span class="sxs-lookup"><span data-stu-id="103e1-105">Possible ways of adding a mobile device to management.</span></span>

## <a name="members"></a><span data-ttu-id="103e1-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="103e1-106">Members</span></span>
|<span data-ttu-id="103e1-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="103e1-107">Member</span></span>|<span data-ttu-id="103e1-108">値</span><span class="sxs-lookup"><span data-stu-id="103e1-108">Value</span></span>|<span data-ttu-id="103e1-109">説明</span><span class="sxs-lookup"><span data-stu-id="103e1-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="103e1-110">不明</span><span class="sxs-lookup"><span data-stu-id="103e1-110">unknown</span></span>|<span data-ttu-id="103e1-111">.0</span><span class="sxs-lookup"><span data-stu-id="103e1-111">0</span></span>|<span data-ttu-id="103e1-112">既定値。登録の種類は収集されませんでした。</span><span class="sxs-lookup"><span data-stu-id="103e1-112">Default value, enrollment type was not collected.</span></span>|
|<span data-ttu-id="103e1-113">userenrollment</span><span class="sxs-lookup"><span data-stu-id="103e1-113">userEnrollment</span></span>|<span data-ttu-id="103e1-114">1-d</span><span class="sxs-lookup"><span data-stu-id="103e1-114">1</span></span>|<span data-ttu-id="103e1-115">byod channel 経由のユーザー主導型の登録。</span><span class="sxs-lookup"><span data-stu-id="103e1-115">User driven enrollment through BYOD channel.</span></span>|
|<span data-ttu-id="103e1-116">deviceEnrollmentManager</span><span class="sxs-lookup"><span data-stu-id="103e1-116">deviceEnrollmentManager</span></span>|<span data-ttu-id="103e1-117">pbm-2</span><span class="sxs-lookup"><span data-stu-id="103e1-117">2</span></span>|<span data-ttu-id="103e1-118">デバイス登録マネージャーアカウントを使用したユーザー登録。</span><span class="sxs-lookup"><span data-stu-id="103e1-118">User enrollment with a device enrollment manager account.</span></span>|
|<span data-ttu-id="103e1-119">appleBulkWithUser</span><span class="sxs-lookup"><span data-stu-id="103e1-119">appleBulkWithUser</span></span>|<span data-ttu-id="103e1-120">1/3</span><span class="sxs-lookup"><span data-stu-id="103e1-120">3</span></span>|<span data-ttu-id="103e1-121">ユーザーチャレンジを使用した Apple 一括登録。</span><span class="sxs-lookup"><span data-stu-id="103e1-121">Apple bulk enrollment with user challenge.</span></span> <span data-ttu-id="103e1-122">(DEP、Apple Configurator)</span><span class="sxs-lookup"><span data-stu-id="103e1-122">(DEP, Apple Configurator)</span></span>|
|<span data-ttu-id="103e1-123">appleBulkWithoutUser</span><span class="sxs-lookup"><span data-stu-id="103e1-123">appleBulkWithoutUser</span></span>|<span data-ttu-id="103e1-124">2/4</span><span class="sxs-lookup"><span data-stu-id="103e1-124">4</span></span>|<span data-ttu-id="103e1-125">ユーザーチャレンジなしの Apple 一括登録。</span><span class="sxs-lookup"><span data-stu-id="103e1-125">Apple bulk enrollment without user challenge.</span></span> <span data-ttu-id="103e1-126">(DEP、Apple Configurator、モバイル構成)</span><span class="sxs-lookup"><span data-stu-id="103e1-126">(DEP, Apple Configurator, Mobile Config)</span></span>|
|<span data-ttu-id="103e1-127">windowsAzureADJoin</span><span class="sxs-lookup"><span data-stu-id="103e1-127">windowsAzureADJoin</span></span>|<span data-ttu-id="103e1-128">5</span><span class="sxs-lookup"><span data-stu-id="103e1-128">5</span></span>|<span data-ttu-id="103e1-129">Windows 10 Azure AD Join。</span><span class="sxs-lookup"><span data-stu-id="103e1-129">Windows 10 Azure AD Join.</span></span>|
|<span data-ttu-id="103e1-130">windowsbulkuserless</span><span class="sxs-lookup"><span data-stu-id="103e1-130">windowsBulkUserless</span></span>|<span data-ttu-id="103e1-131">シックス</span><span class="sxs-lookup"><span data-stu-id="103e1-131">6</span></span>|<span data-ttu-id="103e1-132">Windows 10 証明書を使用した ICD による一括登録。</span><span class="sxs-lookup"><span data-stu-id="103e1-132">Windows 10 Bulk enrollment through ICD with certificate.</span></span>|
|<span data-ttu-id="103e1-133">windowsautoenrollment 登録</span><span class="sxs-lookup"><span data-stu-id="103e1-133">windowsAutoEnrollment</span></span>|<span data-ttu-id="103e1-134">7</span><span class="sxs-lookup"><span data-stu-id="103e1-134">7</span></span>|<span data-ttu-id="103e1-135">Windows 10 の自動登録。</span><span class="sxs-lookup"><span data-stu-id="103e1-135">Windows 10 automatic enrollment.</span></span> <span data-ttu-id="103e1-136">(作業アカウントの追加)</span><span class="sxs-lookup"><span data-stu-id="103e1-136">(Add work account)</span></span>|
|<span data-ttu-id="103e1-137">windowsbulkazuredomainjoin</span><span class="sxs-lookup"><span data-stu-id="103e1-137">windowsBulkAzureDomainJoin</span></span>|<span data-ttu-id="103e1-138">~</span><span class="sxs-lookup"><span data-stu-id="103e1-138">8</span></span>|<span data-ttu-id="103e1-139">Windows 10 一括 Azure AD Join。</span><span class="sxs-lookup"><span data-stu-id="103e1-139">Windows 10 bulk Azure AD Join.</span></span>|
|<span data-ttu-id="103e1-140">windowsCoManagement</span><span class="sxs-lookup"><span data-stu-id="103e1-140">windowsCoManagement</span></span>|<span data-ttu-id="103e1-141">i-9</span><span class="sxs-lookup"><span data-stu-id="103e1-141">9</span></span>|<span data-ttu-id="103e1-142">Windows 10 の共同管理は、自動操縦またはグループポリシーによって開始されます。</span><span class="sxs-lookup"><span data-stu-id="103e1-142">Windows 10 Co-Management triggered by AutoPilot or Group Policy.</span></span>|



