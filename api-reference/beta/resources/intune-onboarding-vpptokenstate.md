---
title: vppTokenState 列挙型
description: Apple ボリューム購入プログラム、トークンに関連付けられている状態です。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b91090f64340e398bf9d48aff3741941fc0d778a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844836"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="b89fd-103">vppTokenState 列挙型</span><span class="sxs-lookup"><span data-stu-id="b89fd-103">vppTokenState enum type</span></span>

> <span data-ttu-id="b89fd-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b89fd-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b89fd-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b89fd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b89fd-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b89fd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b89fd-107">Apple ボリューム購入プログラム、トークンに関連付けられている状態です。</span><span class="sxs-lookup"><span data-stu-id="b89fd-107">Possible states associated with an Apple Volume Purchase Program token.</span></span>
## <a name="members"></a><span data-ttu-id="b89fd-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="b89fd-108">Members</span></span>
|<span data-ttu-id="b89fd-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="b89fd-109">Member</span></span>|<span data-ttu-id="b89fd-110">値</span><span class="sxs-lookup"><span data-stu-id="b89fd-110">Value</span></span>|<span data-ttu-id="b89fd-111">説明</span><span class="sxs-lookup"><span data-stu-id="b89fd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b89fd-112">不明</span><span class="sxs-lookup"><span data-stu-id="b89fd-112">unknown</span></span>|<span data-ttu-id="b89fd-113">0</span><span class="sxs-lookup"><span data-stu-id="b89fd-113">0</span></span>|<span data-ttu-id="b89fd-114">既定の状態。</span><span class="sxs-lookup"><span data-stu-id="b89fd-114">Default state.</span></span>|
|<span data-ttu-id="b89fd-115">有効です</span><span class="sxs-lookup"><span data-stu-id="b89fd-115">valid</span></span>|<span data-ttu-id="b89fd-116">1</span><span class="sxs-lookup"><span data-stu-id="b89fd-116">1</span></span>|<span data-ttu-id="b89fd-117">トークンは、有効です。</span><span class="sxs-lookup"><span data-stu-id="b89fd-117">Token is valid.</span></span>|
|<span data-ttu-id="b89fd-118">有効期限が切れてください。</span><span class="sxs-lookup"><span data-stu-id="b89fd-118">expired</span></span>|<span data-ttu-id="b89fd-119">2</span><span class="sxs-lookup"><span data-stu-id="b89fd-119">2</span></span>|<span data-ttu-id="b89fd-120">トークンの期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="b89fd-120">Token is expired.</span></span>|
|<span data-ttu-id="b89fd-121">無効です</span><span class="sxs-lookup"><span data-stu-id="b89fd-121">invalid</span></span>|<span data-ttu-id="b89fd-122">3</span><span class="sxs-lookup"><span data-stu-id="b89fd-122">3</span></span>|<span data-ttu-id="b89fd-123">トークンが有効ではありません。</span><span class="sxs-lookup"><span data-stu-id="b89fd-123">Token is invalid.</span></span>|
|<span data-ttu-id="b89fd-124">assignedToExternalMDM</span><span class="sxs-lookup"><span data-stu-id="b89fd-124">assignedToExternalMDM</span></span>|<span data-ttu-id="b89fd-125">4</span><span class="sxs-lookup"><span data-stu-id="b89fd-125">4</span></span>|<span data-ttu-id="b89fd-126">トークンは、別の MDM サービスによって管理されます。</span><span class="sxs-lookup"><span data-stu-id="b89fd-126">Token is managed by another MDM Service.</span></span>|





