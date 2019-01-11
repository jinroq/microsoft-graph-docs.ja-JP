---
title: subjectAlternativeNameType 列挙型
description: サブジェクト代替名のオプションです。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 914c4d577cc478e42e7982b9480bc8e43b8d88de
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869546"
---
# <a name="subjectalternativenametype-enum-type"></a><span data-ttu-id="29055-103">subjectAlternativeNameType 列挙型</span><span class="sxs-lookup"><span data-stu-id="29055-103">subjectAlternativeNameType enum type</span></span>

> <span data-ttu-id="29055-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="29055-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="29055-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="29055-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="29055-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="29055-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="29055-107">サブジェクト代替名のオプションです。</span><span class="sxs-lookup"><span data-stu-id="29055-107">Subject Alternative Name Options.</span></span>
## <a name="members"></a><span data-ttu-id="29055-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="29055-108">Members</span></span>
|<span data-ttu-id="29055-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="29055-109">Member</span></span>|<span data-ttu-id="29055-110">値</span><span class="sxs-lookup"><span data-stu-id="29055-110">Value</span></span>|<span data-ttu-id="29055-111">説明</span><span class="sxs-lookup"><span data-stu-id="29055-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29055-112">none</span><span class="sxs-lookup"><span data-stu-id="29055-112">none</span></span>|<span data-ttu-id="29055-113">0</span><span class="sxs-lookup"><span data-stu-id="29055-113">0</span></span>|<span data-ttu-id="29055-114">サブジェクト代替名がありません。</span><span class="sxs-lookup"><span data-stu-id="29055-114">No subject alternative name.</span></span>|
|<span data-ttu-id="29055-115">emailAddress</span><span class="sxs-lookup"><span data-stu-id="29055-115">emailAddress</span></span>|<span data-ttu-id="29055-116">1</span><span class="sxs-lookup"><span data-stu-id="29055-116">1</span></span>|<span data-ttu-id="29055-117">電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="29055-117">Email address.</span></span>|
|<span data-ttu-id="29055-118">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="29055-118">userPrincipalName</span></span>|<span data-ttu-id="29055-119">2</span><span class="sxs-lookup"><span data-stu-id="29055-119">2</span></span>|<span data-ttu-id="29055-120">ユーザー プリンシパル名 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="29055-120">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="29055-121">customAzureADAttribute</span><span class="sxs-lookup"><span data-stu-id="29055-121">customAzureADAttribute</span></span>|<span data-ttu-id="29055-122">4</span><span class="sxs-lookup"><span data-stu-id="29055-122">4</span></span>|<span data-ttu-id="29055-123">Azure の AD 属性をカスタムします。</span><span class="sxs-lookup"><span data-stu-id="29055-123">Custom Azure AD Attribute.</span></span>|
|<span data-ttu-id="29055-124">domainNameService</span><span class="sxs-lookup"><span data-stu-id="29055-124">domainNameService</span></span>|<span data-ttu-id="29055-125">8</span><span class="sxs-lookup"><span data-stu-id="29055-125">8</span></span>|<span data-ttu-id="29055-126">ドメイン ネーム サービス (DNS)。</span><span class="sxs-lookup"><span data-stu-id="29055-126">Domain Name Service (DNS).</span></span>|





