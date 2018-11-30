---
title: vppTokenState 列挙型
description: Apple ボリューム購入プログラム、トークンに関連付けられている状態です。
ms.openlocfilehash: 74d7ea2e0ca2dd03b82b71bea2ab5300214b095d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020464"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="4de4c-103">vppTokenState 列挙型</span><span class="sxs-lookup"><span data-stu-id="4de4c-103">vppTokenState enum type</span></span>

> <span data-ttu-id="4de4c-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4de4c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4de4c-105">Apple ボリューム購入プログラム、トークンに関連付けられている状態です。</span><span class="sxs-lookup"><span data-stu-id="4de4c-105">Possible states associated with an Apple Volume Purchase Program token.</span></span>
## <a name="members"></a><span data-ttu-id="4de4c-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="4de4c-106">Members</span></span>
|<span data-ttu-id="4de4c-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="4de4c-107">Member</span></span>|<span data-ttu-id="4de4c-108">値</span><span class="sxs-lookup"><span data-stu-id="4de4c-108">Value</span></span>|<span data-ttu-id="4de4c-109">説明</span><span class="sxs-lookup"><span data-stu-id="4de4c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4de4c-110">不明</span><span class="sxs-lookup"><span data-stu-id="4de4c-110">unknown</span></span>|<span data-ttu-id="4de4c-111">0</span><span class="sxs-lookup"><span data-stu-id="4de4c-111">0</span></span>|<span data-ttu-id="4de4c-112">既定の状態。</span><span class="sxs-lookup"><span data-stu-id="4de4c-112">Default state.</span></span>|
|<span data-ttu-id="4de4c-113">有効です</span><span class="sxs-lookup"><span data-stu-id="4de4c-113">valid</span></span>|<span data-ttu-id="4de4c-114">1</span><span class="sxs-lookup"><span data-stu-id="4de4c-114">1</span></span>|<span data-ttu-id="4de4c-115">トークンは、有効です。</span><span class="sxs-lookup"><span data-stu-id="4de4c-115">Token is valid.</span></span>|
|<span data-ttu-id="4de4c-116">有効期限が切れてください。</span><span class="sxs-lookup"><span data-stu-id="4de4c-116">expired</span></span>|<span data-ttu-id="4de4c-117">2</span><span class="sxs-lookup"><span data-stu-id="4de4c-117">2</span></span>|<span data-ttu-id="4de4c-118">トークンの期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="4de4c-118">Token is expired.</span></span>|
|<span data-ttu-id="4de4c-119">無効です</span><span class="sxs-lookup"><span data-stu-id="4de4c-119">invalid</span></span>|<span data-ttu-id="4de4c-120">3</span><span class="sxs-lookup"><span data-stu-id="4de4c-120">3</span></span>|<span data-ttu-id="4de4c-121">トークンが有効ではありません。</span><span class="sxs-lookup"><span data-stu-id="4de4c-121">Token is invalid.</span></span>|
|<span data-ttu-id="4de4c-122">assignedToExternalMDM</span><span class="sxs-lookup"><span data-stu-id="4de4c-122">assignedToExternalMDM</span></span>|<span data-ttu-id="4de4c-123">4</span><span class="sxs-lookup"><span data-stu-id="4de4c-123">4</span></span>|<span data-ttu-id="4de4c-124">トークンは、別の MDM サービスによって管理されます。</span><span class="sxs-lookup"><span data-stu-id="4de4c-124">Token is managed by another MDM Service.</span></span>|



