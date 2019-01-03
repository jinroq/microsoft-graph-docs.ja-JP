---
title: vppTokenState 列挙型
description: Apple ボリューム購入プログラム、トークンに関連付けられている状態です。
author: tfitzmac
ms.openlocfilehash: e034f9712e2ef40b40b209935ed96f07b35cdbb9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321183"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="4532a-103">vppTokenState 列挙型</span><span class="sxs-lookup"><span data-stu-id="4532a-103">vppTokenState enum type</span></span>

> <span data-ttu-id="4532a-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4532a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4532a-105">Apple ボリューム購入プログラム、トークンに関連付けられている状態です。</span><span class="sxs-lookup"><span data-stu-id="4532a-105">Possible states associated with an Apple Volume Purchase Program token.</span></span>
## <a name="members"></a><span data-ttu-id="4532a-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="4532a-106">Members</span></span>
|<span data-ttu-id="4532a-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="4532a-107">Member</span></span>|<span data-ttu-id="4532a-108">値</span><span class="sxs-lookup"><span data-stu-id="4532a-108">Value</span></span>|<span data-ttu-id="4532a-109">説明</span><span class="sxs-lookup"><span data-stu-id="4532a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4532a-110">不明</span><span class="sxs-lookup"><span data-stu-id="4532a-110">unknown</span></span>|<span data-ttu-id="4532a-111">0</span><span class="sxs-lookup"><span data-stu-id="4532a-111">0</span></span>|<span data-ttu-id="4532a-112">既定の状態。</span><span class="sxs-lookup"><span data-stu-id="4532a-112">Default state.</span></span>|
|<span data-ttu-id="4532a-113">有効です</span><span class="sxs-lookup"><span data-stu-id="4532a-113">valid</span></span>|<span data-ttu-id="4532a-114">1</span><span class="sxs-lookup"><span data-stu-id="4532a-114">1</span></span>|<span data-ttu-id="4532a-115">トークンは、有効です。</span><span class="sxs-lookup"><span data-stu-id="4532a-115">Token is valid.</span></span>|
|<span data-ttu-id="4532a-116">有効期限が切れてください。</span><span class="sxs-lookup"><span data-stu-id="4532a-116">expired</span></span>|<span data-ttu-id="4532a-117">2</span><span class="sxs-lookup"><span data-stu-id="4532a-117">2</span></span>|<span data-ttu-id="4532a-118">トークンの期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="4532a-118">Token is expired.</span></span>|
|<span data-ttu-id="4532a-119">無効です</span><span class="sxs-lookup"><span data-stu-id="4532a-119">invalid</span></span>|<span data-ttu-id="4532a-120">3</span><span class="sxs-lookup"><span data-stu-id="4532a-120">3</span></span>|<span data-ttu-id="4532a-121">トークンが有効ではありません。</span><span class="sxs-lookup"><span data-stu-id="4532a-121">Token is invalid.</span></span>|
|<span data-ttu-id="4532a-122">assignedToExternalMDM</span><span class="sxs-lookup"><span data-stu-id="4532a-122">assignedToExternalMDM</span></span>|<span data-ttu-id="4532a-123">4</span><span class="sxs-lookup"><span data-stu-id="4532a-123">4</span></span>|<span data-ttu-id="4532a-124">トークンは、別の MDM サービスによって管理されます。</span><span class="sxs-lookup"><span data-stu-id="4532a-124">Token is managed by another MDM Service.</span></span>|


