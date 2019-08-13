---
title: ratingAustraliaMoviesType 列挙型
description: オーストラリアでの映画の定格ラベル
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 638c87c8ae9175f63efe7cb9e91db72ab11edd8a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36368374"
---
# <a name="ratingaustraliamoviestype-enum-type"></a><span data-ttu-id="dc929-103">ratingAustraliaMoviesType 列挙型</span><span class="sxs-lookup"><span data-stu-id="dc929-103">ratingAustraliaMoviesType enum type</span></span>

> <span data-ttu-id="dc929-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dc929-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dc929-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="dc929-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc929-106">オーストラリアでの映画の定格ラベル</span><span class="sxs-lookup"><span data-stu-id="dc929-106">Movies rating labels in Australia</span></span>

## <a name="members"></a><span data-ttu-id="dc929-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="dc929-107">Members</span></span>
|<span data-ttu-id="dc929-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="dc929-108">Member</span></span>|<span data-ttu-id="dc929-109">値</span><span class="sxs-lookup"><span data-stu-id="dc929-109">Value</span></span>|<span data-ttu-id="dc929-110">説明</span><span class="sxs-lookup"><span data-stu-id="dc929-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc929-111">allAllowed</span><span class="sxs-lookup"><span data-stu-id="dc929-111">allAllowed</span></span>|<span data-ttu-id="dc929-112">.0</span><span class="sxs-lookup"><span data-stu-id="dc929-112">0</span></span>|<span data-ttu-id="dc929-113">既定値。すべてのムービーコンテンツを許可する</span><span class="sxs-lookup"><span data-stu-id="dc929-113">Default value, allow all movies content</span></span>|
|<span data-ttu-id="dc929-114">allBlocked</span><span class="sxs-lookup"><span data-stu-id="dc929-114">allBlocked</span></span>|<span data-ttu-id="dc929-115">1-d</span><span class="sxs-lookup"><span data-stu-id="dc929-115">1</span></span>|<span data-ttu-id="dc929-116">任意の映画コンテンツを許可しない</span><span class="sxs-lookup"><span data-stu-id="dc929-116">Do not allow any movies content</span></span>|
|<span data-ttu-id="dc929-117">元帳</span><span class="sxs-lookup"><span data-stu-id="dc929-117">general</span></span>|<span data-ttu-id="dc929-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="dc929-118">2</span></span>|<span data-ttu-id="dc929-119">G 分類は、すべてのユーザーに適しています。</span><span class="sxs-lookup"><span data-stu-id="dc929-119">The G classification is suitable for everyone</span></span>|
|<span data-ttu-id="dc929-120">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="dc929-120">parentalGuidance</span></span>|<span data-ttu-id="dc929-121">1/3</span><span class="sxs-lookup"><span data-stu-id="dc929-121">3</span></span>|<span data-ttu-id="dc929-122">この PG は、親またはガーディアンからのガイダンスを含む15未満のビューアーを推奨します。</span><span class="sxs-lookup"><span data-stu-id="dc929-122">The PG recommends viewers under 15 with guidance from parents or guardians</span></span>|
|<span data-ttu-id="dc929-123">度</span><span class="sxs-lookup"><span data-stu-id="dc929-123">mature</span></span>|<span data-ttu-id="dc929-124">2/4</span><span class="sxs-lookup"><span data-stu-id="dc929-124">4</span></span>|<span data-ttu-id="dc929-125">M 分類は15以下の閲覧者には推奨されません</span><span class="sxs-lookup"><span data-stu-id="dc929-125">The M classification is not recommended for viewers under 15</span></span>|
|<span data-ttu-id="dc929-126">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="dc929-126">agesAbove15</span></span>|<span data-ttu-id="dc929-127">5</span><span class="sxs-lookup"><span data-stu-id="dc929-127">5</span></span>|<span data-ttu-id="dc929-128">MA15 + 分類は15以下の閲覧者には適していません</span><span class="sxs-lookup"><span data-stu-id="dc929-128">The MA15+ classification is not suitable for viewers under 15</span></span>|
|<span data-ttu-id="dc929-129">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="dc929-129">agesAbove18</span></span>|<span data-ttu-id="dc929-130">シックス</span><span class="sxs-lookup"><span data-stu-id="dc929-130">6</span></span>|<span data-ttu-id="dc929-131">R18 + 分類が18の閲覧者には適していません</span><span class="sxs-lookup"><span data-stu-id="dc929-131">The R18+ classification is not suitable for viewers under 18</span></span>|



