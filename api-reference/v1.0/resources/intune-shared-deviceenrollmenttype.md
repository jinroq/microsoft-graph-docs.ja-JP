---
title: deviceEnrollmentType 列挙型
description: 管理するモバイル デバイスを追加するための方法です。
author: tfitzmac
ms.openlocfilehash: 88135947f882433a35fa518b750274f38f48dcc1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27329604"
---
# <a name="deviceenrollmenttype-enum-type"></a><span data-ttu-id="ad4a6-103">deviceEnrollmentType 列挙型</span><span class="sxs-lookup"><span data-stu-id="ad4a6-103">deviceEnrollmentType enum type</span></span>

> <span data-ttu-id="ad4a6-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ad4a6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ad4a6-105">管理するモバイル デバイスを追加するための方法です。</span><span class="sxs-lookup"><span data-stu-id="ad4a6-105">Possible ways of adding a mobile device to management.</span></span>

## <a name="members"></a><span data-ttu-id="ad4a6-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="ad4a6-106">Members</span></span>
|<span data-ttu-id="ad4a6-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="ad4a6-107">Member</span></span>|<span data-ttu-id="ad4a6-108">値</span><span class="sxs-lookup"><span data-stu-id="ad4a6-108">Value</span></span>|<span data-ttu-id="ad4a6-109">説明</span><span class="sxs-lookup"><span data-stu-id="ad4a6-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad4a6-110">不明</span><span class="sxs-lookup"><span data-stu-id="ad4a6-110">unknown</span></span>|<span data-ttu-id="ad4a6-111">0</span><span class="sxs-lookup"><span data-stu-id="ad4a6-111">0</span></span>|<span data-ttu-id="ad4a6-112">登録型の既定値は収集されませんでした。</span><span class="sxs-lookup"><span data-stu-id="ad4a6-112">Default value, enrollment type was not collected.</span></span>|
|<span data-ttu-id="ad4a6-113">userEnrollment</span><span class="sxs-lookup"><span data-stu-id="ad4a6-113">userEnrollment</span></span>|<span data-ttu-id="ad4a6-114">1</span><span class="sxs-lookup"><span data-stu-id="ad4a6-114">1</span></span>|<span data-ttu-id="ad4a6-115">BYOD チャネルを通じてユーザー駆動の登録します。</span><span class="sxs-lookup"><span data-stu-id="ad4a6-115">User driven enrollment through BYOD channel.</span></span>|
|<span data-ttu-id="ad4a6-116">deviceEnrollmentManager</span><span class="sxs-lookup"><span data-stu-id="ad4a6-116">deviceEnrollmentManager</span></span>|<span data-ttu-id="ad4a6-117">2</span><span class="sxs-lookup"><span data-stu-id="ad4a6-117">2</span></span>|<span data-ttu-id="ad4a6-118">デバイス登録の管理者アカウントとユーザー登録します。</span><span class="sxs-lookup"><span data-stu-id="ad4a6-118">User enrollment with a device enrollment manager account.</span></span>|
|<span data-ttu-id="ad4a6-119">appleBulkWithUser</span><span class="sxs-lookup"><span data-stu-id="ad4a6-119">appleBulkWithUser</span></span>|<span data-ttu-id="ad4a6-120">3</span><span class="sxs-lookup"><span data-stu-id="ad4a6-120">3</span></span>|<span data-ttu-id="ad4a6-121">アップル一括登録はユーザーのチャレンジ (DEP、Apple Configurator)。</span><span class="sxs-lookup"><span data-stu-id="ad4a6-121">Apple bulk enrollment with user challenge (DEP, Apple Configurator).</span></span>|
|<span data-ttu-id="ad4a6-122">appleBulkWithoutUser</span><span class="sxs-lookup"><span data-stu-id="ad4a6-122">appleBulkWithoutUser</span></span>|<span data-ttu-id="ad4a6-123">4</span><span class="sxs-lookup"><span data-stu-id="ad4a6-123">4</span></span>|<span data-ttu-id="ad4a6-124">ユーザーの課題 (DEP では、Apple の構成ウィザードは、モバイルの設定) にアップル一括登録します。</span><span class="sxs-lookup"><span data-stu-id="ad4a6-124">Apple bulk enrollment without user challenge (DEP, Apple Configurator, Mobile Config).</span></span>|
|<span data-ttu-id="ad4a6-125">windowsAzureADJoin</span><span class="sxs-lookup"><span data-stu-id="ad4a6-125">windowsAzureADJoin</span></span>|<span data-ttu-id="ad4a6-126">5</span><span class="sxs-lookup"><span data-stu-id="ad4a6-126">5</span></span>|<span data-ttu-id="ad4a6-127">Windows Azure AD を 10 に参加します。</span><span class="sxs-lookup"><span data-stu-id="ad4a6-127">Windows 10 Azure AD Join.</span></span>|
|<span data-ttu-id="ad4a6-128">windowsBulkUserless</span><span class="sxs-lookup"><span data-stu-id="ad4a6-128">windowsBulkUserless</span></span>|<span data-ttu-id="ad4a6-129">6</span><span class="sxs-lookup"><span data-stu-id="ad4a6-129">6</span></span>|<span data-ttu-id="ad4a6-130">証明書で ICD を Windows 10 一括登録します。</span><span class="sxs-lookup"><span data-stu-id="ad4a6-130">Windows 10 Bulk enrollment through ICD with certificate.</span></span>|
|<span data-ttu-id="ad4a6-131">windowsAutoEnrollment</span><span class="sxs-lookup"><span data-stu-id="ad4a6-131">windowsAutoEnrollment</span></span>|<span data-ttu-id="ad4a6-132">7</span><span class="sxs-lookup"><span data-stu-id="ad4a6-132">7</span></span>|<span data-ttu-id="ad4a6-133">10 の Windows の自動登録します。</span><span class="sxs-lookup"><span data-stu-id="ad4a6-133">Windows 10 automatic enrollment.</span></span> <span data-ttu-id="ad4a6-134">(勤務先のアカウントを追加)</span><span class="sxs-lookup"><span data-stu-id="ad4a6-134">(Add work account)</span></span>|
|<span data-ttu-id="ad4a6-135">windowsBulkAzureDomainJoin</span><span class="sxs-lookup"><span data-stu-id="ad4a6-135">windowsBulkAzureDomainJoin</span></span>|<span data-ttu-id="ad4a6-136">8</span><span class="sxs-lookup"><span data-stu-id="ad4a6-136">8</span></span>|<span data-ttu-id="ad4a6-137">10 の windows Azure AD に参加を一括します。</span><span class="sxs-lookup"><span data-stu-id="ad4a6-137">Windows 10 bulk Azure AD Join.</span></span>|
|<span data-ttu-id="ad4a6-138">windowsCoManagement</span><span class="sxs-lookup"><span data-stu-id="ad4a6-138">windowsCoManagement</span></span>|<span data-ttu-id="ad4a6-139">9</span><span class="sxs-lookup"><span data-stu-id="ad4a6-139">9</span></span>|<span data-ttu-id="ad4a6-140">Windows 10 共同管理が自動操縦装置、またはグループ ポリシーによって発生します。</span><span class="sxs-lookup"><span data-stu-id="ad4a6-140">Windows 10 co-management triggered by AutoPilot or Group Policy.</span></span>|



