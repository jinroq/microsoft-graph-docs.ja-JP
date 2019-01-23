---
title: webBrowserCookieSettings 列挙型
description: Web ブラウザーの Cookie の設定です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4a43577fa8db16016f47ed06b5deb1db37bfca39
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410806"
---
# <a name="webbrowsercookiesettings-enum-type"></a><span data-ttu-id="d0ea3-103">webBrowserCookieSettings 列挙型</span><span class="sxs-lookup"><span data-stu-id="d0ea3-103">webBrowserCookieSettings enum type</span></span>

> <span data-ttu-id="d0ea3-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d0ea3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d0ea3-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d0ea3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d0ea3-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d0ea3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0ea3-107">Web ブラウザーの Cookie の設定です。</span><span class="sxs-lookup"><span data-stu-id="d0ea3-107">Web Browser Cookie Settings.</span></span>

## <a name="members"></a><span data-ttu-id="d0ea3-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="d0ea3-108">Members</span></span>
|<span data-ttu-id="d0ea3-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="d0ea3-109">Member</span></span>|<span data-ttu-id="d0ea3-110">値</span><span class="sxs-lookup"><span data-stu-id="d0ea3-110">Value</span></span>|<span data-ttu-id="d0ea3-111">説明</span><span class="sxs-lookup"><span data-stu-id="d0ea3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0ea3-112">browserDefault</span><span class="sxs-lookup"><span data-stu-id="d0ea3-112">browserDefault</span></span>|<span data-ttu-id="d0ea3-113">0</span><span class="sxs-lookup"><span data-stu-id="d0ea3-113">0</span></span>|<span data-ttu-id="d0ea3-114">ブラウザーの既定値でことを目的しません。</span><span class="sxs-lookup"><span data-stu-id="d0ea3-114">Browser default value, no intent.</span></span>|
|<span data-ttu-id="d0ea3-115">blockAlways</span><span class="sxs-lookup"><span data-stu-id="d0ea3-115">blockAlways</span></span>|<span data-ttu-id="d0ea3-116">1</span><span class="sxs-lookup"><span data-stu-id="d0ea3-116">1</span></span>|<span data-ttu-id="d0ea3-117">常に cookie をブロックします。</span><span class="sxs-lookup"><span data-stu-id="d0ea3-117">Always block cookies.</span></span>|
|<span data-ttu-id="d0ea3-118">allowCurrentWebSite</span><span class="sxs-lookup"><span data-stu-id="d0ea3-118">allowCurrentWebSite</span></span>|<span data-ttu-id="d0ea3-119">2</span><span class="sxs-lookup"><span data-stu-id="d0ea3-119">2</span></span>|<span data-ttu-id="d0ea3-120">現在の Web サイトからの cookie を許可します。</span><span class="sxs-lookup"><span data-stu-id="d0ea3-120">Allow cookies from current Web site.</span></span>|
|<span data-ttu-id="d0ea3-121">allowFromWebsitesVisited</span><span class="sxs-lookup"><span data-stu-id="d0ea3-121">allowFromWebsitesVisited</span></span>|<span data-ttu-id="d0ea3-122">3</span><span class="sxs-lookup"><span data-stu-id="d0ea3-122">3</span></span>|<span data-ttu-id="d0ea3-123">訪問した web サイトからの Cookie を許可します。</span><span class="sxs-lookup"><span data-stu-id="d0ea3-123">Allow Cookies from websites visited.</span></span>|
|<span data-ttu-id="d0ea3-124">allowAlways</span><span class="sxs-lookup"><span data-stu-id="d0ea3-124">allowAlways</span></span>|<span data-ttu-id="d0ea3-125">4</span><span class="sxs-lookup"><span data-stu-id="d0ea3-125">4</span></span>|<span data-ttu-id="d0ea3-126">常に cookie を許可します。</span><span class="sxs-lookup"><span data-stu-id="d0ea3-126">Always allow cookies.</span></span>|




