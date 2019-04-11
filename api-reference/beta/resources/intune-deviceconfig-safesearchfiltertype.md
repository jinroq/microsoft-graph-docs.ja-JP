---
title: safeSearchFilterType 列挙型
description: 安全な検索のレベル (アダルトコンテンツのフィルタリング) を指定します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 564e641fcdc7e0d06d48666881fc3bcedfe3505c
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31794730"
---
# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="302de-103">safeSearchFilterType 列挙型</span><span class="sxs-lookup"><span data-stu-id="302de-103">safeSearchFilterType enum type</span></span>

> <span data-ttu-id="302de-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="302de-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="302de-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="302de-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="302de-106">安全な検索のレベル (アダルトコンテンツのフィルタリング) を指定します。</span><span class="sxs-lookup"><span data-stu-id="302de-106">Specifies what level of safe search (filtering adult content) is required</span></span>

## <a name="members"></a><span data-ttu-id="302de-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="302de-107">Members</span></span>
|<span data-ttu-id="302de-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="302de-108">Member</span></span>|<span data-ttu-id="302de-109">値</span><span class="sxs-lookup"><span data-stu-id="302de-109">Value</span></span>|<span data-ttu-id="302de-110">説明</span><span class="sxs-lookup"><span data-stu-id="302de-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="302de-111">自分のもの</span><span class="sxs-lookup"><span data-stu-id="302de-111">userDefined</span></span>|<span data-ttu-id="302de-112">.0</span><span class="sxs-lookup"><span data-stu-id="302de-112">0</span></span>|<span data-ttu-id="302de-113">ユーザー定義、既定値、意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="302de-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="302de-114">厳格</span><span class="sxs-lookup"><span data-stu-id="302de-114">strict</span></span>|<span data-ttu-id="302de-115">1-d</span><span class="sxs-lookup"><span data-stu-id="302de-115">1</span></span>|<span data-ttu-id="302de-116">アダルトコンテンツに対する厳密で最高のフィルタリング。</span><span class="sxs-lookup"><span data-stu-id="302de-116">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="302de-117">多く</span><span class="sxs-lookup"><span data-stu-id="302de-117">moderate</span></span>|<span data-ttu-id="302de-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="302de-118">2</span></span>|<span data-ttu-id="302de-119">成人向けコンテンツに対するフィルター処理を中程度にする (有効な検索結果はフィルター処理されません)。</span><span class="sxs-lookup"><span data-stu-id="302de-119">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|





