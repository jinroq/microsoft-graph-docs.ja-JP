---
title: safeSearchFilterType 列挙型
description: (成人向けコンテンツのフィルタ リング)、安全な検索のレベルが必要なを指定します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 477f0b52342ca1b27d844a5f03aedd806cdd8b5d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875832"
---
# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="e22ec-103">safeSearchFilterType 列挙型</span><span class="sxs-lookup"><span data-stu-id="e22ec-103">safeSearchFilterType enum type</span></span>

> <span data-ttu-id="e22ec-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e22ec-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e22ec-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e22ec-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e22ec-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e22ec-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e22ec-107">(成人向けコンテンツのフィルタ リング)、安全な検索のレベルが必要なを指定します。</span><span class="sxs-lookup"><span data-stu-id="e22ec-107">Specifies what level of safe search (filtering adult content) is required</span></span>
## <a name="members"></a><span data-ttu-id="e22ec-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="e22ec-108">Members</span></span>
|<span data-ttu-id="e22ec-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="e22ec-109">Member</span></span>|<span data-ttu-id="e22ec-110">値</span><span class="sxs-lookup"><span data-stu-id="e22ec-110">Value</span></span>|<span data-ttu-id="e22ec-111">説明</span><span class="sxs-lookup"><span data-stu-id="e22ec-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e22ec-112">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="e22ec-112">userDefined</span></span>|<span data-ttu-id="e22ec-113">0</span><span class="sxs-lookup"><span data-stu-id="e22ec-113">0</span></span>|<span data-ttu-id="e22ec-114">ユーザー定義、既定値、ない目的。</span><span class="sxs-lookup"><span data-stu-id="e22ec-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="e22ec-115">厳密です</span><span class="sxs-lookup"><span data-stu-id="e22ec-115">strict</span></span>|<span data-ttu-id="e22ec-116">1</span><span class="sxs-lookup"><span data-stu-id="e22ec-116">1</span></span>|<span data-ttu-id="e22ec-117">厳密で、最高の成人向けコンテンツのフィルタ リングします。</span><span class="sxs-lookup"><span data-stu-id="e22ec-117">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="e22ec-118">中程度</span><span class="sxs-lookup"><span data-stu-id="e22ec-118">moderate</span></span>|<span data-ttu-id="e22ec-119">2</span><span class="sxs-lookup"><span data-stu-id="e22ec-119">2</span></span>|<span data-ttu-id="e22ec-120">中程度の (有効な検索結果はフィルターされません)、成人向けコンテンツのフィルタ リングします。</span><span class="sxs-lookup"><span data-stu-id="e22ec-120">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|





