---
title: localSecurityOptionsAdministratorElevationPromptBehaviorType 列挙型
description: LocalSecurityOptionsAdministratorElevationPromptBehavior に指定できる値
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 597b49f65027ae2d01cbfddf741ff8ca08f83eb2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32460528"
---
# <a name="localsecurityoptionsadministratorelevationpromptbehaviortype-enum-type"></a><span data-ttu-id="d1ac2-103">localSecurityOptionsAdministratorElevationPromptBehaviorType 列挙型</span><span class="sxs-lookup"><span data-stu-id="d1ac2-103">localSecurityOptionsAdministratorElevationPromptBehaviorType enum type</span></span>

> <span data-ttu-id="d1ac2-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d1ac2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d1ac2-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d1ac2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1ac2-106">LocalSecurityOptionsAdministratorElevationPromptBehavior に指定できる値</span><span class="sxs-lookup"><span data-stu-id="d1ac2-106">Possible values for LocalSecurityOptionsAdministratorElevationPromptBehavior</span></span>

## <a name="members"></a><span data-ttu-id="d1ac2-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="d1ac2-107">Members</span></span>
|<span data-ttu-id="d1ac2-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="d1ac2-108">Member</span></span>|<span data-ttu-id="d1ac2-109">値</span><span class="sxs-lookup"><span data-stu-id="d1ac2-109">Value</span></span>|<span data-ttu-id="d1ac2-110">説明</span><span class="sxs-lookup"><span data-stu-id="d1ac2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1ac2-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="d1ac2-111">notConfigured</span></span>|<span data-ttu-id="d1ac2-112">.0</span><span class="sxs-lookup"><span data-stu-id="d1ac2-112">0</span></span>|<span data-ttu-id="d1ac2-113">Not Configured</span><span class="sxs-lookup"><span data-stu-id="d1ac2-113">Not Configured</span></span>|
|<span data-ttu-id="d1ac2-114">elevateWithoutPrompting</span><span class="sxs-lookup"><span data-stu-id="d1ac2-114">elevateWithoutPrompting</span></span>|<span data-ttu-id="d1ac2-115">1-d</span><span class="sxs-lookup"><span data-stu-id="d1ac2-115">1</span></span>|<span data-ttu-id="d1ac2-116">メッセージを表示せずに昇格します。</span><span class="sxs-lookup"><span data-stu-id="d1ac2-116">Elevate without prompting.</span></span>|
|<span data-ttu-id="d1ac2-117">promptForCredentialsOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="d1ac2-117">promptForCredentialsOnTheSecureDesktop</span></span>|<span data-ttu-id="d1ac2-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="d1ac2-118">2</span></span>|<span data-ttu-id="d1ac2-119">セキュリティで保護されたデスクトップで資格情報の入力を求める</span><span class="sxs-lookup"><span data-stu-id="d1ac2-119">Prompt for credentials on the secure desktop</span></span>|
|<span data-ttu-id="d1ac2-120">promptForConsentOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="d1ac2-120">promptForConsentOnTheSecureDesktop</span></span>|<span data-ttu-id="d1ac2-121">1/3</span><span class="sxs-lookup"><span data-stu-id="d1ac2-121">3</span></span>|<span data-ttu-id="d1ac2-122">セキュリティで保護されたデスクトップで同意を求める</span><span class="sxs-lookup"><span data-stu-id="d1ac2-122">Prompt for consent on the secure desktop</span></span>|
|<span data-ttu-id="d1ac2-123">promptforcredentials</span><span class="sxs-lookup"><span data-stu-id="d1ac2-123">promptForCredentials</span></span>|<span data-ttu-id="d1ac2-124">2/4</span><span class="sxs-lookup"><span data-stu-id="d1ac2-124">4</span></span>|<span data-ttu-id="d1ac2-125">資格情報の入力を求める</span><span class="sxs-lookup"><span data-stu-id="d1ac2-125">Prompt for credentials</span></span>|
|<span data-ttu-id="d1ac2-126">promptforconsent</span><span class="sxs-lookup"><span data-stu-id="d1ac2-126">promptForConsent</span></span>|<span data-ttu-id="d1ac2-127">5</span><span class="sxs-lookup"><span data-stu-id="d1ac2-127">5</span></span>|<span data-ttu-id="d1ac2-128">同意を求めるメッセージ</span><span class="sxs-lookup"><span data-stu-id="d1ac2-128">Prompt for consent</span></span>|
|<span data-ttu-id="d1ac2-129">promptforconfornonwindowsバイナリー</span><span class="sxs-lookup"><span data-stu-id="d1ac2-129">promptForConsentForNonWindowsBinaries</span></span>|<span data-ttu-id="d1ac2-130">シックス</span><span class="sxs-lookup"><span data-stu-id="d1ac2-130">6</span></span>|<span data-ttu-id="d1ac2-131">Windows 以外のバイナリの同意を求める</span><span class="sxs-lookup"><span data-stu-id="d1ac2-131">Prompt for consent for non-Windows binaries</span></span>|





