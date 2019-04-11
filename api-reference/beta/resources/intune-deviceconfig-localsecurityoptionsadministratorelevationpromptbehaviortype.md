---
title: localSecurityOptionsAdministratorElevationPromptBehaviorType 列挙型
description: LocalSecurityOptionsAdministratorElevationPromptBehavior に指定できる値
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 597b49f65027ae2d01cbfddf741ff8ca08f83eb2
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31796935"
---
# <a name="localsecurityoptionsadministratorelevationpromptbehaviortype-enum-type"></a><span data-ttu-id="e0fd5-103">localSecurityOptionsAdministratorElevationPromptBehaviorType 列挙型</span><span class="sxs-lookup"><span data-stu-id="e0fd5-103">localSecurityOptionsAdministratorElevationPromptBehaviorType enum type</span></span>

> <span data-ttu-id="e0fd5-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e0fd5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e0fd5-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e0fd5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e0fd5-106">LocalSecurityOptionsAdministratorElevationPromptBehavior に指定できる値</span><span class="sxs-lookup"><span data-stu-id="e0fd5-106">Possible values for LocalSecurityOptionsAdministratorElevationPromptBehavior</span></span>

## <a name="members"></a><span data-ttu-id="e0fd5-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="e0fd5-107">Members</span></span>
|<span data-ttu-id="e0fd5-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="e0fd5-108">Member</span></span>|<span data-ttu-id="e0fd5-109">値</span><span class="sxs-lookup"><span data-stu-id="e0fd5-109">Value</span></span>|<span data-ttu-id="e0fd5-110">説明</span><span class="sxs-lookup"><span data-stu-id="e0fd5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0fd5-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="e0fd5-111">notConfigured</span></span>|<span data-ttu-id="e0fd5-112">.0</span><span class="sxs-lookup"><span data-stu-id="e0fd5-112">0</span></span>|<span data-ttu-id="e0fd5-113">Not Configured</span><span class="sxs-lookup"><span data-stu-id="e0fd5-113">Not Configured</span></span>|
|<span data-ttu-id="e0fd5-114">elevateWithoutPrompting</span><span class="sxs-lookup"><span data-stu-id="e0fd5-114">elevateWithoutPrompting</span></span>|<span data-ttu-id="e0fd5-115">1-d</span><span class="sxs-lookup"><span data-stu-id="e0fd5-115">1</span></span>|<span data-ttu-id="e0fd5-116">メッセージを表示せずに昇格します。</span><span class="sxs-lookup"><span data-stu-id="e0fd5-116">Elevate without prompting.</span></span>|
|<span data-ttu-id="e0fd5-117">promptForCredentialsOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="e0fd5-117">promptForCredentialsOnTheSecureDesktop</span></span>|<span data-ttu-id="e0fd5-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="e0fd5-118">2</span></span>|<span data-ttu-id="e0fd5-119">セキュリティで保護されたデスクトップで資格情報の入力を求める</span><span class="sxs-lookup"><span data-stu-id="e0fd5-119">Prompt for credentials on the secure desktop</span></span>|
|<span data-ttu-id="e0fd5-120">promptForConsentOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="e0fd5-120">promptForConsentOnTheSecureDesktop</span></span>|<span data-ttu-id="e0fd5-121">1/3</span><span class="sxs-lookup"><span data-stu-id="e0fd5-121">3</span></span>|<span data-ttu-id="e0fd5-122">セキュリティで保護されたデスクトップで同意を求める</span><span class="sxs-lookup"><span data-stu-id="e0fd5-122">Prompt for consent on the secure desktop</span></span>|
|<span data-ttu-id="e0fd5-123">promptforcredentials</span><span class="sxs-lookup"><span data-stu-id="e0fd5-123">promptForCredentials</span></span>|<span data-ttu-id="e0fd5-124">2/4</span><span class="sxs-lookup"><span data-stu-id="e0fd5-124">4</span></span>|<span data-ttu-id="e0fd5-125">資格情報の入力を求める</span><span class="sxs-lookup"><span data-stu-id="e0fd5-125">Prompt for credentials</span></span>|
|<span data-ttu-id="e0fd5-126">promptforconsent</span><span class="sxs-lookup"><span data-stu-id="e0fd5-126">promptForConsent</span></span>|<span data-ttu-id="e0fd5-127">5</span><span class="sxs-lookup"><span data-stu-id="e0fd5-127">5</span></span>|<span data-ttu-id="e0fd5-128">同意を求めるメッセージ</span><span class="sxs-lookup"><span data-stu-id="e0fd5-128">Prompt for consent</span></span>|
|<span data-ttu-id="e0fd5-129">promptforconfornonwindowsバイナリー</span><span class="sxs-lookup"><span data-stu-id="e0fd5-129">promptForConsentForNonWindowsBinaries</span></span>|<span data-ttu-id="e0fd5-130">シックス</span><span class="sxs-lookup"><span data-stu-id="e0fd5-130">6</span></span>|<span data-ttu-id="e0fd5-131">Windows 以外のバイナリの同意を求める</span><span class="sxs-lookup"><span data-stu-id="e0fd5-131">Prompt for consent for non-Windows binaries</span></span>|





