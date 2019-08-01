---
title: safeSearchFilterType 列挙型
description: 安全な検索のレベル (アダルトコンテンツのフィルタリング) を指定します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: c88542d6d06f623d20a294cc49aff321692c75a6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36027854"
---
# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="2bc86-103">safeSearchFilterType 列挙型</span><span class="sxs-lookup"><span data-stu-id="2bc86-103">safeSearchFilterType enum type</span></span>

> <span data-ttu-id="2bc86-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2bc86-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2bc86-105">安全な検索のレベル (アダルトコンテンツのフィルタリング) を指定します。</span><span class="sxs-lookup"><span data-stu-id="2bc86-105">Specifies what level of safe search (filtering adult content) is required</span></span>

## <a name="members"></a><span data-ttu-id="2bc86-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="2bc86-106">Members</span></span>
|<span data-ttu-id="2bc86-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="2bc86-107">Member</span></span>|<span data-ttu-id="2bc86-108">値</span><span class="sxs-lookup"><span data-stu-id="2bc86-108">Value</span></span>|<span data-ttu-id="2bc86-109">説明</span><span class="sxs-lookup"><span data-stu-id="2bc86-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2bc86-110">自分のもの</span><span class="sxs-lookup"><span data-stu-id="2bc86-110">userDefined</span></span>|<span data-ttu-id="2bc86-111">.0</span><span class="sxs-lookup"><span data-stu-id="2bc86-111">0</span></span>|<span data-ttu-id="2bc86-112">ユーザー定義、既定値、意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="2bc86-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="2bc86-113">厳格</span><span class="sxs-lookup"><span data-stu-id="2bc86-113">strict</span></span>|<span data-ttu-id="2bc86-114">1-d</span><span class="sxs-lookup"><span data-stu-id="2bc86-114">1</span></span>|<span data-ttu-id="2bc86-115">アダルトコンテンツに対する厳密で最高のフィルタリング。</span><span class="sxs-lookup"><span data-stu-id="2bc86-115">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="2bc86-116">多く</span><span class="sxs-lookup"><span data-stu-id="2bc86-116">moderate</span></span>|<span data-ttu-id="2bc86-117">pbm-2</span><span class="sxs-lookup"><span data-stu-id="2bc86-117">2</span></span>|<span data-ttu-id="2bc86-118">成人向けコンテンツに対するフィルター処理を中程度にする (有効な検索結果はフィルター処理されません)。</span><span class="sxs-lookup"><span data-stu-id="2bc86-118">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|



