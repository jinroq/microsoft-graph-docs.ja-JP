---
title: deviceEnrollmentType 列挙型
description: 管理するモバイル デバイスを追加するための方法です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 72acbdf412ebb91269fcdc3f851ffbc204e0274b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987756"
---
# <a name="deviceenrollmenttype-enum-type"></a><span data-ttu-id="1a320-103">deviceEnrollmentType 列挙型</span><span class="sxs-lookup"><span data-stu-id="1a320-103">deviceEnrollmentType enum type</span></span>

> <span data-ttu-id="1a320-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1a320-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1a320-105">管理するモバイル デバイスを追加するための方法です。</span><span class="sxs-lookup"><span data-stu-id="1a320-105">Possible ways of adding a mobile device to management.</span></span>

## <a name="members"></a><span data-ttu-id="1a320-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="1a320-106">Members</span></span>
|<span data-ttu-id="1a320-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="1a320-107">Member</span></span>|<span data-ttu-id="1a320-108">値</span><span class="sxs-lookup"><span data-stu-id="1a320-108">Value</span></span>|<span data-ttu-id="1a320-109">説明</span><span class="sxs-lookup"><span data-stu-id="1a320-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a320-110">不明</span><span class="sxs-lookup"><span data-stu-id="1a320-110">unknown</span></span>|<span data-ttu-id="1a320-111">0</span><span class="sxs-lookup"><span data-stu-id="1a320-111">0</span></span>|<span data-ttu-id="1a320-112">登録型の既定値は収集されませんでした。</span><span class="sxs-lookup"><span data-stu-id="1a320-112">Default value, enrollment type was not collected.</span></span>|
|<span data-ttu-id="1a320-113">userEnrollment</span><span class="sxs-lookup"><span data-stu-id="1a320-113">userEnrollment</span></span>|<span data-ttu-id="1a320-114">1</span><span class="sxs-lookup"><span data-stu-id="1a320-114">1</span></span>|<span data-ttu-id="1a320-115">BYOD チャネルを通じてユーザー駆動の登録します。</span><span class="sxs-lookup"><span data-stu-id="1a320-115">User driven enrollment through BYOD channel.</span></span>|
|<span data-ttu-id="1a320-116">deviceEnrollmentManager</span><span class="sxs-lookup"><span data-stu-id="1a320-116">deviceEnrollmentManager</span></span>|<span data-ttu-id="1a320-117">2</span><span class="sxs-lookup"><span data-stu-id="1a320-117">2</span></span>|<span data-ttu-id="1a320-118">デバイス登録の管理者アカウントとユーザー登録します。</span><span class="sxs-lookup"><span data-stu-id="1a320-118">User enrollment with a device enrollment manager account.</span></span>|
|<span data-ttu-id="1a320-119">appleBulkWithUser</span><span class="sxs-lookup"><span data-stu-id="1a320-119">appleBulkWithUser</span></span>|<span data-ttu-id="1a320-120">3</span><span class="sxs-lookup"><span data-stu-id="1a320-120">3</span></span>|<span data-ttu-id="1a320-121">アップル一括登録はユーザーのチャレンジ (DEP、Apple Configurator)。</span><span class="sxs-lookup"><span data-stu-id="1a320-121">Apple bulk enrollment with user challenge (DEP, Apple Configurator).</span></span>|
|<span data-ttu-id="1a320-122">appleBulkWithoutUser</span><span class="sxs-lookup"><span data-stu-id="1a320-122">appleBulkWithoutUser</span></span>|<span data-ttu-id="1a320-123">4</span><span class="sxs-lookup"><span data-stu-id="1a320-123">4</span></span>|<span data-ttu-id="1a320-124">ユーザーの課題 (DEP では、Apple の構成ウィザードは、モバイルの設定) にアップル一括登録します。</span><span class="sxs-lookup"><span data-stu-id="1a320-124">Apple bulk enrollment without user challenge (DEP, Apple Configurator, Mobile Config).</span></span>|
|<span data-ttu-id="1a320-125">windowsAzureADJoin</span><span class="sxs-lookup"><span data-stu-id="1a320-125">windowsAzureADJoin</span></span>|<span data-ttu-id="1a320-126">5</span><span class="sxs-lookup"><span data-stu-id="1a320-126">5</span></span>|<span data-ttu-id="1a320-127">Windows Azure AD を 10 に参加します。</span><span class="sxs-lookup"><span data-stu-id="1a320-127">Windows 10 Azure AD Join.</span></span>|
|<span data-ttu-id="1a320-128">windowsBulkUserless</span><span class="sxs-lookup"><span data-stu-id="1a320-128">windowsBulkUserless</span></span>|<span data-ttu-id="1a320-129">6</span><span class="sxs-lookup"><span data-stu-id="1a320-129">6</span></span>|<span data-ttu-id="1a320-130">証明書で ICD を Windows 10 一括登録します。</span><span class="sxs-lookup"><span data-stu-id="1a320-130">Windows 10 Bulk enrollment through ICD with certificate.</span></span>|
|<span data-ttu-id="1a320-131">windowsAutoEnrollment</span><span class="sxs-lookup"><span data-stu-id="1a320-131">windowsAutoEnrollment</span></span>|<span data-ttu-id="1a320-132">7</span><span class="sxs-lookup"><span data-stu-id="1a320-132">7</span></span>|<span data-ttu-id="1a320-133">10 の Windows の自動登録します。</span><span class="sxs-lookup"><span data-stu-id="1a320-133">Windows 10 automatic enrollment.</span></span> <span data-ttu-id="1a320-134">(勤務先のアカウントを追加)</span><span class="sxs-lookup"><span data-stu-id="1a320-134">(Add work account)</span></span>|
|<span data-ttu-id="1a320-135">windowsBulkAzureDomainJoin</span><span class="sxs-lookup"><span data-stu-id="1a320-135">windowsBulkAzureDomainJoin</span></span>|<span data-ttu-id="1a320-136">8</span><span class="sxs-lookup"><span data-stu-id="1a320-136">8</span></span>|<span data-ttu-id="1a320-137">10 の windows Azure AD に参加を一括します。</span><span class="sxs-lookup"><span data-stu-id="1a320-137">Windows 10 bulk Azure AD Join.</span></span>|
|<span data-ttu-id="1a320-138">windowsCoManagement</span><span class="sxs-lookup"><span data-stu-id="1a320-138">windowsCoManagement</span></span>|<span data-ttu-id="1a320-139">9</span><span class="sxs-lookup"><span data-stu-id="1a320-139">9</span></span>|<span data-ttu-id="1a320-140">Windows 10 共同管理が自動操縦装置、またはグループ ポリシーによって発生します。</span><span class="sxs-lookup"><span data-stu-id="1a320-140">Windows 10 co-management triggered by AutoPilot or Group Policy.</span></span>|



