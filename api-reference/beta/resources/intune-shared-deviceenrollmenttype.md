---
title: deviceEnrollmentType 列挙型
description: 管理するモバイル デバイスを追加するための方法です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: bffe0e592240cbeee22a63dac8c339a0d3b3ff3d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946841"
---
# <a name="deviceenrollmenttype-enum-type"></a><span data-ttu-id="9c628-103">deviceEnrollmentType 列挙型</span><span class="sxs-lookup"><span data-stu-id="9c628-103">deviceEnrollmentType enum type</span></span>

> <span data-ttu-id="9c628-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9c628-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9c628-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9c628-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9c628-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9c628-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9c628-107">管理するモバイル デバイスを追加するための方法です。</span><span class="sxs-lookup"><span data-stu-id="9c628-107">Possible ways of adding a mobile device to management.</span></span>
## <a name="members"></a><span data-ttu-id="9c628-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="9c628-108">Members</span></span>
|<span data-ttu-id="9c628-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="9c628-109">Member</span></span>|<span data-ttu-id="9c628-110">値</span><span class="sxs-lookup"><span data-stu-id="9c628-110">Value</span></span>|<span data-ttu-id="9c628-111">説明</span><span class="sxs-lookup"><span data-stu-id="9c628-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c628-112">不明</span><span class="sxs-lookup"><span data-stu-id="9c628-112">unknown</span></span>|<span data-ttu-id="9c628-113">0</span><span class="sxs-lookup"><span data-stu-id="9c628-113">0</span></span>|<span data-ttu-id="9c628-114">登録型の既定値は収集されませんでした。</span><span class="sxs-lookup"><span data-stu-id="9c628-114">Default value, enrollment type was not collected.</span></span>|
|<span data-ttu-id="9c628-115">userEnrollment</span><span class="sxs-lookup"><span data-stu-id="9c628-115">userEnrollment</span></span>|<span data-ttu-id="9c628-116">1</span><span class="sxs-lookup"><span data-stu-id="9c628-116">1</span></span>|<span data-ttu-id="9c628-117">BYOD チャネルを通じてユーザー駆動の登録します。</span><span class="sxs-lookup"><span data-stu-id="9c628-117">User driven enrollment through BYOD channel.</span></span>|
|<span data-ttu-id="9c628-118">deviceEnrollmentManager</span><span class="sxs-lookup"><span data-stu-id="9c628-118">deviceEnrollmentManager</span></span>|<span data-ttu-id="9c628-119">2</span><span class="sxs-lookup"><span data-stu-id="9c628-119">2</span></span>|<span data-ttu-id="9c628-120">デバイス登録の管理者アカウントとユーザー登録します。</span><span class="sxs-lookup"><span data-stu-id="9c628-120">User enrollment with a device enrollment manager account.</span></span>|
|<span data-ttu-id="9c628-121">appleBulkWithUser</span><span class="sxs-lookup"><span data-stu-id="9c628-121">appleBulkWithUser</span></span>|<span data-ttu-id="9c628-122">3</span><span class="sxs-lookup"><span data-stu-id="9c628-122">3</span></span>|<span data-ttu-id="9c628-123">アップル一括登録はユーザーの課題です。</span><span class="sxs-lookup"><span data-stu-id="9c628-123">Apple bulk enrollment with user challenge.</span></span> <span data-ttu-id="9c628-124">(DEP、Apple の構成ウィザード)</span><span class="sxs-lookup"><span data-stu-id="9c628-124">(DEP, Apple Configurator)</span></span>|
|<span data-ttu-id="9c628-125">appleBulkWithoutUser</span><span class="sxs-lookup"><span data-stu-id="9c628-125">appleBulkWithoutUser</span></span>|<span data-ttu-id="9c628-126">4</span><span class="sxs-lookup"><span data-stu-id="9c628-126">4</span></span>|<span data-ttu-id="9c628-127">ユーザーの課題に Apple の一括登録します。</span><span class="sxs-lookup"><span data-stu-id="9c628-127">Apple bulk enrollment without user challenge.</span></span> <span data-ttu-id="9c628-128">(DEP では、Apple の構成ウィザードは、モバイルの設定)</span><span class="sxs-lookup"><span data-stu-id="9c628-128">(DEP, Apple Configurator, Mobile Config)</span></span>|
|<span data-ttu-id="9c628-129">windowsAzureADJoin</span><span class="sxs-lookup"><span data-stu-id="9c628-129">windowsAzureADJoin</span></span>|<span data-ttu-id="9c628-130">5</span><span class="sxs-lookup"><span data-stu-id="9c628-130">5</span></span>|<span data-ttu-id="9c628-131">Windows Azure AD を 10 に参加します。</span><span class="sxs-lookup"><span data-stu-id="9c628-131">Windows 10 Azure AD Join.</span></span>|
|<span data-ttu-id="9c628-132">windowsBulkUserless</span><span class="sxs-lookup"><span data-stu-id="9c628-132">windowsBulkUserless</span></span>|<span data-ttu-id="9c628-133">6</span><span class="sxs-lookup"><span data-stu-id="9c628-133">6</span></span>|<span data-ttu-id="9c628-134">証明書で ICD を Windows 10 一括登録します。</span><span class="sxs-lookup"><span data-stu-id="9c628-134">Windows 10 Bulk enrollment through ICD with certificate.</span></span>|
|<span data-ttu-id="9c628-135">windowsAutoEnrollment</span><span class="sxs-lookup"><span data-stu-id="9c628-135">windowsAutoEnrollment</span></span>|<span data-ttu-id="9c628-136">7</span><span class="sxs-lookup"><span data-stu-id="9c628-136">7</span></span>|<span data-ttu-id="9c628-137">10 の Windows の自動登録します。</span><span class="sxs-lookup"><span data-stu-id="9c628-137">Windows 10 automatic enrollment.</span></span> <span data-ttu-id="9c628-138">(勤務先のアカウントを追加)</span><span class="sxs-lookup"><span data-stu-id="9c628-138">(Add work account)</span></span>|
|<span data-ttu-id="9c628-139">windowsBulkAzureDomainJoin</span><span class="sxs-lookup"><span data-stu-id="9c628-139">windowsBulkAzureDomainJoin</span></span>|<span data-ttu-id="9c628-140">8</span><span class="sxs-lookup"><span data-stu-id="9c628-140">8</span></span>|<span data-ttu-id="9c628-141">10 の windows Azure AD に参加を一括します。</span><span class="sxs-lookup"><span data-stu-id="9c628-141">Windows 10 bulk Azure AD Join.</span></span>|
|<span data-ttu-id="9c628-142">windowsCoManagement</span><span class="sxs-lookup"><span data-stu-id="9c628-142">windowsCoManagement</span></span>|<span data-ttu-id="9c628-143">9</span><span class="sxs-lookup"><span data-stu-id="9c628-143">9</span></span>|<span data-ttu-id="9c628-144">Windows 10 共同管理自動操縦装置、またはグループ ポリシーによって発生します。</span><span class="sxs-lookup"><span data-stu-id="9c628-144">Windows 10 Co-Management triggered by AutoPilot or Group Policy.</span></span>|





