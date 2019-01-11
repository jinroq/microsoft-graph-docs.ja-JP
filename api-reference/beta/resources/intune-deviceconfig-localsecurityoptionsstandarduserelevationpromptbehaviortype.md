---
title: localSecurityOptionsStandardUserElevationPromptBehaviorType 列挙型
description: LocalSecurityOptionsStandardUserElevationPromptBehavior に指定できる値
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 29b6e3d25450420eec63ff2d574dfc5c0f23fd8a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27877106"
---
# <a name="localsecurityoptionsstandarduserelevationpromptbehaviortype-enum-type"></a><span data-ttu-id="4758b-103">localSecurityOptionsStandardUserElevationPromptBehaviorType 列挙型</span><span class="sxs-lookup"><span data-stu-id="4758b-103">localSecurityOptionsStandardUserElevationPromptBehaviorType enum type</span></span>

> <span data-ttu-id="4758b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4758b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4758b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4758b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4758b-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4758b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4758b-107">LocalSecurityOptionsStandardUserElevationPromptBehavior に指定できる値</span><span class="sxs-lookup"><span data-stu-id="4758b-107">Possible values for LocalSecurityOptionsStandardUserElevationPromptBehavior</span></span>
## <a name="members"></a><span data-ttu-id="4758b-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="4758b-108">Members</span></span>
|<span data-ttu-id="4758b-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="4758b-109">Member</span></span>|<span data-ttu-id="4758b-110">値</span><span class="sxs-lookup"><span data-stu-id="4758b-110">Value</span></span>|<span data-ttu-id="4758b-111">説明</span><span class="sxs-lookup"><span data-stu-id="4758b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4758b-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="4758b-112">notConfigured</span></span>|<span data-ttu-id="4758b-113">0</span><span class="sxs-lookup"><span data-stu-id="4758b-113">0</span></span>|<span data-ttu-id="4758b-114">構成されていません</span><span class="sxs-lookup"><span data-stu-id="4758b-114">Not Configured</span></span>|
|<span data-ttu-id="4758b-115">automaticallyDenyElevationRequests</span><span class="sxs-lookup"><span data-stu-id="4758b-115">automaticallyDenyElevationRequests</span></span>|<span data-ttu-id="4758b-116">1</span><span class="sxs-lookup"><span data-stu-id="4758b-116">1</span></span>|<span data-ttu-id="4758b-117">昇格の要求を自動的に拒否します。</span><span class="sxs-lookup"><span data-stu-id="4758b-117">Automatically deny elevation requests</span></span>|
|<span data-ttu-id="4758b-118">promptForCredentialsOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="4758b-118">promptForCredentialsOnTheSecureDesktop</span></span>|<span data-ttu-id="4758b-119">2</span><span class="sxs-lookup"><span data-stu-id="4758b-119">2</span></span>|<span data-ttu-id="4758b-120">セキュリティで保護されたデスクトップで資格情報の入力を求める</span><span class="sxs-lookup"><span data-stu-id="4758b-120">Prompt for credentials on the secure desktop</span></span>|
|<span data-ttu-id="4758b-121">promptForCredentials</span><span class="sxs-lookup"><span data-stu-id="4758b-121">promptForCredentials</span></span>|<span data-ttu-id="4758b-122">3</span><span class="sxs-lookup"><span data-stu-id="4758b-122">3</span></span>|<span data-ttu-id="4758b-123">資格情報の入力を求める</span><span class="sxs-lookup"><span data-stu-id="4758b-123">Prompt for credentials</span></span>|





