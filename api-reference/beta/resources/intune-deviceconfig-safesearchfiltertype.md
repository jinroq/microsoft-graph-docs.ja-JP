---
title: safeSearchFilterType 列挙型
description: 安全な検索のレベル (アダルトコンテンツのフィルタリング) を指定します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 196131eb11efad25a4b2fa541bf1b20d85dda33e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140174"
---
# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="c176a-103">safeSearchFilterType 列挙型</span><span class="sxs-lookup"><span data-stu-id="c176a-103">safeSearchFilterType enum type</span></span>

> <span data-ttu-id="c176a-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c176a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c176a-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c176a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c176a-106">安全な検索のレベル (アダルトコンテンツのフィルタリング) を指定します。</span><span class="sxs-lookup"><span data-stu-id="c176a-106">Specifies what level of safe search (filtering adult content) is required</span></span>

## <a name="members"></a><span data-ttu-id="c176a-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="c176a-107">Members</span></span>
|<span data-ttu-id="c176a-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="c176a-108">Member</span></span>|<span data-ttu-id="c176a-109">値</span><span class="sxs-lookup"><span data-stu-id="c176a-109">Value</span></span>|<span data-ttu-id="c176a-110">説明</span><span class="sxs-lookup"><span data-stu-id="c176a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c176a-111">自分のもの</span><span class="sxs-lookup"><span data-stu-id="c176a-111">userDefined</span></span>|<span data-ttu-id="c176a-112">.0</span><span class="sxs-lookup"><span data-stu-id="c176a-112">0</span></span>|<span data-ttu-id="c176a-113">ユーザー定義、既定値、意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="c176a-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="c176a-114">厳格</span><span class="sxs-lookup"><span data-stu-id="c176a-114">strict</span></span>|<span data-ttu-id="c176a-115">1-d</span><span class="sxs-lookup"><span data-stu-id="c176a-115">1</span></span>|<span data-ttu-id="c176a-116">アダルトコンテンツに対する厳密で最高のフィルタリング。</span><span class="sxs-lookup"><span data-stu-id="c176a-116">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="c176a-117">多く</span><span class="sxs-lookup"><span data-stu-id="c176a-117">moderate</span></span>|<span data-ttu-id="c176a-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="c176a-118">2</span></span>|<span data-ttu-id="c176a-119">成人向けコンテンツに対するフィルター処理を中程度にする (有効な検索結果はフィルター処理されません)。</span><span class="sxs-lookup"><span data-stu-id="c176a-119">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|




