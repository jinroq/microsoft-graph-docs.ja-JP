---
title: vppTokenState 列挙型
description: Apple ボリューム購入プログラム、トークンに関連付けられている状態です。
ms.openlocfilehash: 7180364063a48e1b0eeb2778ed4def7c0d3930a6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069713"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="2e7b4-103">vppTokenState 列挙型</span><span class="sxs-lookup"><span data-stu-id="2e7b4-103">vppTokenState enum type</span></span>

> <span data-ttu-id="2e7b4-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2e7b4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2e7b4-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2e7b4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2e7b4-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2e7b4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2e7b4-107">Apple ボリューム購入プログラム、トークンに関連付けられている状態です。</span><span class="sxs-lookup"><span data-stu-id="2e7b4-107">Possible states associated with an Apple Volume Purchase Program token.</span></span>
## <a name="members"></a><span data-ttu-id="2e7b4-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="2e7b4-108">Members</span></span>
|<span data-ttu-id="2e7b4-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="2e7b4-109">Member</span></span>|<span data-ttu-id="2e7b4-110">値</span><span class="sxs-lookup"><span data-stu-id="2e7b4-110">Value</span></span>|<span data-ttu-id="2e7b4-111">説明</span><span class="sxs-lookup"><span data-stu-id="2e7b4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e7b4-112">不明</span><span class="sxs-lookup"><span data-stu-id="2e7b4-112">unknown</span></span>|<span data-ttu-id="2e7b4-113">0</span><span class="sxs-lookup"><span data-stu-id="2e7b4-113">0</span></span>|<span data-ttu-id="2e7b4-114">既定の状態。</span><span class="sxs-lookup"><span data-stu-id="2e7b4-114">Default state.</span></span>|
|<span data-ttu-id="2e7b4-115">有効です</span><span class="sxs-lookup"><span data-stu-id="2e7b4-115">valid</span></span>|<span data-ttu-id="2e7b4-116">1</span><span class="sxs-lookup"><span data-stu-id="2e7b4-116">1</span></span>|<span data-ttu-id="2e7b4-117">トークンは、有効です。</span><span class="sxs-lookup"><span data-stu-id="2e7b4-117">Token is valid.</span></span>|
|<span data-ttu-id="2e7b4-118">有効期限が切れてください。</span><span class="sxs-lookup"><span data-stu-id="2e7b4-118">expired</span></span>|<span data-ttu-id="2e7b4-119">2</span><span class="sxs-lookup"><span data-stu-id="2e7b4-119">2</span></span>|<span data-ttu-id="2e7b4-120">トークンの期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="2e7b4-120">Token is expired.</span></span>|
|<span data-ttu-id="2e7b4-121">無効です</span><span class="sxs-lookup"><span data-stu-id="2e7b4-121">invalid</span></span>|<span data-ttu-id="2e7b4-122">3</span><span class="sxs-lookup"><span data-stu-id="2e7b4-122">3</span></span>|<span data-ttu-id="2e7b4-123">トークンが有効ではありません。</span><span class="sxs-lookup"><span data-stu-id="2e7b4-123">Token is invalid.</span></span>|
|<span data-ttu-id="2e7b4-124">assignedToExternalMDM</span><span class="sxs-lookup"><span data-stu-id="2e7b4-124">assignedToExternalMDM</span></span>|<span data-ttu-id="2e7b4-125">4</span><span class="sxs-lookup"><span data-stu-id="2e7b4-125">4</span></span>|<span data-ttu-id="2e7b4-126">トークンは、別の MDM サービスによって管理されます。</span><span class="sxs-lookup"><span data-stu-id="2e7b4-126">Token is managed by another MDM Service.</span></span>|





