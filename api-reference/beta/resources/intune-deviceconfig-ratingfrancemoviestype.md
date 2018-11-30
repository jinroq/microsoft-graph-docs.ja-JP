---
title: ratingFranceMoviesType 列挙型
description: 映画がフランスでのラベルの評価
ms.openlocfilehash: 21f93bd34c093a993480491bafbca063ed8d540f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066954"
---
# <a name="ratingfrancemoviestype-enum-type"></a><span data-ttu-id="f531c-103">ratingFranceMoviesType 列挙型</span><span class="sxs-lookup"><span data-stu-id="f531c-103">ratingFranceMoviesType enum type</span></span>

> <span data-ttu-id="f531c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f531c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f531c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f531c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f531c-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f531c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f531c-107">映画がフランスでのラベルの評価</span><span class="sxs-lookup"><span data-stu-id="f531c-107">Movies rating labels in France</span></span>
## <a name="members"></a><span data-ttu-id="f531c-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="f531c-108">Members</span></span>
|<span data-ttu-id="f531c-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="f531c-109">Member</span></span>|<span data-ttu-id="f531c-110">値</span><span class="sxs-lookup"><span data-stu-id="f531c-110">Value</span></span>|<span data-ttu-id="f531c-111">説明</span><span class="sxs-lookup"><span data-stu-id="f531c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f531c-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="f531c-112">allAllowed</span></span>|<span data-ttu-id="f531c-113">0</span><span class="sxs-lookup"><span data-stu-id="f531c-113">0</span></span>|<span data-ttu-id="f531c-114">既定値、映画のすべてのコンテンツを許可します。</span><span class="sxs-lookup"><span data-stu-id="f531c-114">Default value, allow all movies content</span></span>|
|<span data-ttu-id="f531c-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="f531c-115">allBlocked</span></span>|<span data-ttu-id="f531c-116">1</span><span class="sxs-lookup"><span data-stu-id="f531c-116">1</span></span>|<span data-ttu-id="f531c-117">ビデオ コンテンツを許可しません。</span><span class="sxs-lookup"><span data-stu-id="f531c-117">Do not allow any movies content</span></span>|
|<span data-ttu-id="f531c-118">agesAbove10</span><span class="sxs-lookup"><span data-stu-id="f531c-118">agesAbove10</span></span>|<span data-ttu-id="f531c-119">2</span><span class="sxs-lookup"><span data-stu-id="f531c-119">2</span></span>|<span data-ttu-id="f531c-120">10 の分類には、10 未満の未成年にフィルムのスクリーニングが禁止されています。</span><span class="sxs-lookup"><span data-stu-id="f531c-120">The 10 classification prohibits the screening of the film to minors under 10</span></span>|
|<span data-ttu-id="f531c-121">agesAbove12</span><span class="sxs-lookup"><span data-stu-id="f531c-121">agesAbove12</span></span>|<span data-ttu-id="f531c-122">3</span><span class="sxs-lookup"><span data-stu-id="f531c-122">3</span></span>|<span data-ttu-id="f531c-123">12 の分類には、未成年で 12 のフィルムのスクリーニングが禁止されています。</span><span class="sxs-lookup"><span data-stu-id="f531c-123">The 12 classification prohibits the screening of the film to minors under 12</span></span>|
|<span data-ttu-id="f531c-124">agesAbove16</span><span class="sxs-lookup"><span data-stu-id="f531c-124">agesAbove16</span></span>|<span data-ttu-id="f531c-125">4</span><span class="sxs-lookup"><span data-stu-id="f531c-125">4</span></span>|<span data-ttu-id="f531c-126">16 の分類には、未成年の 16 のフィルムのスクリーニングが禁止されています。</span><span class="sxs-lookup"><span data-stu-id="f531c-126">The 16 classification prohibits the screening of the film to minors under 16</span></span>|
|<span data-ttu-id="f531c-127">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="f531c-127">agesAbove18</span></span>|<span data-ttu-id="f531c-128">5</span><span class="sxs-lookup"><span data-stu-id="f531c-128">5</span></span>|<span data-ttu-id="f531c-129">18 の分類には、18 才未満の未成年に審査が禁止されています。</span><span class="sxs-lookup"><span data-stu-id="f531c-129">The 18 classification prohibits the screening to minors under 18</span></span>|





