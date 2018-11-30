---
title: ratingAppsType 列挙型
description: アプリケーションのメディア ・ コンテンツと評価
ms.openlocfilehash: 28ace3ba1e21a3f5f0901c926c6b633c8e96f041
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068532"
---
# <a name="ratingappstype-enum-type"></a><span data-ttu-id="979e1-103">ratingAppsType 列挙型</span><span class="sxs-lookup"><span data-stu-id="979e1-103">ratingAppsType enum type</span></span>

> <span data-ttu-id="979e1-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="979e1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="979e1-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="979e1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="979e1-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="979e1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="979e1-107">アプリケーションのメディア ・ コンテンツと評価</span><span class="sxs-lookup"><span data-stu-id="979e1-107">Apps rating as in media content</span></span>
## <a name="members"></a><span data-ttu-id="979e1-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="979e1-108">Members</span></span>
|<span data-ttu-id="979e1-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="979e1-109">Member</span></span>|<span data-ttu-id="979e1-110">値</span><span class="sxs-lookup"><span data-stu-id="979e1-110">Value</span></span>|<span data-ttu-id="979e1-111">説明</span><span class="sxs-lookup"><span data-stu-id="979e1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="979e1-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="979e1-112">allAllowed</span></span>|<span data-ttu-id="979e1-113">0</span><span class="sxs-lookup"><span data-stu-id="979e1-113">0</span></span>|<span data-ttu-id="979e1-114">既定値、アプリケーションのすべてのコンテンツを許可します。</span><span class="sxs-lookup"><span data-stu-id="979e1-114">Default value, allow all apps content</span></span>|
|<span data-ttu-id="979e1-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="979e1-115">allBlocked</span></span>|<span data-ttu-id="979e1-116">1</span><span class="sxs-lookup"><span data-stu-id="979e1-116">1</span></span>|<span data-ttu-id="979e1-117">任意のアプリケーションのコンテンツを許可しません。</span><span class="sxs-lookup"><span data-stu-id="979e1-117">Do not allow any apps content</span></span>|
|<span data-ttu-id="979e1-118">agesAbove4</span><span class="sxs-lookup"><span data-stu-id="979e1-118">agesAbove4</span></span>|<span data-ttu-id="979e1-119">2</span><span class="sxs-lookup"><span data-stu-id="979e1-119">2</span></span>|<span data-ttu-id="979e1-120">4 + では、神話の時代以降</span><span class="sxs-lookup"><span data-stu-id="979e1-120">4+, age 4 and above</span></span>|
|<span data-ttu-id="979e1-121">agesAbove9</span><span class="sxs-lookup"><span data-stu-id="979e1-121">agesAbove9</span></span>|<span data-ttu-id="979e1-122">3</span><span class="sxs-lookup"><span data-stu-id="979e1-122">3</span></span>|<span data-ttu-id="979e1-123">9 + 9 の時代以降</span><span class="sxs-lookup"><span data-stu-id="979e1-123">9+, age 9 and above</span></span>|
|<span data-ttu-id="979e1-124">agesAbove12</span><span class="sxs-lookup"><span data-stu-id="979e1-124">agesAbove12</span></span>|<span data-ttu-id="979e1-125">4</span><span class="sxs-lookup"><span data-stu-id="979e1-125">4</span></span>|<span data-ttu-id="979e1-126">12 + 12 の時代以降</span><span class="sxs-lookup"><span data-stu-id="979e1-126">12+, age 12 and above</span></span> |
|<span data-ttu-id="979e1-127">agesAbove17</span><span class="sxs-lookup"><span data-stu-id="979e1-127">agesAbove17</span></span>|<span data-ttu-id="979e1-128">5</span><span class="sxs-lookup"><span data-stu-id="979e1-128">5</span></span>|<span data-ttu-id="979e1-129">17 + 17 の時代以降</span><span class="sxs-lookup"><span data-stu-id="979e1-129">17+, age 17 and above</span></span>|





