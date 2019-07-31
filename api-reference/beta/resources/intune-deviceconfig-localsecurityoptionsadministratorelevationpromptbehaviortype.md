---
title: localSecurityOptionsAdministratorElevationPromptBehaviorType 列挙型
description: LocalSecurityOptionsAdministratorElevationPromptBehavior に指定できる値
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 397c8300a6acb2226a5f5dcccf630dde5d31bbc1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36000999"
---
# <a name="localsecurityoptionsadministratorelevationpromptbehaviortype-enum-type"></a><span data-ttu-id="9233b-103">localSecurityOptionsAdministratorElevationPromptBehaviorType 列挙型</span><span class="sxs-lookup"><span data-stu-id="9233b-103">localSecurityOptionsAdministratorElevationPromptBehaviorType enum type</span></span>

> <span data-ttu-id="9233b-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9233b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9233b-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9233b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9233b-106">LocalSecurityOptionsAdministratorElevationPromptBehavior に指定できる値</span><span class="sxs-lookup"><span data-stu-id="9233b-106">Possible values for LocalSecurityOptionsAdministratorElevationPromptBehavior</span></span>

## <a name="members"></a><span data-ttu-id="9233b-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="9233b-107">Members</span></span>
|<span data-ttu-id="9233b-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="9233b-108">Member</span></span>|<span data-ttu-id="9233b-109">値</span><span class="sxs-lookup"><span data-stu-id="9233b-109">Value</span></span>|<span data-ttu-id="9233b-110">説明</span><span class="sxs-lookup"><span data-stu-id="9233b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9233b-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="9233b-111">notConfigured</span></span>|<span data-ttu-id="9233b-112">.0</span><span class="sxs-lookup"><span data-stu-id="9233b-112">0</span></span>|<span data-ttu-id="9233b-113">Not Configured</span><span class="sxs-lookup"><span data-stu-id="9233b-113">Not Configured</span></span>|
|<span data-ttu-id="9233b-114">elevateWithoutPrompting</span><span class="sxs-lookup"><span data-stu-id="9233b-114">elevateWithoutPrompting</span></span>|<span data-ttu-id="9233b-115">1-d</span><span class="sxs-lookup"><span data-stu-id="9233b-115">1</span></span>|<span data-ttu-id="9233b-116">メッセージを表示せずに昇格します。</span><span class="sxs-lookup"><span data-stu-id="9233b-116">Elevate without prompting.</span></span>|
|<span data-ttu-id="9233b-117">promptForCredentialsOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="9233b-117">promptForCredentialsOnTheSecureDesktop</span></span>|<span data-ttu-id="9233b-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="9233b-118">2</span></span>|<span data-ttu-id="9233b-119">セキュリティで保護されたデスクトップで資格情報の入力を求める</span><span class="sxs-lookup"><span data-stu-id="9233b-119">Prompt for credentials on the secure desktop</span></span>|
|<span data-ttu-id="9233b-120">promptForConsentOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="9233b-120">promptForConsentOnTheSecureDesktop</span></span>|<span data-ttu-id="9233b-121">1/3</span><span class="sxs-lookup"><span data-stu-id="9233b-121">3</span></span>|<span data-ttu-id="9233b-122">セキュリティで保護されたデスクトップで同意を求める</span><span class="sxs-lookup"><span data-stu-id="9233b-122">Prompt for consent on the secure desktop</span></span>|
|<span data-ttu-id="9233b-123">promptForCredentials</span><span class="sxs-lookup"><span data-stu-id="9233b-123">promptForCredentials</span></span>|<span data-ttu-id="9233b-124">2/4</span><span class="sxs-lookup"><span data-stu-id="9233b-124">4</span></span>|<span data-ttu-id="9233b-125">資格情報の入力を求める</span><span class="sxs-lookup"><span data-stu-id="9233b-125">Prompt for credentials</span></span>|
|<span data-ttu-id="9233b-126">promptForConsent</span><span class="sxs-lookup"><span data-stu-id="9233b-126">promptForConsent</span></span>|<span data-ttu-id="9233b-127">5</span><span class="sxs-lookup"><span data-stu-id="9233b-127">5</span></span>|<span data-ttu-id="9233b-128">同意を求めるメッセージ</span><span class="sxs-lookup"><span data-stu-id="9233b-128">Prompt for consent</span></span>|
|<span data-ttu-id="9233b-129">Promptforconfornonwindowsバイナリー</span><span class="sxs-lookup"><span data-stu-id="9233b-129">promptForConsentForNonWindowsBinaries</span></span>|<span data-ttu-id="9233b-130">シックス</span><span class="sxs-lookup"><span data-stu-id="9233b-130">6</span></span>|<span data-ttu-id="9233b-131">Windows 以外のバイナリの同意を求める</span><span class="sxs-lookup"><span data-stu-id="9233b-131">Prompt for consent for non-Windows binaries</span></span>|





