---
title: localSecurityOptionsAdministratorElevationPromptBehaviorType 列挙型
description: LocalSecurityOptionsAdministratorElevationPromptBehavior に指定できる値
author: tfitzmac
ms.openlocfilehash: 620e2030433bd0f7a72263fa16907ec18c86f5f8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308751"
---
# <a name="localsecurityoptionsadministratorelevationpromptbehaviortype-enum-type"></a><span data-ttu-id="f2eeb-103">localSecurityOptionsAdministratorElevationPromptBehaviorType 列挙型</span><span class="sxs-lookup"><span data-stu-id="f2eeb-103">localSecurityOptionsAdministratorElevationPromptBehaviorType enum type</span></span>

> <span data-ttu-id="f2eeb-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f2eeb-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f2eeb-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f2eeb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f2eeb-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f2eeb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f2eeb-107">LocalSecurityOptionsAdministratorElevationPromptBehavior に指定できる値</span><span class="sxs-lookup"><span data-stu-id="f2eeb-107">Possible values for LocalSecurityOptionsAdministratorElevationPromptBehavior</span></span>
## <a name="members"></a><span data-ttu-id="f2eeb-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="f2eeb-108">Members</span></span>
|<span data-ttu-id="f2eeb-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="f2eeb-109">Member</span></span>|<span data-ttu-id="f2eeb-110">値</span><span class="sxs-lookup"><span data-stu-id="f2eeb-110">Value</span></span>|<span data-ttu-id="f2eeb-111">説明</span><span class="sxs-lookup"><span data-stu-id="f2eeb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2eeb-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="f2eeb-112">notConfigured</span></span>|<span data-ttu-id="f2eeb-113">0</span><span class="sxs-lookup"><span data-stu-id="f2eeb-113">0</span></span>|<span data-ttu-id="f2eeb-114">構成されていません</span><span class="sxs-lookup"><span data-stu-id="f2eeb-114">Not Configured</span></span>|
|<span data-ttu-id="f2eeb-115">elevateWithoutPrompting</span><span class="sxs-lookup"><span data-stu-id="f2eeb-115">elevateWithoutPrompting</span></span>|<span data-ttu-id="f2eeb-116">1</span><span class="sxs-lookup"><span data-stu-id="f2eeb-116">1</span></span>|<span data-ttu-id="f2eeb-117">メッセージを表示せずに昇格します。</span><span class="sxs-lookup"><span data-stu-id="f2eeb-117">Elevate without prompting.</span></span>|
|<span data-ttu-id="f2eeb-118">promptForCredentialsOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="f2eeb-118">promptForCredentialsOnTheSecureDesktop</span></span>|<span data-ttu-id="f2eeb-119">2</span><span class="sxs-lookup"><span data-stu-id="f2eeb-119">2</span></span>|<span data-ttu-id="f2eeb-120">セキュリティで保護されたデスクトップで資格情報の入力を求める</span><span class="sxs-lookup"><span data-stu-id="f2eeb-120">Prompt for credentials on the secure desktop</span></span>|
|<span data-ttu-id="f2eeb-121">promptForConsentOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="f2eeb-121">promptForConsentOnTheSecureDesktop</span></span>|<span data-ttu-id="f2eeb-122">3</span><span class="sxs-lookup"><span data-stu-id="f2eeb-122">3</span></span>|<span data-ttu-id="f2eeb-123">セキュリティで保護されたデスクトップで同意を求める</span><span class="sxs-lookup"><span data-stu-id="f2eeb-123">Prompt for consent on the secure desktop</span></span>|
|<span data-ttu-id="f2eeb-124">promptForCredentials</span><span class="sxs-lookup"><span data-stu-id="f2eeb-124">promptForCredentials</span></span>|<span data-ttu-id="f2eeb-125">4</span><span class="sxs-lookup"><span data-stu-id="f2eeb-125">4</span></span>|<span data-ttu-id="f2eeb-126">資格情報の入力を求める</span><span class="sxs-lookup"><span data-stu-id="f2eeb-126">Prompt for credentials</span></span>|
|<span data-ttu-id="f2eeb-127">promptForConsent</span><span class="sxs-lookup"><span data-stu-id="f2eeb-127">promptForConsent</span></span>|<span data-ttu-id="f2eeb-128">5</span><span class="sxs-lookup"><span data-stu-id="f2eeb-128">5</span></span>|<span data-ttu-id="f2eeb-129">同意を求める</span><span class="sxs-lookup"><span data-stu-id="f2eeb-129">Prompt for consent</span></span>|
|<span data-ttu-id="f2eeb-130">promptForConsentForNonWindowsBinaries</span><span class="sxs-lookup"><span data-stu-id="f2eeb-130">promptForConsentForNonWindowsBinaries</span></span>|<span data-ttu-id="f2eeb-131">6</span><span class="sxs-lookup"><span data-stu-id="f2eeb-131">6</span></span>|<span data-ttu-id="f2eeb-132">Windows 以外のバイナリの同意を要求します。</span><span class="sxs-lookup"><span data-stu-id="f2eeb-132">Prompt for consent for non-Windows binaries</span></span>|





