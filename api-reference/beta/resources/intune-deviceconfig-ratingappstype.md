---
title: ratingAppsType 列挙型
description: アプリケーションのメディア ・ コンテンツと評価
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2b8abf9bd3c1c8e0a0fdf9fb4aaada295c22f5cb
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406564"
---
# <a name="ratingappstype-enum-type"></a><span data-ttu-id="61b51-103">ratingAppsType 列挙型</span><span class="sxs-lookup"><span data-stu-id="61b51-103">ratingAppsType enum type</span></span>

> <span data-ttu-id="61b51-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="61b51-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="61b51-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="61b51-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="61b51-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="61b51-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="61b51-107">アプリケーションのメディア ・ コンテンツと評価</span><span class="sxs-lookup"><span data-stu-id="61b51-107">Apps rating as in media content</span></span>

## <a name="members"></a><span data-ttu-id="61b51-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="61b51-108">Members</span></span>
|<span data-ttu-id="61b51-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="61b51-109">Member</span></span>|<span data-ttu-id="61b51-110">値</span><span class="sxs-lookup"><span data-stu-id="61b51-110">Value</span></span>|<span data-ttu-id="61b51-111">説明</span><span class="sxs-lookup"><span data-stu-id="61b51-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61b51-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="61b51-112">allAllowed</span></span>|<span data-ttu-id="61b51-113">0</span><span class="sxs-lookup"><span data-stu-id="61b51-113">0</span></span>|<span data-ttu-id="61b51-114">既定値、アプリケーションのすべてのコンテンツを許可します。</span><span class="sxs-lookup"><span data-stu-id="61b51-114">Default value, allow all apps content</span></span>|
|<span data-ttu-id="61b51-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="61b51-115">allBlocked</span></span>|<span data-ttu-id="61b51-116">1</span><span class="sxs-lookup"><span data-stu-id="61b51-116">1</span></span>|<span data-ttu-id="61b51-117">任意のアプリケーションのコンテンツを許可しません。</span><span class="sxs-lookup"><span data-stu-id="61b51-117">Do not allow any apps content</span></span>|
|<span data-ttu-id="61b51-118">agesAbove4</span><span class="sxs-lookup"><span data-stu-id="61b51-118">agesAbove4</span></span>|<span data-ttu-id="61b51-119">2</span><span class="sxs-lookup"><span data-stu-id="61b51-119">2</span></span>|<span data-ttu-id="61b51-120">4 + では、神話の時代以降</span><span class="sxs-lookup"><span data-stu-id="61b51-120">4+, age 4 and above</span></span>|
|<span data-ttu-id="61b51-121">agesAbove9</span><span class="sxs-lookup"><span data-stu-id="61b51-121">agesAbove9</span></span>|<span data-ttu-id="61b51-122">3</span><span class="sxs-lookup"><span data-stu-id="61b51-122">3</span></span>|<span data-ttu-id="61b51-123">9 + 9 の時代以降</span><span class="sxs-lookup"><span data-stu-id="61b51-123">9+, age 9 and above</span></span>|
|<span data-ttu-id="61b51-124">agesAbove12</span><span class="sxs-lookup"><span data-stu-id="61b51-124">agesAbove12</span></span>|<span data-ttu-id="61b51-125">4</span><span class="sxs-lookup"><span data-stu-id="61b51-125">4</span></span>|<span data-ttu-id="61b51-126">12 + 12 の時代以降</span><span class="sxs-lookup"><span data-stu-id="61b51-126">12+, age 12 and above</span></span> |
|<span data-ttu-id="61b51-127">agesAbove17</span><span class="sxs-lookup"><span data-stu-id="61b51-127">agesAbove17</span></span>|<span data-ttu-id="61b51-128">5</span><span class="sxs-lookup"><span data-stu-id="61b51-128">5</span></span>|<span data-ttu-id="61b51-129">17 + 17 の時代以降</span><span class="sxs-lookup"><span data-stu-id="61b51-129">17+, age 17 and above</span></span>|




