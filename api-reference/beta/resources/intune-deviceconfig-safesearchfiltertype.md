---
title: safeSearchFilterType 列挙型
description: 安全な検索のレベル (アダルトコンテンツのフィルタリング) を指定します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 1b11ec96553549f5be971d18f69a7e91d88a4bf0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36000579"
---
# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="6c6a1-103">safeSearchFilterType 列挙型</span><span class="sxs-lookup"><span data-stu-id="6c6a1-103">safeSearchFilterType enum type</span></span>

> <span data-ttu-id="6c6a1-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6c6a1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6c6a1-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6c6a1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c6a1-106">安全な検索のレベル (アダルトコンテンツのフィルタリング) を指定します。</span><span class="sxs-lookup"><span data-stu-id="6c6a1-106">Specifies what level of safe search (filtering adult content) is required</span></span>

## <a name="members"></a><span data-ttu-id="6c6a1-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="6c6a1-107">Members</span></span>
|<span data-ttu-id="6c6a1-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="6c6a1-108">Member</span></span>|<span data-ttu-id="6c6a1-109">値</span><span class="sxs-lookup"><span data-stu-id="6c6a1-109">Value</span></span>|<span data-ttu-id="6c6a1-110">説明</span><span class="sxs-lookup"><span data-stu-id="6c6a1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c6a1-111">自分のもの</span><span class="sxs-lookup"><span data-stu-id="6c6a1-111">userDefined</span></span>|<span data-ttu-id="6c6a1-112">.0</span><span class="sxs-lookup"><span data-stu-id="6c6a1-112">0</span></span>|<span data-ttu-id="6c6a1-113">ユーザー定義、既定値、意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="6c6a1-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="6c6a1-114">厳格</span><span class="sxs-lookup"><span data-stu-id="6c6a1-114">strict</span></span>|<span data-ttu-id="6c6a1-115">1-d</span><span class="sxs-lookup"><span data-stu-id="6c6a1-115">1</span></span>|<span data-ttu-id="6c6a1-116">アダルトコンテンツに対する厳密で最高のフィルタリング。</span><span class="sxs-lookup"><span data-stu-id="6c6a1-116">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="6c6a1-117">多く</span><span class="sxs-lookup"><span data-stu-id="6c6a1-117">moderate</span></span>|<span data-ttu-id="6c6a1-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="6c6a1-118">2</span></span>|<span data-ttu-id="6c6a1-119">成人向けコンテンツに対するフィルター処理を中程度にする (有効な検索結果はフィルター処理されません)。</span><span class="sxs-lookup"><span data-stu-id="6c6a1-119">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|





