---
title: subjectAlternativeNameType 列挙型
description: サブジェクト代替名のオプションです。
ms.openlocfilehash: 385ee36111907dd2e48bc18a2efda9552eb61924
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067953"
---
# <a name="subjectalternativenametype-enum-type"></a><span data-ttu-id="e026a-103">subjectAlternativeNameType 列挙型</span><span class="sxs-lookup"><span data-stu-id="e026a-103">subjectAlternativeNameType enum type</span></span>

> <span data-ttu-id="e026a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e026a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e026a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e026a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e026a-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e026a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e026a-107">サブジェクト代替名のオプションです。</span><span class="sxs-lookup"><span data-stu-id="e026a-107">Subject Alternative Name Options.</span></span>
## <a name="members"></a><span data-ttu-id="e026a-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="e026a-108">Members</span></span>
|<span data-ttu-id="e026a-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="e026a-109">Member</span></span>|<span data-ttu-id="e026a-110">値</span><span class="sxs-lookup"><span data-stu-id="e026a-110">Value</span></span>|<span data-ttu-id="e026a-111">説明</span><span class="sxs-lookup"><span data-stu-id="e026a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e026a-112">none</span><span class="sxs-lookup"><span data-stu-id="e026a-112">none</span></span>|<span data-ttu-id="e026a-113">0</span><span class="sxs-lookup"><span data-stu-id="e026a-113">0</span></span>|<span data-ttu-id="e026a-114">サブジェクト代替名がありません。</span><span class="sxs-lookup"><span data-stu-id="e026a-114">No subject alternative name.</span></span>|
|<span data-ttu-id="e026a-115">emailAddress</span><span class="sxs-lookup"><span data-stu-id="e026a-115">emailAddress</span></span>|<span data-ttu-id="e026a-116">1</span><span class="sxs-lookup"><span data-stu-id="e026a-116">1</span></span>|<span data-ttu-id="e026a-117">電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="e026a-117">Email address.</span></span>|
|<span data-ttu-id="e026a-118">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e026a-118">userPrincipalName</span></span>|<span data-ttu-id="e026a-119">2</span><span class="sxs-lookup"><span data-stu-id="e026a-119">2</span></span>|<span data-ttu-id="e026a-120">ユーザー プリンシパル名 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="e026a-120">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="e026a-121">customAzureADAttribute</span><span class="sxs-lookup"><span data-stu-id="e026a-121">customAzureADAttribute</span></span>|<span data-ttu-id="e026a-122">4</span><span class="sxs-lookup"><span data-stu-id="e026a-122">4</span></span>|<span data-ttu-id="e026a-123">Azure の AD 属性をカスタムします。</span><span class="sxs-lookup"><span data-stu-id="e026a-123">Custom Azure AD Attribute.</span></span>|
|<span data-ttu-id="e026a-124">domainNameService</span><span class="sxs-lookup"><span data-stu-id="e026a-124">domainNameService</span></span>|<span data-ttu-id="e026a-125">8</span><span class="sxs-lookup"><span data-stu-id="e026a-125">8</span></span>|<span data-ttu-id="e026a-126">ドメイン ネーム サービス (DNS)。</span><span class="sxs-lookup"><span data-stu-id="e026a-126">Domain Name Service (DNS).</span></span>|





