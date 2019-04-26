---
title: ratingAustraliaMoviesType 列挙型
description: オーストラリアでの映画の定格ラベル
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3106197ce0efd3c0355461df58c5d22c314a08a6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32560803"
---
# <a name="ratingaustraliamoviestype-enum-type"></a><span data-ttu-id="d8ea9-103">ratingAustraliaMoviesType 列挙型</span><span class="sxs-lookup"><span data-stu-id="d8ea9-103">ratingAustraliaMoviesType enum type</span></span>

> <span data-ttu-id="d8ea9-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d8ea9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8ea9-105">オーストラリアでの映画の定格ラベル</span><span class="sxs-lookup"><span data-stu-id="d8ea9-105">Movies rating labels in Australia</span></span>

## <a name="members"></a><span data-ttu-id="d8ea9-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="d8ea9-106">Members</span></span>
|<span data-ttu-id="d8ea9-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="d8ea9-107">Member</span></span>|<span data-ttu-id="d8ea9-108">値</span><span class="sxs-lookup"><span data-stu-id="d8ea9-108">Value</span></span>|<span data-ttu-id="d8ea9-109">説明</span><span class="sxs-lookup"><span data-stu-id="d8ea9-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8ea9-110">allallowed</span><span class="sxs-lookup"><span data-stu-id="d8ea9-110">allAllowed</span></span>|<span data-ttu-id="d8ea9-111">.0</span><span class="sxs-lookup"><span data-stu-id="d8ea9-111">0</span></span>|<span data-ttu-id="d8ea9-112">既定値。すべてのムービーコンテンツを許可する</span><span class="sxs-lookup"><span data-stu-id="d8ea9-112">Default value, allow all movies content</span></span>|
|<span data-ttu-id="d8ea9-113">allblocked</span><span class="sxs-lookup"><span data-stu-id="d8ea9-113">allBlocked</span></span>|<span data-ttu-id="d8ea9-114">1 </span><span class="sxs-lookup"><span data-stu-id="d8ea9-114">1</span></span>|<span data-ttu-id="d8ea9-115">任意の映画コンテンツを許可しない</span><span class="sxs-lookup"><span data-stu-id="d8ea9-115">Do not allow any movies content</span></span>|
|<span data-ttu-id="d8ea9-116">元帳</span><span class="sxs-lookup"><span data-stu-id="d8ea9-116">general</span></span>|<span data-ttu-id="d8ea9-117">2 </span><span class="sxs-lookup"><span data-stu-id="d8ea9-117">2</span></span>|<span data-ttu-id="d8ea9-118">G 分類は、すべてのユーザーに適しています。</span><span class="sxs-lookup"><span data-stu-id="d8ea9-118">The G classification is suitable for everyone</span></span>|
|<span data-ttu-id="d8ea9-119">parentalguidance</span><span class="sxs-lookup"><span data-stu-id="d8ea9-119">parentalGuidance</span></span>|<span data-ttu-id="d8ea9-120">3 </span><span class="sxs-lookup"><span data-stu-id="d8ea9-120">3</span></span>|<span data-ttu-id="d8ea9-121">この PG は、親またはガーディアンからのガイダンスを含む15未満のビューアーを推奨します。</span><span class="sxs-lookup"><span data-stu-id="d8ea9-121">The PG recommends viewers under 15 with guidance from parents or guardians</span></span>|
|<span data-ttu-id="d8ea9-122">度</span><span class="sxs-lookup"><span data-stu-id="d8ea9-122">mature</span></span>|<span data-ttu-id="d8ea9-123">4 </span><span class="sxs-lookup"><span data-stu-id="d8ea9-123">4</span></span>|<span data-ttu-id="d8ea9-124">M 分類は15以下の閲覧者には推奨されません</span><span class="sxs-lookup"><span data-stu-id="d8ea9-124">The M classification is not recommended for viewers under 15</span></span>|
|<span data-ttu-id="d8ea9-125">agesAbove15</span><span class="sxs-lookup"><span data-stu-id="d8ea9-125">agesAbove15</span></span>|<span data-ttu-id="d8ea9-126">5 </span><span class="sxs-lookup"><span data-stu-id="d8ea9-126">5</span></span>|<span data-ttu-id="d8ea9-127">MA15 + 分類は15以下の閲覧者には適していません</span><span class="sxs-lookup"><span data-stu-id="d8ea9-127">The MA15+ classification is not suitable for viewers under 15</span></span>|
|<span data-ttu-id="d8ea9-128">agesAbove18</span><span class="sxs-lookup"><span data-stu-id="d8ea9-128">agesAbove18</span></span>|<span data-ttu-id="d8ea9-129">6 </span><span class="sxs-lookup"><span data-stu-id="d8ea9-129">6</span></span>|<span data-ttu-id="d8ea9-130">R18 + 分類が18の閲覧者には適していません</span><span class="sxs-lookup"><span data-stu-id="d8ea9-130">The R18+ classification is not suitable for viewers under 18</span></span>|



