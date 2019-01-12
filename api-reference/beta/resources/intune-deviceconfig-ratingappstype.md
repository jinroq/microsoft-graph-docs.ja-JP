---
title: ratingAppsType 列挙型
description: アプリケーションのメディア ・ コンテンツと評価
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 709734a36010ded195a93b383adefc80f729c4fe
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953407"
---
# <a name="ratingappstype-enum-type"></a><span data-ttu-id="44e88-103">ratingAppsType 列挙型</span><span class="sxs-lookup"><span data-stu-id="44e88-103">ratingAppsType enum type</span></span>

> <span data-ttu-id="44e88-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="44e88-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="44e88-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="44e88-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="44e88-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="44e88-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="44e88-107">アプリケーションのメディア ・ コンテンツと評価</span><span class="sxs-lookup"><span data-stu-id="44e88-107">Apps rating as in media content</span></span>
## <a name="members"></a><span data-ttu-id="44e88-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="44e88-108">Members</span></span>
|<span data-ttu-id="44e88-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="44e88-109">Member</span></span>|<span data-ttu-id="44e88-110">値</span><span class="sxs-lookup"><span data-stu-id="44e88-110">Value</span></span>|<span data-ttu-id="44e88-111">説明</span><span class="sxs-lookup"><span data-stu-id="44e88-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44e88-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="44e88-112">allAllowed</span></span>|<span data-ttu-id="44e88-113">0</span><span class="sxs-lookup"><span data-stu-id="44e88-113">0</span></span>|<span data-ttu-id="44e88-114">既定値、アプリケーションのすべてのコンテンツを許可します。</span><span class="sxs-lookup"><span data-stu-id="44e88-114">Default value, allow all apps content</span></span>|
|<span data-ttu-id="44e88-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="44e88-115">allBlocked</span></span>|<span data-ttu-id="44e88-116">1</span><span class="sxs-lookup"><span data-stu-id="44e88-116">1</span></span>|<span data-ttu-id="44e88-117">任意のアプリケーションのコンテンツを許可しません。</span><span class="sxs-lookup"><span data-stu-id="44e88-117">Do not allow any apps content</span></span>|
|<span data-ttu-id="44e88-118">agesAbove4</span><span class="sxs-lookup"><span data-stu-id="44e88-118">agesAbove4</span></span>|<span data-ttu-id="44e88-119">2</span><span class="sxs-lookup"><span data-stu-id="44e88-119">2</span></span>|<span data-ttu-id="44e88-120">4 + では、神話の時代以降</span><span class="sxs-lookup"><span data-stu-id="44e88-120">4+, age 4 and above</span></span>|
|<span data-ttu-id="44e88-121">agesAbove9</span><span class="sxs-lookup"><span data-stu-id="44e88-121">agesAbove9</span></span>|<span data-ttu-id="44e88-122">3</span><span class="sxs-lookup"><span data-stu-id="44e88-122">3</span></span>|<span data-ttu-id="44e88-123">9 + 9 の時代以降</span><span class="sxs-lookup"><span data-stu-id="44e88-123">9+, age 9 and above</span></span>|
|<span data-ttu-id="44e88-124">agesAbove12</span><span class="sxs-lookup"><span data-stu-id="44e88-124">agesAbove12</span></span>|<span data-ttu-id="44e88-125">4</span><span class="sxs-lookup"><span data-stu-id="44e88-125">4</span></span>|<span data-ttu-id="44e88-126">12 + 12 の時代以降</span><span class="sxs-lookup"><span data-stu-id="44e88-126">12+, age 12 and above</span></span> |
|<span data-ttu-id="44e88-127">agesAbove17</span><span class="sxs-lookup"><span data-stu-id="44e88-127">agesAbove17</span></span>|<span data-ttu-id="44e88-128">5</span><span class="sxs-lookup"><span data-stu-id="44e88-128">5</span></span>|<span data-ttu-id="44e88-129">17 + 17 の時代以降</span><span class="sxs-lookup"><span data-stu-id="44e88-129">17+, age 17 and above</span></span>|





