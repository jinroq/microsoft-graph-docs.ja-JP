---
title: deviceEnrollmentType 列挙型
description: モバイルデバイスを管理に追加する方法には、次のようなものがあります。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 0b53d279863ad3e17691b9e4d0397ba5f7d1b408
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36372084"
---
# <a name="deviceenrollmenttype-enum-type"></a><span data-ttu-id="f54d9-103">deviceEnrollmentType 列挙型</span><span class="sxs-lookup"><span data-stu-id="f54d9-103">deviceEnrollmentType enum type</span></span>

> <span data-ttu-id="f54d9-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f54d9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f54d9-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f54d9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f54d9-106">モバイルデバイスを管理に追加する方法には、次のようなものがあります。</span><span class="sxs-lookup"><span data-stu-id="f54d9-106">Possible ways of adding a mobile device to management.</span></span>

## <a name="members"></a><span data-ttu-id="f54d9-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="f54d9-107">Members</span></span>
|<span data-ttu-id="f54d9-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="f54d9-108">Member</span></span>|<span data-ttu-id="f54d9-109">値</span><span class="sxs-lookup"><span data-stu-id="f54d9-109">Value</span></span>|<span data-ttu-id="f54d9-110">説明</span><span class="sxs-lookup"><span data-stu-id="f54d9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f54d9-111">不明</span><span class="sxs-lookup"><span data-stu-id="f54d9-111">unknown</span></span>|<span data-ttu-id="f54d9-112">.0</span><span class="sxs-lookup"><span data-stu-id="f54d9-112">0</span></span>|<span data-ttu-id="f54d9-113">既定値。登録の種類は収集されませんでした。</span><span class="sxs-lookup"><span data-stu-id="f54d9-113">Default value, enrollment type was not collected.</span></span>|
|<span data-ttu-id="f54d9-114">userEnrollment</span><span class="sxs-lookup"><span data-stu-id="f54d9-114">userEnrollment</span></span>|<span data-ttu-id="f54d9-115">1-d</span><span class="sxs-lookup"><span data-stu-id="f54d9-115">1</span></span>|<span data-ttu-id="f54d9-116">BYOD channel 経由のユーザー主導型の登録。</span><span class="sxs-lookup"><span data-stu-id="f54d9-116">User driven enrollment through BYOD channel.</span></span>|
|<span data-ttu-id="f54d9-117">deviceEnrollmentManager</span><span class="sxs-lookup"><span data-stu-id="f54d9-117">deviceEnrollmentManager</span></span>|<span data-ttu-id="f54d9-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="f54d9-118">2</span></span>|<span data-ttu-id="f54d9-119">デバイス登録マネージャーアカウントを使用したユーザー登録。</span><span class="sxs-lookup"><span data-stu-id="f54d9-119">User enrollment with a device enrollment manager account.</span></span>|
|<span data-ttu-id="f54d9-120">appleBulkWithUser</span><span class="sxs-lookup"><span data-stu-id="f54d9-120">appleBulkWithUser</span></span>|<span data-ttu-id="f54d9-121">1/3</span><span class="sxs-lookup"><span data-stu-id="f54d9-121">3</span></span>|<span data-ttu-id="f54d9-122">ユーザーチャレンジを使用した Apple 一括登録。</span><span class="sxs-lookup"><span data-stu-id="f54d9-122">Apple bulk enrollment with user challenge.</span></span> <span data-ttu-id="f54d9-123">(DEP、Apple Configurator)</span><span class="sxs-lookup"><span data-stu-id="f54d9-123">(DEP, Apple Configurator)</span></span>|
|<span data-ttu-id="f54d9-124">appleBulkWithoutUser</span><span class="sxs-lookup"><span data-stu-id="f54d9-124">appleBulkWithoutUser</span></span>|<span data-ttu-id="f54d9-125">2/4</span><span class="sxs-lookup"><span data-stu-id="f54d9-125">4</span></span>|<span data-ttu-id="f54d9-126">ユーザーチャレンジなしの Apple 一括登録。</span><span class="sxs-lookup"><span data-stu-id="f54d9-126">Apple bulk enrollment without user challenge.</span></span> <span data-ttu-id="f54d9-127">(DEP、Apple Configurator、モバイル構成)</span><span class="sxs-lookup"><span data-stu-id="f54d9-127">(DEP, Apple Configurator, Mobile Config)</span></span>|
|<span data-ttu-id="f54d9-128">windowsAzureADJoin</span><span class="sxs-lookup"><span data-stu-id="f54d9-128">windowsAzureADJoin</span></span>|<span data-ttu-id="f54d9-129">5</span><span class="sxs-lookup"><span data-stu-id="f54d9-129">5</span></span>|<span data-ttu-id="f54d9-130">Windows 10 Azure AD Join。</span><span class="sxs-lookup"><span data-stu-id="f54d9-130">Windows 10 Azure AD Join.</span></span>|
|<span data-ttu-id="f54d9-131">windowsBulkUserless</span><span class="sxs-lookup"><span data-stu-id="f54d9-131">windowsBulkUserless</span></span>|<span data-ttu-id="f54d9-132">シックス</span><span class="sxs-lookup"><span data-stu-id="f54d9-132">6</span></span>|<span data-ttu-id="f54d9-133">Windows 10 証明書を使用した ICD による一括登録。</span><span class="sxs-lookup"><span data-stu-id="f54d9-133">Windows 10 Bulk enrollment through ICD with certificate.</span></span>|
|<span data-ttu-id="f54d9-134">windowsAutoEnrollment 登録</span><span class="sxs-lookup"><span data-stu-id="f54d9-134">windowsAutoEnrollment</span></span>|<span data-ttu-id="f54d9-135">7</span><span class="sxs-lookup"><span data-stu-id="f54d9-135">7</span></span>|<span data-ttu-id="f54d9-136">Windows 10 の自動登録。</span><span class="sxs-lookup"><span data-stu-id="f54d9-136">Windows 10 automatic enrollment.</span></span> <span data-ttu-id="f54d9-137">(作業アカウントの追加)</span><span class="sxs-lookup"><span data-stu-id="f54d9-137">(Add work account)</span></span>|
|<span data-ttu-id="f54d9-138">windowsBulkAzureDomainJoin</span><span class="sxs-lookup"><span data-stu-id="f54d9-138">windowsBulkAzureDomainJoin</span></span>|<span data-ttu-id="f54d9-139">8 </span><span class="sxs-lookup"><span data-stu-id="f54d9-139">8</span></span>|<span data-ttu-id="f54d9-140">Windows 10 一括 Azure AD Join。</span><span class="sxs-lookup"><span data-stu-id="f54d9-140">Windows 10 bulk Azure AD Join.</span></span>|
|<span data-ttu-id="f54d9-141">windowsCoManagement</span><span class="sxs-lookup"><span data-stu-id="f54d9-141">windowsCoManagement</span></span>|<span data-ttu-id="f54d9-142">9 </span><span class="sxs-lookup"><span data-stu-id="f54d9-142">9</span></span>|<span data-ttu-id="f54d9-143">Windows 10 の共同管理は、自動操縦またはグループポリシーによって開始されます。</span><span class="sxs-lookup"><span data-stu-id="f54d9-143">Windows 10 Co-Management triggered by AutoPilot or Group Policy.</span></span>|



