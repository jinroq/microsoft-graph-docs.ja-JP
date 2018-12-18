---
title: subjectAlternativeNameType 列挙型
description: サブジェクト代替名のオプションです。
author: tfitzmac
ms.openlocfilehash: 2c1249c90998a24eca63da7d80e580ac497aa9b8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326657"
---
# <a name="subjectalternativenametype-enum-type"></a><span data-ttu-id="304c9-103">subjectAlternativeNameType 列挙型</span><span class="sxs-lookup"><span data-stu-id="304c9-103">subjectAlternativeNameType enum type</span></span>

> <span data-ttu-id="304c9-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="304c9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="304c9-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="304c9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="304c9-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="304c9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="304c9-107">サブジェクト代替名のオプションです。</span><span class="sxs-lookup"><span data-stu-id="304c9-107">Subject Alternative Name Options.</span></span>
## <a name="members"></a><span data-ttu-id="304c9-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="304c9-108">Members</span></span>
|<span data-ttu-id="304c9-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="304c9-109">Member</span></span>|<span data-ttu-id="304c9-110">値</span><span class="sxs-lookup"><span data-stu-id="304c9-110">Value</span></span>|<span data-ttu-id="304c9-111">説明</span><span class="sxs-lookup"><span data-stu-id="304c9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="304c9-112">none</span><span class="sxs-lookup"><span data-stu-id="304c9-112">none</span></span>|<span data-ttu-id="304c9-113">0</span><span class="sxs-lookup"><span data-stu-id="304c9-113">0</span></span>|<span data-ttu-id="304c9-114">サブジェクト代替名がありません。</span><span class="sxs-lookup"><span data-stu-id="304c9-114">No subject alternative name.</span></span>|
|<span data-ttu-id="304c9-115">emailAddress</span><span class="sxs-lookup"><span data-stu-id="304c9-115">emailAddress</span></span>|<span data-ttu-id="304c9-116">1</span><span class="sxs-lookup"><span data-stu-id="304c9-116">1</span></span>|<span data-ttu-id="304c9-117">電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="304c9-117">Email address.</span></span>|
|<span data-ttu-id="304c9-118">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="304c9-118">userPrincipalName</span></span>|<span data-ttu-id="304c9-119">2</span><span class="sxs-lookup"><span data-stu-id="304c9-119">2</span></span>|<span data-ttu-id="304c9-120">ユーザー プリンシパル名 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="304c9-120">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="304c9-121">customAzureADAttribute</span><span class="sxs-lookup"><span data-stu-id="304c9-121">customAzureADAttribute</span></span>|<span data-ttu-id="304c9-122">4</span><span class="sxs-lookup"><span data-stu-id="304c9-122">4</span></span>|<span data-ttu-id="304c9-123">Azure の AD 属性をカスタムします。</span><span class="sxs-lookup"><span data-stu-id="304c9-123">Custom Azure AD Attribute.</span></span>|
|<span data-ttu-id="304c9-124">domainNameService</span><span class="sxs-lookup"><span data-stu-id="304c9-124">domainNameService</span></span>|<span data-ttu-id="304c9-125">8</span><span class="sxs-lookup"><span data-stu-id="304c9-125">8</span></span>|<span data-ttu-id="304c9-126">ドメイン ネーム サービス (DNS)。</span><span class="sxs-lookup"><span data-stu-id="304c9-126">Domain Name Service (DNS).</span></span>|





