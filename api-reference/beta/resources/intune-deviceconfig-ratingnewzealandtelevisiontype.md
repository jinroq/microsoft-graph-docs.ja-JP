---
title: ratingNewZealandTelevisionType 列挙型
description: ニュージーランドのテレビのコンテンツの規制ラベル
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f26568d6fdaedd06a243720127b7937581f819c5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982751"
---
# <a name="ratingnewzealandtelevisiontype-enum-type"></a><span data-ttu-id="9e58d-103">ratingNewZealandTelevisionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="9e58d-103">ratingNewZealandTelevisionType enum type</span></span>

> <span data-ttu-id="9e58d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9e58d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9e58d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9e58d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9e58d-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9e58d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9e58d-107">ニュージーランドのテレビのコンテンツの規制ラベル</span><span class="sxs-lookup"><span data-stu-id="9e58d-107">TV content rating labels in New Zealand</span></span>
## <a name="members"></a><span data-ttu-id="9e58d-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="9e58d-108">Members</span></span>
|<span data-ttu-id="9e58d-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="9e58d-109">Member</span></span>|<span data-ttu-id="9e58d-110">値</span><span class="sxs-lookup"><span data-stu-id="9e58d-110">Value</span></span>|<span data-ttu-id="9e58d-111">説明</span><span class="sxs-lookup"><span data-stu-id="9e58d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e58d-112">allAllowed</span><span class="sxs-lookup"><span data-stu-id="9e58d-112">allAllowed</span></span>|<span data-ttu-id="9e58d-113">0</span><span class="sxs-lookup"><span data-stu-id="9e58d-113">0</span></span>|<span data-ttu-id="9e58d-114">既定値、すべてのテレビ番組コンテンツを許可します。</span><span class="sxs-lookup"><span data-stu-id="9e58d-114">Default value, allow all TV shows content</span></span>|
|<span data-ttu-id="9e58d-115">allBlocked</span><span class="sxs-lookup"><span data-stu-id="9e58d-115">allBlocked</span></span>|<span data-ttu-id="9e58d-116">1</span><span class="sxs-lookup"><span data-stu-id="9e58d-116">1</span></span>|<span data-ttu-id="9e58d-117">任意のテレビ番組コンテンツを許可しません。</span><span class="sxs-lookup"><span data-stu-id="9e58d-117">Do not allow any TV shows content</span></span>|
|<span data-ttu-id="9e58d-118">全般</span><span class="sxs-lookup"><span data-stu-id="9e58d-118">general</span></span>|<span data-ttu-id="9e58d-119">2</span><span class="sxs-lookup"><span data-stu-id="9e58d-119">2</span></span>|<span data-ttu-id="9e58d-120">G 分類 14 下の子に害を与える可能性の高い材料を除外します。</span><span class="sxs-lookup"><span data-stu-id="9e58d-120">The G classification excludes materials likely to harm children under 14</span></span>|
|<span data-ttu-id="9e58d-121">parentalGuidance</span><span class="sxs-lookup"><span data-stu-id="9e58d-121">parentalGuidance</span></span>|<span data-ttu-id="9e58d-122">3</span><span class="sxs-lookup"><span data-stu-id="9e58d-122">3</span></span>|<span data-ttu-id="9e58d-123">PGR のクラス分けが若い視聴者を監督するには、親と保護者を促進します。</span><span class="sxs-lookup"><span data-stu-id="9e58d-123">The PGR classification encourages parents and guardians to supervise younger viewers</span></span>|
|<span data-ttu-id="9e58d-124">大人</span><span class="sxs-lookup"><span data-stu-id="9e58d-124">adults</span></span>|<span data-ttu-id="9e58d-125">4</span><span class="sxs-lookup"><span data-stu-id="9e58d-125">4</span></span>|<span data-ttu-id="9e58d-126">AO 分類が子供に適していません。</span><span class="sxs-lookup"><span data-stu-id="9e58d-126">The AO classification is not suitable for children</span></span>|





