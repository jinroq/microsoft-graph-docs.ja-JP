---
title: deviceEnrollmentType 列挙型
description: 管理するモバイル デバイスを追加するための方法です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: aed1f40604a765b1a434bca35dbb356e65e8ccd5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399291"
---
# <a name="deviceenrollmenttype-enum-type"></a><span data-ttu-id="11a80-103">deviceEnrollmentType 列挙型</span><span class="sxs-lookup"><span data-stu-id="11a80-103">deviceEnrollmentType enum type</span></span>

> <span data-ttu-id="11a80-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="11a80-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="11a80-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="11a80-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="11a80-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="11a80-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11a80-107">管理するモバイル デバイスを追加するための方法です。</span><span class="sxs-lookup"><span data-stu-id="11a80-107">Possible ways of adding a mobile device to management.</span></span>

## <a name="members"></a><span data-ttu-id="11a80-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="11a80-108">Members</span></span>
|<span data-ttu-id="11a80-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="11a80-109">Member</span></span>|<span data-ttu-id="11a80-110">値</span><span class="sxs-lookup"><span data-stu-id="11a80-110">Value</span></span>|<span data-ttu-id="11a80-111">説明</span><span class="sxs-lookup"><span data-stu-id="11a80-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11a80-112">不明</span><span class="sxs-lookup"><span data-stu-id="11a80-112">unknown</span></span>|<span data-ttu-id="11a80-113">0</span><span class="sxs-lookup"><span data-stu-id="11a80-113">0</span></span>|<span data-ttu-id="11a80-114">登録型の既定値は収集されませんでした。</span><span class="sxs-lookup"><span data-stu-id="11a80-114">Default value, enrollment type was not collected.</span></span>|
|<span data-ttu-id="11a80-115">userEnrollment</span><span class="sxs-lookup"><span data-stu-id="11a80-115">userEnrollment</span></span>|<span data-ttu-id="11a80-116">1</span><span class="sxs-lookup"><span data-stu-id="11a80-116">1</span></span>|<span data-ttu-id="11a80-117">BYOD チャネルを通じてユーザー駆動の登録します。</span><span class="sxs-lookup"><span data-stu-id="11a80-117">User driven enrollment through BYOD channel.</span></span>|
|<span data-ttu-id="11a80-118">deviceEnrollmentManager</span><span class="sxs-lookup"><span data-stu-id="11a80-118">deviceEnrollmentManager</span></span>|<span data-ttu-id="11a80-119">2</span><span class="sxs-lookup"><span data-stu-id="11a80-119">2</span></span>|<span data-ttu-id="11a80-120">デバイス登録の管理者アカウントとユーザー登録します。</span><span class="sxs-lookup"><span data-stu-id="11a80-120">User enrollment with a device enrollment manager account.</span></span>|
|<span data-ttu-id="11a80-121">appleBulkWithUser</span><span class="sxs-lookup"><span data-stu-id="11a80-121">appleBulkWithUser</span></span>|<span data-ttu-id="11a80-122">3</span><span class="sxs-lookup"><span data-stu-id="11a80-122">3</span></span>|<span data-ttu-id="11a80-123">アップル一括登録はユーザーの課題です。</span><span class="sxs-lookup"><span data-stu-id="11a80-123">Apple bulk enrollment with user challenge.</span></span> <span data-ttu-id="11a80-124">(DEP、Apple の構成ウィザード)</span><span class="sxs-lookup"><span data-stu-id="11a80-124">(DEP, Apple Configurator)</span></span>|
|<span data-ttu-id="11a80-125">appleBulkWithoutUser</span><span class="sxs-lookup"><span data-stu-id="11a80-125">appleBulkWithoutUser</span></span>|<span data-ttu-id="11a80-126">4</span><span class="sxs-lookup"><span data-stu-id="11a80-126">4</span></span>|<span data-ttu-id="11a80-127">ユーザーの課題に Apple の一括登録します。</span><span class="sxs-lookup"><span data-stu-id="11a80-127">Apple bulk enrollment without user challenge.</span></span> <span data-ttu-id="11a80-128">(DEP では、Apple の構成ウィザードは、モバイルの設定)</span><span class="sxs-lookup"><span data-stu-id="11a80-128">(DEP, Apple Configurator, Mobile Config)</span></span>|
|<span data-ttu-id="11a80-129">windowsAzureADJoin</span><span class="sxs-lookup"><span data-stu-id="11a80-129">windowsAzureADJoin</span></span>|<span data-ttu-id="11a80-130">5</span><span class="sxs-lookup"><span data-stu-id="11a80-130">5</span></span>|<span data-ttu-id="11a80-131">Windows Azure AD を 10 に参加します。</span><span class="sxs-lookup"><span data-stu-id="11a80-131">Windows 10 Azure AD Join.</span></span>|
|<span data-ttu-id="11a80-132">windowsBulkUserless</span><span class="sxs-lookup"><span data-stu-id="11a80-132">windowsBulkUserless</span></span>|<span data-ttu-id="11a80-133">6</span><span class="sxs-lookup"><span data-stu-id="11a80-133">6</span></span>|<span data-ttu-id="11a80-134">証明書で ICD を Windows 10 一括登録します。</span><span class="sxs-lookup"><span data-stu-id="11a80-134">Windows 10 Bulk enrollment through ICD with certificate.</span></span>|
|<span data-ttu-id="11a80-135">windowsAutoEnrollment</span><span class="sxs-lookup"><span data-stu-id="11a80-135">windowsAutoEnrollment</span></span>|<span data-ttu-id="11a80-136">7</span><span class="sxs-lookup"><span data-stu-id="11a80-136">7</span></span>|<span data-ttu-id="11a80-137">10 の Windows の自動登録します。</span><span class="sxs-lookup"><span data-stu-id="11a80-137">Windows 10 automatic enrollment.</span></span> <span data-ttu-id="11a80-138">(勤務先のアカウントを追加)</span><span class="sxs-lookup"><span data-stu-id="11a80-138">(Add work account)</span></span>|
|<span data-ttu-id="11a80-139">windowsBulkAzureDomainJoin</span><span class="sxs-lookup"><span data-stu-id="11a80-139">windowsBulkAzureDomainJoin</span></span>|<span data-ttu-id="11a80-140">8</span><span class="sxs-lookup"><span data-stu-id="11a80-140">8</span></span>|<span data-ttu-id="11a80-141">10 の windows Azure AD に参加を一括します。</span><span class="sxs-lookup"><span data-stu-id="11a80-141">Windows 10 bulk Azure AD Join.</span></span>|
|<span data-ttu-id="11a80-142">windowsCoManagement</span><span class="sxs-lookup"><span data-stu-id="11a80-142">windowsCoManagement</span></span>|<span data-ttu-id="11a80-143">9</span><span class="sxs-lookup"><span data-stu-id="11a80-143">9</span></span>|<span data-ttu-id="11a80-144">Windows 10 共同管理自動操縦装置、またはグループ ポリシーによって発生します。</span><span class="sxs-lookup"><span data-stu-id="11a80-144">Windows 10 Co-Management triggered by AutoPilot or Group Policy.</span></span>|




