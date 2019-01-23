---
title: localSecurityOptionsAdministratorElevationPromptBehaviorType 列挙型
description: LocalSecurityOptionsAdministratorElevationPromptBehavior に指定できる値
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 978436bca4ac0ca281fde61e046e854ba3725c73
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413760"
---
# <a name="localsecurityoptionsadministratorelevationpromptbehaviortype-enum-type"></a><span data-ttu-id="0b731-103">localSecurityOptionsAdministratorElevationPromptBehaviorType 列挙型</span><span class="sxs-lookup"><span data-stu-id="0b731-103">localSecurityOptionsAdministratorElevationPromptBehaviorType enum type</span></span>

> <span data-ttu-id="0b731-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0b731-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0b731-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0b731-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0b731-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0b731-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b731-107">LocalSecurityOptionsAdministratorElevationPromptBehavior に指定できる値</span><span class="sxs-lookup"><span data-stu-id="0b731-107">Possible values for LocalSecurityOptionsAdministratorElevationPromptBehavior</span></span>

## <a name="members"></a><span data-ttu-id="0b731-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="0b731-108">Members</span></span>
|<span data-ttu-id="0b731-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="0b731-109">Member</span></span>|<span data-ttu-id="0b731-110">値</span><span class="sxs-lookup"><span data-stu-id="0b731-110">Value</span></span>|<span data-ttu-id="0b731-111">説明</span><span class="sxs-lookup"><span data-stu-id="0b731-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b731-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="0b731-112">notConfigured</span></span>|<span data-ttu-id="0b731-113">0</span><span class="sxs-lookup"><span data-stu-id="0b731-113">0</span></span>|<span data-ttu-id="0b731-114">構成されていません</span><span class="sxs-lookup"><span data-stu-id="0b731-114">Not Configured</span></span>|
|<span data-ttu-id="0b731-115">elevateWithoutPrompting</span><span class="sxs-lookup"><span data-stu-id="0b731-115">elevateWithoutPrompting</span></span>|<span data-ttu-id="0b731-116">1</span><span class="sxs-lookup"><span data-stu-id="0b731-116">1</span></span>|<span data-ttu-id="0b731-117">メッセージを表示せずに昇格します。</span><span class="sxs-lookup"><span data-stu-id="0b731-117">Elevate without prompting.</span></span>|
|<span data-ttu-id="0b731-118">promptForCredentialsOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="0b731-118">promptForCredentialsOnTheSecureDesktop</span></span>|<span data-ttu-id="0b731-119">2</span><span class="sxs-lookup"><span data-stu-id="0b731-119">2</span></span>|<span data-ttu-id="0b731-120">セキュリティで保護されたデスクトップで資格情報の入力を求める</span><span class="sxs-lookup"><span data-stu-id="0b731-120">Prompt for credentials on the secure desktop</span></span>|
|<span data-ttu-id="0b731-121">promptForConsentOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="0b731-121">promptForConsentOnTheSecureDesktop</span></span>|<span data-ttu-id="0b731-122">3</span><span class="sxs-lookup"><span data-stu-id="0b731-122">3</span></span>|<span data-ttu-id="0b731-123">セキュリティで保護されたデスクトップで同意を求める</span><span class="sxs-lookup"><span data-stu-id="0b731-123">Prompt for consent on the secure desktop</span></span>|
|<span data-ttu-id="0b731-124">promptForCredentials</span><span class="sxs-lookup"><span data-stu-id="0b731-124">promptForCredentials</span></span>|<span data-ttu-id="0b731-125">4</span><span class="sxs-lookup"><span data-stu-id="0b731-125">4</span></span>|<span data-ttu-id="0b731-126">資格情報の入力を求める</span><span class="sxs-lookup"><span data-stu-id="0b731-126">Prompt for credentials</span></span>|
|<span data-ttu-id="0b731-127">promptForConsent</span><span class="sxs-lookup"><span data-stu-id="0b731-127">promptForConsent</span></span>|<span data-ttu-id="0b731-128">5</span><span class="sxs-lookup"><span data-stu-id="0b731-128">5</span></span>|<span data-ttu-id="0b731-129">同意を求める</span><span class="sxs-lookup"><span data-stu-id="0b731-129">Prompt for consent</span></span>|
|<span data-ttu-id="0b731-130">promptForConsentForNonWindowsBinaries</span><span class="sxs-lookup"><span data-stu-id="0b731-130">promptForConsentForNonWindowsBinaries</span></span>|<span data-ttu-id="0b731-131">6</span><span class="sxs-lookup"><span data-stu-id="0b731-131">6</span></span>|<span data-ttu-id="0b731-132">Windows 以外のバイナリの同意を要求します。</span><span class="sxs-lookup"><span data-stu-id="0b731-132">Prompt for consent for non-Windows binaries</span></span>|




