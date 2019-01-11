---
title: safeSearchFilterType 列挙型
description: (成人向けコンテンツのフィルタ リング)、安全な検索のレベルが必要なを指定します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 28aea918c35bb9d90f514e4a8838f219c212405b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830857"
---
# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="24f58-103">safeSearchFilterType 列挙型</span><span class="sxs-lookup"><span data-stu-id="24f58-103">safeSearchFilterType enum type</span></span>

> <span data-ttu-id="24f58-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="24f58-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="24f58-105">(成人向けコンテンツのフィルタ リング)、安全な検索のレベルが必要なを指定します。</span><span class="sxs-lookup"><span data-stu-id="24f58-105">Specifies what level of safe search (filtering adult content) is required</span></span>
## <a name="members"></a><span data-ttu-id="24f58-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="24f58-106">Members</span></span>
|<span data-ttu-id="24f58-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="24f58-107">Member</span></span>|<span data-ttu-id="24f58-108">値</span><span class="sxs-lookup"><span data-stu-id="24f58-108">Value</span></span>|<span data-ttu-id="24f58-109">説明</span><span class="sxs-lookup"><span data-stu-id="24f58-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24f58-110">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="24f58-110">userDefined</span></span>|<span data-ttu-id="24f58-111">0</span><span class="sxs-lookup"><span data-stu-id="24f58-111">0</span></span>|<span data-ttu-id="24f58-112">ユーザー定義、既定値、ない目的。</span><span class="sxs-lookup"><span data-stu-id="24f58-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="24f58-113">厳密です</span><span class="sxs-lookup"><span data-stu-id="24f58-113">strict</span></span>|<span data-ttu-id="24f58-114">1</span><span class="sxs-lookup"><span data-stu-id="24f58-114">1</span></span>|<span data-ttu-id="24f58-115">厳密で、最高の成人向けコンテンツのフィルタ リングします。</span><span class="sxs-lookup"><span data-stu-id="24f58-115">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="24f58-116">中程度</span><span class="sxs-lookup"><span data-stu-id="24f58-116">moderate</span></span>|<span data-ttu-id="24f58-117">2</span><span class="sxs-lookup"><span data-stu-id="24f58-117">2</span></span>|<span data-ttu-id="24f58-118">中程度の (有効な検索結果はフィルターされません)、成人向けコンテンツのフィルタ リングします。</span><span class="sxs-lookup"><span data-stu-id="24f58-118">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|



