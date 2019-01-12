---
title: webBrowserCookieSettings 列挙型
description: Web ブラウザーの Cookie の設定です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 54fe38b9227c38f3af13ec242ece2d0bd6c144fa
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27927395"
---
# <a name="webbrowsercookiesettings-enum-type"></a><span data-ttu-id="3ee9c-103">webBrowserCookieSettings 列挙型</span><span class="sxs-lookup"><span data-stu-id="3ee9c-103">webBrowserCookieSettings enum type</span></span>

> <span data-ttu-id="3ee9c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3ee9c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3ee9c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3ee9c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3ee9c-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="3ee9c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3ee9c-107">Web ブラウザーの Cookie の設定です。</span><span class="sxs-lookup"><span data-stu-id="3ee9c-107">Web Browser Cookie Settings.</span></span>
## <a name="members"></a><span data-ttu-id="3ee9c-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="3ee9c-108">Members</span></span>
|<span data-ttu-id="3ee9c-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="3ee9c-109">Member</span></span>|<span data-ttu-id="3ee9c-110">値</span><span class="sxs-lookup"><span data-stu-id="3ee9c-110">Value</span></span>|<span data-ttu-id="3ee9c-111">説明</span><span class="sxs-lookup"><span data-stu-id="3ee9c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ee9c-112">browserDefault</span><span class="sxs-lookup"><span data-stu-id="3ee9c-112">browserDefault</span></span>|<span data-ttu-id="3ee9c-113">0</span><span class="sxs-lookup"><span data-stu-id="3ee9c-113">0</span></span>|<span data-ttu-id="3ee9c-114">ブラウザーの既定値でことを目的しません。</span><span class="sxs-lookup"><span data-stu-id="3ee9c-114">Browser default value, no intent.</span></span>|
|<span data-ttu-id="3ee9c-115">blockAlways</span><span class="sxs-lookup"><span data-stu-id="3ee9c-115">blockAlways</span></span>|<span data-ttu-id="3ee9c-116">1</span><span class="sxs-lookup"><span data-stu-id="3ee9c-116">1</span></span>|<span data-ttu-id="3ee9c-117">常に cookie をブロックします。</span><span class="sxs-lookup"><span data-stu-id="3ee9c-117">Always block cookies.</span></span>|
|<span data-ttu-id="3ee9c-118">allowCurrentWebSite</span><span class="sxs-lookup"><span data-stu-id="3ee9c-118">allowCurrentWebSite</span></span>|<span data-ttu-id="3ee9c-119">2</span><span class="sxs-lookup"><span data-stu-id="3ee9c-119">2</span></span>|<span data-ttu-id="3ee9c-120">現在の Web サイトからの cookie を許可します。</span><span class="sxs-lookup"><span data-stu-id="3ee9c-120">Allow cookies from current Web site.</span></span>|
|<span data-ttu-id="3ee9c-121">allowFromWebsitesVisited</span><span class="sxs-lookup"><span data-stu-id="3ee9c-121">allowFromWebsitesVisited</span></span>|<span data-ttu-id="3ee9c-122">3</span><span class="sxs-lookup"><span data-stu-id="3ee9c-122">3</span></span>|<span data-ttu-id="3ee9c-123">訪問した web サイトからの Cookie を許可します。</span><span class="sxs-lookup"><span data-stu-id="3ee9c-123">Allow Cookies from websites visited.</span></span>|
|<span data-ttu-id="3ee9c-124">allowAlways</span><span class="sxs-lookup"><span data-stu-id="3ee9c-124">allowAlways</span></span>|<span data-ttu-id="3ee9c-125">4</span><span class="sxs-lookup"><span data-stu-id="3ee9c-125">4</span></span>|<span data-ttu-id="3ee9c-126">常に cookie を許可します。</span><span class="sxs-lookup"><span data-stu-id="3ee9c-126">Always allow cookies.</span></span>|





