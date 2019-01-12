---
title: vppTokenState 列挙型
description: Apple ボリューム購入プログラム、トークンに関連付けられている状態です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6bdeb73b6491f3960ce30db91a35d06c0f8ffaf1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986664"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="0de86-103">vppTokenState 列挙型</span><span class="sxs-lookup"><span data-stu-id="0de86-103">vppTokenState enum type</span></span>

> <span data-ttu-id="0de86-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0de86-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0de86-105">Apple ボリューム購入プログラム、トークンに関連付けられている状態です。</span><span class="sxs-lookup"><span data-stu-id="0de86-105">Possible states associated with an Apple Volume Purchase Program token.</span></span>
## <a name="members"></a><span data-ttu-id="0de86-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="0de86-106">Members</span></span>
|<span data-ttu-id="0de86-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="0de86-107">Member</span></span>|<span data-ttu-id="0de86-108">値</span><span class="sxs-lookup"><span data-stu-id="0de86-108">Value</span></span>|<span data-ttu-id="0de86-109">説明</span><span class="sxs-lookup"><span data-stu-id="0de86-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0de86-110">不明</span><span class="sxs-lookup"><span data-stu-id="0de86-110">unknown</span></span>|<span data-ttu-id="0de86-111">0</span><span class="sxs-lookup"><span data-stu-id="0de86-111">0</span></span>|<span data-ttu-id="0de86-112">既定の状態。</span><span class="sxs-lookup"><span data-stu-id="0de86-112">Default state.</span></span>|
|<span data-ttu-id="0de86-113">有効です</span><span class="sxs-lookup"><span data-stu-id="0de86-113">valid</span></span>|<span data-ttu-id="0de86-114">1</span><span class="sxs-lookup"><span data-stu-id="0de86-114">1</span></span>|<span data-ttu-id="0de86-115">トークンは、有効です。</span><span class="sxs-lookup"><span data-stu-id="0de86-115">Token is valid.</span></span>|
|<span data-ttu-id="0de86-116">有効期限が切れてください。</span><span class="sxs-lookup"><span data-stu-id="0de86-116">expired</span></span>|<span data-ttu-id="0de86-117">2</span><span class="sxs-lookup"><span data-stu-id="0de86-117">2</span></span>|<span data-ttu-id="0de86-118">トークンの期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="0de86-118">Token is expired.</span></span>|
|<span data-ttu-id="0de86-119">無効です</span><span class="sxs-lookup"><span data-stu-id="0de86-119">invalid</span></span>|<span data-ttu-id="0de86-120">3</span><span class="sxs-lookup"><span data-stu-id="0de86-120">3</span></span>|<span data-ttu-id="0de86-121">トークンが有効ではありません。</span><span class="sxs-lookup"><span data-stu-id="0de86-121">Token is invalid.</span></span>|
|<span data-ttu-id="0de86-122">assignedToExternalMDM</span><span class="sxs-lookup"><span data-stu-id="0de86-122">assignedToExternalMDM</span></span>|<span data-ttu-id="0de86-123">4</span><span class="sxs-lookup"><span data-stu-id="0de86-123">4</span></span>|<span data-ttu-id="0de86-124">トークンは、別の MDM サービスによって管理されます。</span><span class="sxs-lookup"><span data-stu-id="0de86-124">Token is managed by another MDM Service.</span></span>|



