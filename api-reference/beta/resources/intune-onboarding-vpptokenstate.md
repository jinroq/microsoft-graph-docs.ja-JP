---
title: vppTokenState 列挙型
description: Apple ボリューム購入プログラム、トークンに関連付けられている状態です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b8e2148cccbb891b1c139abd9d15ba424b3b3e9b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967379"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="ab846-103">vppTokenState 列挙型</span><span class="sxs-lookup"><span data-stu-id="ab846-103">vppTokenState enum type</span></span>

> <span data-ttu-id="ab846-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ab846-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ab846-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ab846-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ab846-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ab846-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ab846-107">Apple ボリューム購入プログラム、トークンに関連付けられている状態です。</span><span class="sxs-lookup"><span data-stu-id="ab846-107">Possible states associated with an Apple Volume Purchase Program token.</span></span>
## <a name="members"></a><span data-ttu-id="ab846-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="ab846-108">Members</span></span>
|<span data-ttu-id="ab846-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="ab846-109">Member</span></span>|<span data-ttu-id="ab846-110">値</span><span class="sxs-lookup"><span data-stu-id="ab846-110">Value</span></span>|<span data-ttu-id="ab846-111">説明</span><span class="sxs-lookup"><span data-stu-id="ab846-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab846-112">不明</span><span class="sxs-lookup"><span data-stu-id="ab846-112">unknown</span></span>|<span data-ttu-id="ab846-113">0</span><span class="sxs-lookup"><span data-stu-id="ab846-113">0</span></span>|<span data-ttu-id="ab846-114">既定の状態。</span><span class="sxs-lookup"><span data-stu-id="ab846-114">Default state.</span></span>|
|<span data-ttu-id="ab846-115">有効です</span><span class="sxs-lookup"><span data-stu-id="ab846-115">valid</span></span>|<span data-ttu-id="ab846-116">1</span><span class="sxs-lookup"><span data-stu-id="ab846-116">1</span></span>|<span data-ttu-id="ab846-117">トークンは、有効です。</span><span class="sxs-lookup"><span data-stu-id="ab846-117">Token is valid.</span></span>|
|<span data-ttu-id="ab846-118">有効期限が切れてください。</span><span class="sxs-lookup"><span data-stu-id="ab846-118">expired</span></span>|<span data-ttu-id="ab846-119">2</span><span class="sxs-lookup"><span data-stu-id="ab846-119">2</span></span>|<span data-ttu-id="ab846-120">トークンの期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="ab846-120">Token is expired.</span></span>|
|<span data-ttu-id="ab846-121">無効です</span><span class="sxs-lookup"><span data-stu-id="ab846-121">invalid</span></span>|<span data-ttu-id="ab846-122">3</span><span class="sxs-lookup"><span data-stu-id="ab846-122">3</span></span>|<span data-ttu-id="ab846-123">トークンが有効ではありません。</span><span class="sxs-lookup"><span data-stu-id="ab846-123">Token is invalid.</span></span>|
|<span data-ttu-id="ab846-124">assignedToExternalMDM</span><span class="sxs-lookup"><span data-stu-id="ab846-124">assignedToExternalMDM</span></span>|<span data-ttu-id="ab846-125">4</span><span class="sxs-lookup"><span data-stu-id="ab846-125">4</span></span>|<span data-ttu-id="ab846-126">トークンは、別の MDM サービスによって管理されます。</span><span class="sxs-lookup"><span data-stu-id="ab846-126">Token is managed by another MDM Service.</span></span>|





