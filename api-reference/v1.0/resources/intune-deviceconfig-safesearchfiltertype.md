---
title: safeSearchFilterType 列挙型
description: (成人向けコンテンツのフィルタ リング)、安全な検索のレベルが必要なを指定します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 788a266cdd0161ce1cfef426a7fcf4d9726e3324
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27964614"
---
# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="498dc-103">safeSearchFilterType 列挙型</span><span class="sxs-lookup"><span data-stu-id="498dc-103">safeSearchFilterType enum type</span></span>

> <span data-ttu-id="498dc-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="498dc-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="498dc-105">(成人向けコンテンツのフィルタ リング)、安全な検索のレベルが必要なを指定します。</span><span class="sxs-lookup"><span data-stu-id="498dc-105">Specifies what level of safe search (filtering adult content) is required</span></span>
## <a name="members"></a><span data-ttu-id="498dc-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="498dc-106">Members</span></span>
|<span data-ttu-id="498dc-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="498dc-107">Member</span></span>|<span data-ttu-id="498dc-108">値</span><span class="sxs-lookup"><span data-stu-id="498dc-108">Value</span></span>|<span data-ttu-id="498dc-109">説明</span><span class="sxs-lookup"><span data-stu-id="498dc-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="498dc-110">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="498dc-110">userDefined</span></span>|<span data-ttu-id="498dc-111">0</span><span class="sxs-lookup"><span data-stu-id="498dc-111">0</span></span>|<span data-ttu-id="498dc-112">ユーザー定義、既定値、ない目的。</span><span class="sxs-lookup"><span data-stu-id="498dc-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="498dc-113">厳密です</span><span class="sxs-lookup"><span data-stu-id="498dc-113">strict</span></span>|<span data-ttu-id="498dc-114">1</span><span class="sxs-lookup"><span data-stu-id="498dc-114">1</span></span>|<span data-ttu-id="498dc-115">厳密で、最高の成人向けコンテンツのフィルタ リングします。</span><span class="sxs-lookup"><span data-stu-id="498dc-115">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="498dc-116">中程度</span><span class="sxs-lookup"><span data-stu-id="498dc-116">moderate</span></span>|<span data-ttu-id="498dc-117">2</span><span class="sxs-lookup"><span data-stu-id="498dc-117">2</span></span>|<span data-ttu-id="498dc-118">中程度の (有効な検索結果はフィルターされません)、成人向けコンテンツのフィルタ リングします。</span><span class="sxs-lookup"><span data-stu-id="498dc-118">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|



