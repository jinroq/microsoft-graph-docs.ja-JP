---
title: safeSearchFilterType 列挙型
description: 安全な検索のレベル (アダルトコンテンツのフィルタリング) を指定します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: a5fa53c28f743f23a8e8e0544182ab62b98c6ced
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36368080"
---
# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="77c34-103">safeSearchFilterType 列挙型</span><span class="sxs-lookup"><span data-stu-id="77c34-103">safeSearchFilterType enum type</span></span>

> <span data-ttu-id="77c34-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="77c34-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="77c34-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="77c34-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77c34-106">安全な検索のレベル (アダルトコンテンツのフィルタリング) を指定します。</span><span class="sxs-lookup"><span data-stu-id="77c34-106">Specifies what level of safe search (filtering adult content) is required</span></span>

## <a name="members"></a><span data-ttu-id="77c34-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="77c34-107">Members</span></span>
|<span data-ttu-id="77c34-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="77c34-108">Member</span></span>|<span data-ttu-id="77c34-109">値</span><span class="sxs-lookup"><span data-stu-id="77c34-109">Value</span></span>|<span data-ttu-id="77c34-110">説明</span><span class="sxs-lookup"><span data-stu-id="77c34-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77c34-111">自分のもの</span><span class="sxs-lookup"><span data-stu-id="77c34-111">userDefined</span></span>|<span data-ttu-id="77c34-112">.0</span><span class="sxs-lookup"><span data-stu-id="77c34-112">0</span></span>|<span data-ttu-id="77c34-113">ユーザー定義、既定値、意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="77c34-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="77c34-114">厳格</span><span class="sxs-lookup"><span data-stu-id="77c34-114">strict</span></span>|<span data-ttu-id="77c34-115">1-d</span><span class="sxs-lookup"><span data-stu-id="77c34-115">1</span></span>|<span data-ttu-id="77c34-116">アダルトコンテンツに対する厳密で最高のフィルタリング。</span><span class="sxs-lookup"><span data-stu-id="77c34-116">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="77c34-117">多く</span><span class="sxs-lookup"><span data-stu-id="77c34-117">moderate</span></span>|<span data-ttu-id="77c34-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="77c34-118">2</span></span>|<span data-ttu-id="77c34-119">成人向けコンテンツに対するフィルター処理を中程度にする (有効な検索結果はフィルター処理されません)。</span><span class="sxs-lookup"><span data-stu-id="77c34-119">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|



