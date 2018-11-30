---
title: localSecurityOptionsStandardUserElevationPromptBehaviorType 列挙型
description: LocalSecurityOptionsStandardUserElevationPromptBehavior に指定できる値
ms.openlocfilehash: 96be8f96bf78c9af8d7a71b511a69df64270115b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070311"
---
# <a name="localsecurityoptionsstandarduserelevationpromptbehaviortype-enum-type"></a><span data-ttu-id="c153a-103">localSecurityOptionsStandardUserElevationPromptBehaviorType 列挙型</span><span class="sxs-lookup"><span data-stu-id="c153a-103">localSecurityOptionsStandardUserElevationPromptBehaviorType enum type</span></span>

> <span data-ttu-id="c153a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c153a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c153a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c153a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c153a-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c153a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c153a-107">LocalSecurityOptionsStandardUserElevationPromptBehavior に指定できる値</span><span class="sxs-lookup"><span data-stu-id="c153a-107">Possible values for LocalSecurityOptionsStandardUserElevationPromptBehavior</span></span>
## <a name="members"></a><span data-ttu-id="c153a-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="c153a-108">Members</span></span>
|<span data-ttu-id="c153a-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="c153a-109">Member</span></span>|<span data-ttu-id="c153a-110">値</span><span class="sxs-lookup"><span data-stu-id="c153a-110">Value</span></span>|<span data-ttu-id="c153a-111">説明</span><span class="sxs-lookup"><span data-stu-id="c153a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c153a-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="c153a-112">notConfigured</span></span>|<span data-ttu-id="c153a-113">0</span><span class="sxs-lookup"><span data-stu-id="c153a-113">0</span></span>|<span data-ttu-id="c153a-114">構成されていません</span><span class="sxs-lookup"><span data-stu-id="c153a-114">Not Configured</span></span>|
|<span data-ttu-id="c153a-115">automaticallyDenyElevationRequests</span><span class="sxs-lookup"><span data-stu-id="c153a-115">automaticallyDenyElevationRequests</span></span>|<span data-ttu-id="c153a-116">1</span><span class="sxs-lookup"><span data-stu-id="c153a-116">1</span></span>|<span data-ttu-id="c153a-117">昇格の要求を自動的に拒否します。</span><span class="sxs-lookup"><span data-stu-id="c153a-117">Automatically deny elevation requests</span></span>|
|<span data-ttu-id="c153a-118">promptForCredentialsOnTheSecureDesktop</span><span class="sxs-lookup"><span data-stu-id="c153a-118">promptForCredentialsOnTheSecureDesktop</span></span>|<span data-ttu-id="c153a-119">2</span><span class="sxs-lookup"><span data-stu-id="c153a-119">2</span></span>|<span data-ttu-id="c153a-120">セキュリティで保護されたデスクトップで資格情報の入力を求める</span><span class="sxs-lookup"><span data-stu-id="c153a-120">Prompt for credentials on the secure desktop</span></span>|
|<span data-ttu-id="c153a-121">promptForCredentials</span><span class="sxs-lookup"><span data-stu-id="c153a-121">promptForCredentials</span></span>|<span data-ttu-id="c153a-122">3</span><span class="sxs-lookup"><span data-stu-id="c153a-122">3</span></span>|<span data-ttu-id="c153a-123">資格情報の入力を求める</span><span class="sxs-lookup"><span data-stu-id="c153a-123">Prompt for credentials</span></span>|





