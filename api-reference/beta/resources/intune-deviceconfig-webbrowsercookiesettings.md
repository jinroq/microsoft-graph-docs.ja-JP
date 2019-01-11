---
title: webBrowserCookieSettings 列挙型
description: Web ブラウザーの Cookie の設定です。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 9b0ee6c860e3960ef719556f6db83a8e94d55d46
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889594"
---
# <a name="webbrowsercookiesettings-enum-type"></a><span data-ttu-id="b7215-103">webBrowserCookieSettings 列挙型</span><span class="sxs-lookup"><span data-stu-id="b7215-103">webBrowserCookieSettings enum type</span></span>

> <span data-ttu-id="b7215-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b7215-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b7215-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b7215-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b7215-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b7215-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b7215-107">Web ブラウザーの Cookie の設定です。</span><span class="sxs-lookup"><span data-stu-id="b7215-107">Web Browser Cookie Settings.</span></span>
## <a name="members"></a><span data-ttu-id="b7215-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="b7215-108">Members</span></span>
|<span data-ttu-id="b7215-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="b7215-109">Member</span></span>|<span data-ttu-id="b7215-110">値</span><span class="sxs-lookup"><span data-stu-id="b7215-110">Value</span></span>|<span data-ttu-id="b7215-111">説明</span><span class="sxs-lookup"><span data-stu-id="b7215-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7215-112">browserDefault</span><span class="sxs-lookup"><span data-stu-id="b7215-112">browserDefault</span></span>|<span data-ttu-id="b7215-113">0</span><span class="sxs-lookup"><span data-stu-id="b7215-113">0</span></span>|<span data-ttu-id="b7215-114">ブラウザーの既定値でことを目的しません。</span><span class="sxs-lookup"><span data-stu-id="b7215-114">Browser default value, no intent.</span></span>|
|<span data-ttu-id="b7215-115">blockAlways</span><span class="sxs-lookup"><span data-stu-id="b7215-115">blockAlways</span></span>|<span data-ttu-id="b7215-116">1</span><span class="sxs-lookup"><span data-stu-id="b7215-116">1</span></span>|<span data-ttu-id="b7215-117">常に cookie をブロックします。</span><span class="sxs-lookup"><span data-stu-id="b7215-117">Always block cookies.</span></span>|
|<span data-ttu-id="b7215-118">allowCurrentWebSite</span><span class="sxs-lookup"><span data-stu-id="b7215-118">allowCurrentWebSite</span></span>|<span data-ttu-id="b7215-119">2</span><span class="sxs-lookup"><span data-stu-id="b7215-119">2</span></span>|<span data-ttu-id="b7215-120">現在の Web サイトからの cookie を許可します。</span><span class="sxs-lookup"><span data-stu-id="b7215-120">Allow cookies from current Web site.</span></span>|
|<span data-ttu-id="b7215-121">allowFromWebsitesVisited</span><span class="sxs-lookup"><span data-stu-id="b7215-121">allowFromWebsitesVisited</span></span>|<span data-ttu-id="b7215-122">3</span><span class="sxs-lookup"><span data-stu-id="b7215-122">3</span></span>|<span data-ttu-id="b7215-123">訪問した web サイトからの Cookie を許可します。</span><span class="sxs-lookup"><span data-stu-id="b7215-123">Allow Cookies from websites visited.</span></span>|
|<span data-ttu-id="b7215-124">allowAlways</span><span class="sxs-lookup"><span data-stu-id="b7215-124">allowAlways</span></span>|<span data-ttu-id="b7215-125">4</span><span class="sxs-lookup"><span data-stu-id="b7215-125">4</span></span>|<span data-ttu-id="b7215-126">常に cookie を許可します。</span><span class="sxs-lookup"><span data-stu-id="b7215-126">Always allow cookies.</span></span>|





