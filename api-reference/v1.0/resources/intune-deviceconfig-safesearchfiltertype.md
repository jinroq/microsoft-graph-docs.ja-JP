---
title: safeSearchFilterType 列挙型
description: 安全な検索のレベル (アダルトコンテンツのフィルタリング) を指定します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c82f80f6081f57a88fcdf26f7639277d72b5e0d8
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250587"
---
# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="e170d-103">safeSearchFilterType 列挙型</span><span class="sxs-lookup"><span data-stu-id="e170d-103">safeSearchFilterType enum type</span></span>

> <span data-ttu-id="e170d-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e170d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e170d-105">安全な検索のレベル (アダルトコンテンツのフィルタリング) を指定します。</span><span class="sxs-lookup"><span data-stu-id="e170d-105">Specifies what level of safe search (filtering adult content) is required</span></span>

## <a name="members"></a><span data-ttu-id="e170d-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="e170d-106">Members</span></span>
|<span data-ttu-id="e170d-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="e170d-107">Member</span></span>|<span data-ttu-id="e170d-108">値</span><span class="sxs-lookup"><span data-stu-id="e170d-108">Value</span></span>|<span data-ttu-id="e170d-109">説明</span><span class="sxs-lookup"><span data-stu-id="e170d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e170d-110">自分のもの</span><span class="sxs-lookup"><span data-stu-id="e170d-110">userDefined</span></span>|<span data-ttu-id="e170d-111">.0</span><span class="sxs-lookup"><span data-stu-id="e170d-111">0</span></span>|<span data-ttu-id="e170d-112">ユーザー定義、既定値、意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="e170d-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="e170d-113">厳格</span><span class="sxs-lookup"><span data-stu-id="e170d-113">strict</span></span>|<span data-ttu-id="e170d-114">1-d</span><span class="sxs-lookup"><span data-stu-id="e170d-114">1</span></span>|<span data-ttu-id="e170d-115">アダルトコンテンツに対する厳密で最高のフィルタリング。</span><span class="sxs-lookup"><span data-stu-id="e170d-115">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="e170d-116">多く</span><span class="sxs-lookup"><span data-stu-id="e170d-116">moderate</span></span>|<span data-ttu-id="e170d-117">pbm-2</span><span class="sxs-lookup"><span data-stu-id="e170d-117">2</span></span>|<span data-ttu-id="e170d-118">成人向けコンテンツに対するフィルター処理を中程度にする (有効な検索結果はフィルター処理されません)。</span><span class="sxs-lookup"><span data-stu-id="e170d-118">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|



