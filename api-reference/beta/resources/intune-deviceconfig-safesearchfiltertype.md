---
title: safeSearchFilterType 列挙型
description: (成人向けコンテンツのフィルタ リング)、安全な検索のレベルが必要なを指定します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4493c71b48a0f5ff4b0c48307504087c722393e1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403484"
---
# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="e1a5c-103">safeSearchFilterType 列挙型</span><span class="sxs-lookup"><span data-stu-id="e1a5c-103">safeSearchFilterType enum type</span></span>

> <span data-ttu-id="e1a5c-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e1a5c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e1a5c-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e1a5c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e1a5c-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e1a5c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1a5c-107">(成人向けコンテンツのフィルタ リング)、安全な検索のレベルが必要なを指定します。</span><span class="sxs-lookup"><span data-stu-id="e1a5c-107">Specifies what level of safe search (filtering adult content) is required</span></span>

## <a name="members"></a><span data-ttu-id="e1a5c-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="e1a5c-108">Members</span></span>
|<span data-ttu-id="e1a5c-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="e1a5c-109">Member</span></span>|<span data-ttu-id="e1a5c-110">値</span><span class="sxs-lookup"><span data-stu-id="e1a5c-110">Value</span></span>|<span data-ttu-id="e1a5c-111">説明</span><span class="sxs-lookup"><span data-stu-id="e1a5c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1a5c-112">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="e1a5c-112">userDefined</span></span>|<span data-ttu-id="e1a5c-113">0</span><span class="sxs-lookup"><span data-stu-id="e1a5c-113">0</span></span>|<span data-ttu-id="e1a5c-114">ユーザー定義、既定値、ない目的。</span><span class="sxs-lookup"><span data-stu-id="e1a5c-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="e1a5c-115">厳密です</span><span class="sxs-lookup"><span data-stu-id="e1a5c-115">strict</span></span>|<span data-ttu-id="e1a5c-116">1</span><span class="sxs-lookup"><span data-stu-id="e1a5c-116">1</span></span>|<span data-ttu-id="e1a5c-117">厳密で、最高の成人向けコンテンツのフィルタ リングします。</span><span class="sxs-lookup"><span data-stu-id="e1a5c-117">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="e1a5c-118">中程度</span><span class="sxs-lookup"><span data-stu-id="e1a5c-118">moderate</span></span>|<span data-ttu-id="e1a5c-119">2</span><span class="sxs-lookup"><span data-stu-id="e1a5c-119">2</span></span>|<span data-ttu-id="e1a5c-120">中程度の (有効な検索結果はフィルターされません)、成人向けコンテンツのフィルタ リングします。</span><span class="sxs-lookup"><span data-stu-id="e1a5c-120">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|




