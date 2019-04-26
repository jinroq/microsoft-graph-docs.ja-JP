---
title: safeSearchFilterType 列挙型
description: 安全な検索のレベル (アダルトコンテンツのフィルタリング) を指定します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c82f80f6081f57a88fcdf26f7639277d72b5e0d8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534900"
---
# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="44a90-103">safeSearchFilterType 列挙型</span><span class="sxs-lookup"><span data-stu-id="44a90-103">safeSearchFilterType enum type</span></span>

> <span data-ttu-id="44a90-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="44a90-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44a90-105">安全な検索のレベル (アダルトコンテンツのフィルタリング) を指定します。</span><span class="sxs-lookup"><span data-stu-id="44a90-105">Specifies what level of safe search (filtering adult content) is required</span></span>

## <a name="members"></a><span data-ttu-id="44a90-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="44a90-106">Members</span></span>
|<span data-ttu-id="44a90-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="44a90-107">Member</span></span>|<span data-ttu-id="44a90-108">値</span><span class="sxs-lookup"><span data-stu-id="44a90-108">Value</span></span>|<span data-ttu-id="44a90-109">説明</span><span class="sxs-lookup"><span data-stu-id="44a90-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44a90-110">自分のもの</span><span class="sxs-lookup"><span data-stu-id="44a90-110">userDefined</span></span>|<span data-ttu-id="44a90-111">.0</span><span class="sxs-lookup"><span data-stu-id="44a90-111">0</span></span>|<span data-ttu-id="44a90-112">ユーザー定義、既定値、意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="44a90-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="44a90-113">厳格</span><span class="sxs-lookup"><span data-stu-id="44a90-113">strict</span></span>|<span data-ttu-id="44a90-114">1 </span><span class="sxs-lookup"><span data-stu-id="44a90-114">1</span></span>|<span data-ttu-id="44a90-115">アダルトコンテンツに対する厳密で最高のフィルタリング。</span><span class="sxs-lookup"><span data-stu-id="44a90-115">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="44a90-116">多く</span><span class="sxs-lookup"><span data-stu-id="44a90-116">moderate</span></span>|<span data-ttu-id="44a90-117">2 </span><span class="sxs-lookup"><span data-stu-id="44a90-117">2</span></span>|<span data-ttu-id="44a90-118">成人向けコンテンツに対するフィルター処理を中程度にする (有効な検索結果はフィルター処理されません)。</span><span class="sxs-lookup"><span data-stu-id="44a90-118">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|



