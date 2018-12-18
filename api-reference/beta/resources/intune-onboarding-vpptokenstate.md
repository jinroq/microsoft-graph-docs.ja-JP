---
title: vppTokenState 列挙型
description: Apple ボリューム購入プログラム、トークンに関連付けられている状態です。
author: tfitzmac
ms.openlocfilehash: 70ff74a888e351d7f55c64a68771e221f9a644b4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306581"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="022af-103">vppTokenState 列挙型</span><span class="sxs-lookup"><span data-stu-id="022af-103">vppTokenState enum type</span></span>

> <span data-ttu-id="022af-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="022af-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="022af-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="022af-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="022af-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="022af-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="022af-107">Apple ボリューム購入プログラム、トークンに関連付けられている状態です。</span><span class="sxs-lookup"><span data-stu-id="022af-107">Possible states associated with an Apple Volume Purchase Program token.</span></span>
## <a name="members"></a><span data-ttu-id="022af-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="022af-108">Members</span></span>
|<span data-ttu-id="022af-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="022af-109">Member</span></span>|<span data-ttu-id="022af-110">値</span><span class="sxs-lookup"><span data-stu-id="022af-110">Value</span></span>|<span data-ttu-id="022af-111">説明</span><span class="sxs-lookup"><span data-stu-id="022af-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="022af-112">不明</span><span class="sxs-lookup"><span data-stu-id="022af-112">unknown</span></span>|<span data-ttu-id="022af-113">0</span><span class="sxs-lookup"><span data-stu-id="022af-113">0</span></span>|<span data-ttu-id="022af-114">既定の状態。</span><span class="sxs-lookup"><span data-stu-id="022af-114">Default state.</span></span>|
|<span data-ttu-id="022af-115">有効です</span><span class="sxs-lookup"><span data-stu-id="022af-115">valid</span></span>|<span data-ttu-id="022af-116">1</span><span class="sxs-lookup"><span data-stu-id="022af-116">1</span></span>|<span data-ttu-id="022af-117">トークンは、有効です。</span><span class="sxs-lookup"><span data-stu-id="022af-117">Token is valid.</span></span>|
|<span data-ttu-id="022af-118">有効期限が切れてください。</span><span class="sxs-lookup"><span data-stu-id="022af-118">expired</span></span>|<span data-ttu-id="022af-119">2</span><span class="sxs-lookup"><span data-stu-id="022af-119">2</span></span>|<span data-ttu-id="022af-120">トークンの期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="022af-120">Token is expired.</span></span>|
|<span data-ttu-id="022af-121">無効です</span><span class="sxs-lookup"><span data-stu-id="022af-121">invalid</span></span>|<span data-ttu-id="022af-122">3</span><span class="sxs-lookup"><span data-stu-id="022af-122">3</span></span>|<span data-ttu-id="022af-123">トークンが有効ではありません。</span><span class="sxs-lookup"><span data-stu-id="022af-123">Token is invalid.</span></span>|
|<span data-ttu-id="022af-124">assignedToExternalMDM</span><span class="sxs-lookup"><span data-stu-id="022af-124">assignedToExternalMDM</span></span>|<span data-ttu-id="022af-125">4</span><span class="sxs-lookup"><span data-stu-id="022af-125">4</span></span>|<span data-ttu-id="022af-126">トークンは、別の MDM サービスによって管理されます。</span><span class="sxs-lookup"><span data-stu-id="022af-126">Token is managed by another MDM Service.</span></span>|





