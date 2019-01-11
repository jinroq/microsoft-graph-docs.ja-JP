---
title: localSecurityOptionsAdministratorElevationPromptBehaviorType 列挙型
description: LocalSecurityOptionsAdministratorElevationPromptBehavior に指定できる値
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 424c1193015d688019892d66ed07588358dcb8c2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870883"
---
# <a name="localsecurityoptionsadministratorelevationpromptbehaviortype-enum-type"></a><span data-ttu-id="56be1-103">localSecurityOptionsAdministratorElevationPromptBehaviorType 列挙型</span><span class="sxs-lookup"><span data-stu-id="56be1-103">localSecurityOptionsAdministratorElevationPromptBehaviorType enum type</span></span>

> <span data-ttu-id="56be1-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="56be1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="56be1-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="56be1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="56be1-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="56be1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="56be1-107">LocalSecurityOptionsAdministratorElevationPromptBehavior に指定できる値</span><span class="sxs-lookup"><span data-stu-id="56be1-107">Possible values for LocalSecurityOptionsAdministratorElevationPromptBehavior</span></span>
## <a name="members"></a><span data-ttu-id="56be1-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="56be1-108">Members</span></span>
|<span data-ttu-id="56be1-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="56be1-109">Member</span></span>|<span data-ttu-id="56be1-110">値</span><span class="sxs-lookup"><span data-stu-id="56be1-110">Value</span></span>|<span data-ttu-id="56be1-111">説明</span><span class="sxs-lookup"><span data-stu-id="56be1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56be1-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="56be1-112">notConfigured</span></span>|<span data-ttu-id="56be1-113">0</span><span class="sxs-lookup"><span data-stu-id="56be1-113">0</span></span>|<span data-ttu-id="56be1-114">構成されていません</span><span class="sxs-lookup"><span data-stu-id="56be1-114">Not Configured</span></span>|
|<span data-ttu-id="56be1-115">elevateWithoutPrompting</span><span class="sxs-lookup"><span data-stu-id="56be1-115">elevateWithoutPrompting</span></span>|<span data-ttu-id="56be1-116">1</span><span class="sxs-lookup"><span data-stu-id="56be1-116">1</span></span>|<span data-ttu-id="56be1-117">メッセージを表示せずに昇格します。</span><span class="sxs-lookup"><span data-stu-id="56be1-117">Elevate without prompting.</span></span>|
|<span data-ttu-id="56be1-118">promptForCredentialsOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="56be1-118">promptForCredentialsOnTheSecureDesktop</span></span>|<span data-ttu-id="56be1-119">2</span><span class="sxs-lookup"><span data-stu-id="56be1-119">2</span></span>|<span data-ttu-id="56be1-120">セキュリティで保護されたデスクトップで資格情報の入力を求める</span><span class="sxs-lookup"><span data-stu-id="56be1-120">Prompt for credentials on the secure desktop</span></span>|
|<span data-ttu-id="56be1-121">promptForConsentOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="56be1-121">promptForConsentOnTheSecureDesktop</span></span>|<span data-ttu-id="56be1-122">3</span><span class="sxs-lookup"><span data-stu-id="56be1-122">3</span></span>|<span data-ttu-id="56be1-123">セキュリティで保護されたデスクトップで同意を求める</span><span class="sxs-lookup"><span data-stu-id="56be1-123">Prompt for consent on the secure desktop</span></span>|
|<span data-ttu-id="56be1-124">promptForCredentials</span><span class="sxs-lookup"><span data-stu-id="56be1-124">promptForCredentials</span></span>|<span data-ttu-id="56be1-125">4</span><span class="sxs-lookup"><span data-stu-id="56be1-125">4</span></span>|<span data-ttu-id="56be1-126">資格情報の入力を求める</span><span class="sxs-lookup"><span data-stu-id="56be1-126">Prompt for credentials</span></span>|
|<span data-ttu-id="56be1-127">promptForConsent</span><span class="sxs-lookup"><span data-stu-id="56be1-127">promptForConsent</span></span>|<span data-ttu-id="56be1-128">5</span><span class="sxs-lookup"><span data-stu-id="56be1-128">5</span></span>|<span data-ttu-id="56be1-129">同意を求める</span><span class="sxs-lookup"><span data-stu-id="56be1-129">Prompt for consent</span></span>|
|<span data-ttu-id="56be1-130">promptForConsentForNonWindowsBinaries</span><span class="sxs-lookup"><span data-stu-id="56be1-130">promptForConsentForNonWindowsBinaries</span></span>|<span data-ttu-id="56be1-131">6</span><span class="sxs-lookup"><span data-stu-id="56be1-131">6</span></span>|<span data-ttu-id="56be1-132">Windows 以外のバイナリの同意を要求します。</span><span class="sxs-lookup"><span data-stu-id="56be1-132">Prompt for consent for non-Windows binaries</span></span>|





