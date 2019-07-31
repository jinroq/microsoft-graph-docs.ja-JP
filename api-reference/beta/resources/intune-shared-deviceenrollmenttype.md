---
title: deviceEnrollmentType 列挙型
description: モバイルデバイスを管理に追加する方法には、次のようなものがあります。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 89efb76eb78121937dd2f0558986af0df1750aa9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967470"
---
# <a name="deviceenrollmenttype-enum-type"></a><span data-ttu-id="9f4ec-103">deviceEnrollmentType 列挙型</span><span class="sxs-lookup"><span data-stu-id="9f4ec-103">deviceEnrollmentType enum type</span></span>

> <span data-ttu-id="9f4ec-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9f4ec-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9f4ec-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9f4ec-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f4ec-106">モバイルデバイスを管理に追加する方法には、次のようなものがあります。</span><span class="sxs-lookup"><span data-stu-id="9f4ec-106">Possible ways of adding a mobile device to management.</span></span>

## <a name="members"></a><span data-ttu-id="9f4ec-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="9f4ec-107">Members</span></span>
|<span data-ttu-id="9f4ec-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="9f4ec-108">Member</span></span>|<span data-ttu-id="9f4ec-109">値</span><span class="sxs-lookup"><span data-stu-id="9f4ec-109">Value</span></span>|<span data-ttu-id="9f4ec-110">説明</span><span class="sxs-lookup"><span data-stu-id="9f4ec-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f4ec-111">不明</span><span class="sxs-lookup"><span data-stu-id="9f4ec-111">unknown</span></span>|<span data-ttu-id="9f4ec-112">.0</span><span class="sxs-lookup"><span data-stu-id="9f4ec-112">0</span></span>|<span data-ttu-id="9f4ec-113">既定値。登録の種類は収集されませんでした。</span><span class="sxs-lookup"><span data-stu-id="9f4ec-113">Default value, enrollment type was not collected.</span></span>|
|<span data-ttu-id="9f4ec-114">userEnrollment</span><span class="sxs-lookup"><span data-stu-id="9f4ec-114">userEnrollment</span></span>|<span data-ttu-id="9f4ec-115">1-d</span><span class="sxs-lookup"><span data-stu-id="9f4ec-115">1</span></span>|<span data-ttu-id="9f4ec-116">BYOD channel 経由のユーザー主導型の登録。</span><span class="sxs-lookup"><span data-stu-id="9f4ec-116">User driven enrollment through BYOD channel.</span></span>|
|<span data-ttu-id="9f4ec-117">deviceEnrollmentManager</span><span class="sxs-lookup"><span data-stu-id="9f4ec-117">deviceEnrollmentManager</span></span>|<span data-ttu-id="9f4ec-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="9f4ec-118">2</span></span>|<span data-ttu-id="9f4ec-119">デバイス登録マネージャーアカウントを使用したユーザー登録。</span><span class="sxs-lookup"><span data-stu-id="9f4ec-119">User enrollment with a device enrollment manager account.</span></span>|
|<span data-ttu-id="9f4ec-120">appleBulkWithUser</span><span class="sxs-lookup"><span data-stu-id="9f4ec-120">appleBulkWithUser</span></span>|<span data-ttu-id="9f4ec-121">1/3</span><span class="sxs-lookup"><span data-stu-id="9f4ec-121">3</span></span>|<span data-ttu-id="9f4ec-122">ユーザーチャレンジを使用した Apple 一括登録。</span><span class="sxs-lookup"><span data-stu-id="9f4ec-122">Apple bulk enrollment with user challenge.</span></span> <span data-ttu-id="9f4ec-123">(DEP、Apple Configurator)</span><span class="sxs-lookup"><span data-stu-id="9f4ec-123">(DEP, Apple Configurator)</span></span>|
|<span data-ttu-id="9f4ec-124">appleBulkWithoutUser</span><span class="sxs-lookup"><span data-stu-id="9f4ec-124">appleBulkWithoutUser</span></span>|<span data-ttu-id="9f4ec-125">2/4</span><span class="sxs-lookup"><span data-stu-id="9f4ec-125">4</span></span>|<span data-ttu-id="9f4ec-126">ユーザーチャレンジなしの Apple 一括登録。</span><span class="sxs-lookup"><span data-stu-id="9f4ec-126">Apple bulk enrollment without user challenge.</span></span> <span data-ttu-id="9f4ec-127">(DEP、Apple Configurator、モバイル構成)</span><span class="sxs-lookup"><span data-stu-id="9f4ec-127">(DEP, Apple Configurator, Mobile Config)</span></span>|
|<span data-ttu-id="9f4ec-128">windowsAzureADJoin</span><span class="sxs-lookup"><span data-stu-id="9f4ec-128">windowsAzureADJoin</span></span>|<span data-ttu-id="9f4ec-129">5</span><span class="sxs-lookup"><span data-stu-id="9f4ec-129">5</span></span>|<span data-ttu-id="9f4ec-130">Windows 10 Azure AD Join。</span><span class="sxs-lookup"><span data-stu-id="9f4ec-130">Windows 10 Azure AD Join.</span></span>|
|<span data-ttu-id="9f4ec-131">windowsBulkUserless</span><span class="sxs-lookup"><span data-stu-id="9f4ec-131">windowsBulkUserless</span></span>|<span data-ttu-id="9f4ec-132">シックス</span><span class="sxs-lookup"><span data-stu-id="9f4ec-132">6</span></span>|<span data-ttu-id="9f4ec-133">Windows 10 証明書を使用した ICD による一括登録。</span><span class="sxs-lookup"><span data-stu-id="9f4ec-133">Windows 10 Bulk enrollment through ICD with certificate.</span></span>|
|<span data-ttu-id="9f4ec-134">windowsAutoEnrollment 登録</span><span class="sxs-lookup"><span data-stu-id="9f4ec-134">windowsAutoEnrollment</span></span>|<span data-ttu-id="9f4ec-135">7</span><span class="sxs-lookup"><span data-stu-id="9f4ec-135">7</span></span>|<span data-ttu-id="9f4ec-136">Windows 10 の自動登録。</span><span class="sxs-lookup"><span data-stu-id="9f4ec-136">Windows 10 automatic enrollment.</span></span> <span data-ttu-id="9f4ec-137">(作業アカウントの追加)</span><span class="sxs-lookup"><span data-stu-id="9f4ec-137">(Add work account)</span></span>|
|<span data-ttu-id="9f4ec-138">windowsBulkAzureDomainJoin</span><span class="sxs-lookup"><span data-stu-id="9f4ec-138">windowsBulkAzureDomainJoin</span></span>|<span data-ttu-id="9f4ec-139">8 </span><span class="sxs-lookup"><span data-stu-id="9f4ec-139">8</span></span>|<span data-ttu-id="9f4ec-140">Windows 10 一括 Azure AD Join。</span><span class="sxs-lookup"><span data-stu-id="9f4ec-140">Windows 10 bulk Azure AD Join.</span></span>|
|<span data-ttu-id="9f4ec-141">windowsCoManagement</span><span class="sxs-lookup"><span data-stu-id="9f4ec-141">windowsCoManagement</span></span>|<span data-ttu-id="9f4ec-142">9 </span><span class="sxs-lookup"><span data-stu-id="9f4ec-142">9</span></span>|<span data-ttu-id="9f4ec-143">Windows 10 の共同管理は、自動操縦またはグループポリシーによって開始されます。</span><span class="sxs-lookup"><span data-stu-id="9f4ec-143">Windows 10 Co-Management triggered by AutoPilot or Group Policy.</span></span>|





