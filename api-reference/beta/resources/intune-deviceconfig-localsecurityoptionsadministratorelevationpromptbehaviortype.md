---
title: localSecurityOptionsAdministratorElevationPromptBehaviorType 列挙型
description: LocalSecurityOptionsAdministratorElevationPromptBehavior に指定できる値
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ae886f6c7696150cb85a17cb2caa65823705e121
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916825"
---
# <a name="localsecurityoptionsadministratorelevationpromptbehaviortype-enum-type"></a><span data-ttu-id="6cd95-103">localSecurityOptionsAdministratorElevationPromptBehaviorType 列挙型</span><span class="sxs-lookup"><span data-stu-id="6cd95-103">localSecurityOptionsAdministratorElevationPromptBehaviorType enum type</span></span>

> <span data-ttu-id="6cd95-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6cd95-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6cd95-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6cd95-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6cd95-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6cd95-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6cd95-107">LocalSecurityOptionsAdministratorElevationPromptBehavior に指定できる値</span><span class="sxs-lookup"><span data-stu-id="6cd95-107">Possible values for LocalSecurityOptionsAdministratorElevationPromptBehavior</span></span>
## <a name="members"></a><span data-ttu-id="6cd95-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="6cd95-108">Members</span></span>
|<span data-ttu-id="6cd95-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="6cd95-109">Member</span></span>|<span data-ttu-id="6cd95-110">値</span><span class="sxs-lookup"><span data-stu-id="6cd95-110">Value</span></span>|<span data-ttu-id="6cd95-111">説明</span><span class="sxs-lookup"><span data-stu-id="6cd95-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6cd95-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="6cd95-112">notConfigured</span></span>|<span data-ttu-id="6cd95-113">0</span><span class="sxs-lookup"><span data-stu-id="6cd95-113">0</span></span>|<span data-ttu-id="6cd95-114">構成されていません</span><span class="sxs-lookup"><span data-stu-id="6cd95-114">Not Configured</span></span>|
|<span data-ttu-id="6cd95-115">elevateWithoutPrompting</span><span class="sxs-lookup"><span data-stu-id="6cd95-115">elevateWithoutPrompting</span></span>|<span data-ttu-id="6cd95-116">1</span><span class="sxs-lookup"><span data-stu-id="6cd95-116">1</span></span>|<span data-ttu-id="6cd95-117">メッセージを表示せずに昇格します。</span><span class="sxs-lookup"><span data-stu-id="6cd95-117">Elevate without prompting.</span></span>|
|<span data-ttu-id="6cd95-118">promptForCredentialsOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="6cd95-118">promptForCredentialsOnTheSecureDesktop</span></span>|<span data-ttu-id="6cd95-119">2</span><span class="sxs-lookup"><span data-stu-id="6cd95-119">2</span></span>|<span data-ttu-id="6cd95-120">セキュリティで保護されたデスクトップで資格情報の入力を求める</span><span class="sxs-lookup"><span data-stu-id="6cd95-120">Prompt for credentials on the secure desktop</span></span>|
|<span data-ttu-id="6cd95-121">promptForConsentOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="6cd95-121">promptForConsentOnTheSecureDesktop</span></span>|<span data-ttu-id="6cd95-122">3</span><span class="sxs-lookup"><span data-stu-id="6cd95-122">3</span></span>|<span data-ttu-id="6cd95-123">セキュリティで保護されたデスクトップで同意を求める</span><span class="sxs-lookup"><span data-stu-id="6cd95-123">Prompt for consent on the secure desktop</span></span>|
|<span data-ttu-id="6cd95-124">promptForCredentials</span><span class="sxs-lookup"><span data-stu-id="6cd95-124">promptForCredentials</span></span>|<span data-ttu-id="6cd95-125">4</span><span class="sxs-lookup"><span data-stu-id="6cd95-125">4</span></span>|<span data-ttu-id="6cd95-126">資格情報の入力を求める</span><span class="sxs-lookup"><span data-stu-id="6cd95-126">Prompt for credentials</span></span>|
|<span data-ttu-id="6cd95-127">promptForConsent</span><span class="sxs-lookup"><span data-stu-id="6cd95-127">promptForConsent</span></span>|<span data-ttu-id="6cd95-128">5</span><span class="sxs-lookup"><span data-stu-id="6cd95-128">5</span></span>|<span data-ttu-id="6cd95-129">同意を求める</span><span class="sxs-lookup"><span data-stu-id="6cd95-129">Prompt for consent</span></span>|
|<span data-ttu-id="6cd95-130">promptForConsentForNonWindowsBinaries</span><span class="sxs-lookup"><span data-stu-id="6cd95-130">promptForConsentForNonWindowsBinaries</span></span>|<span data-ttu-id="6cd95-131">6</span><span class="sxs-lookup"><span data-stu-id="6cd95-131">6</span></span>|<span data-ttu-id="6cd95-132">Windows 以外のバイナリの同意を要求します。</span><span class="sxs-lookup"><span data-stu-id="6cd95-132">Prompt for consent for non-Windows binaries</span></span>|





