---
title: vppTokenState 列挙型
description: Apple ボリューム購入プログラム、トークンに関連付けられている状態です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7d0c4ee7ae0b8e35f97a18d0958a2456cab40a10
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416161"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="7915c-103">vppTokenState 列挙型</span><span class="sxs-lookup"><span data-stu-id="7915c-103">vppTokenState enum type</span></span>

> <span data-ttu-id="7915c-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7915c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7915c-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7915c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7915c-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7915c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7915c-107">Apple ボリューム購入プログラム、トークンに関連付けられている状態です。</span><span class="sxs-lookup"><span data-stu-id="7915c-107">Possible states associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="7915c-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="7915c-108">Members</span></span>
|<span data-ttu-id="7915c-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="7915c-109">Member</span></span>|<span data-ttu-id="7915c-110">値</span><span class="sxs-lookup"><span data-stu-id="7915c-110">Value</span></span>|<span data-ttu-id="7915c-111">説明</span><span class="sxs-lookup"><span data-stu-id="7915c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7915c-112">不明</span><span class="sxs-lookup"><span data-stu-id="7915c-112">unknown</span></span>|<span data-ttu-id="7915c-113">0</span><span class="sxs-lookup"><span data-stu-id="7915c-113">0</span></span>|<span data-ttu-id="7915c-114">既定の状態。</span><span class="sxs-lookup"><span data-stu-id="7915c-114">Default state.</span></span>|
|<span data-ttu-id="7915c-115">有効です</span><span class="sxs-lookup"><span data-stu-id="7915c-115">valid</span></span>|<span data-ttu-id="7915c-116">1</span><span class="sxs-lookup"><span data-stu-id="7915c-116">1</span></span>|<span data-ttu-id="7915c-117">トークンは、有効です。</span><span class="sxs-lookup"><span data-stu-id="7915c-117">Token is valid.</span></span>|
|<span data-ttu-id="7915c-118">有効期限が切れてください。</span><span class="sxs-lookup"><span data-stu-id="7915c-118">expired</span></span>|<span data-ttu-id="7915c-119">2</span><span class="sxs-lookup"><span data-stu-id="7915c-119">2</span></span>|<span data-ttu-id="7915c-120">トークンの期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="7915c-120">Token is expired.</span></span>|
|<span data-ttu-id="7915c-121">無効です</span><span class="sxs-lookup"><span data-stu-id="7915c-121">invalid</span></span>|<span data-ttu-id="7915c-122">3</span><span class="sxs-lookup"><span data-stu-id="7915c-122">3</span></span>|<span data-ttu-id="7915c-123">トークンが有効ではありません。</span><span class="sxs-lookup"><span data-stu-id="7915c-123">Token is invalid.</span></span>|
|<span data-ttu-id="7915c-124">assignedToExternalMDM</span><span class="sxs-lookup"><span data-stu-id="7915c-124">assignedToExternalMDM</span></span>|<span data-ttu-id="7915c-125">4</span><span class="sxs-lookup"><span data-stu-id="7915c-125">4</span></span>|<span data-ttu-id="7915c-126">トークンは、別の MDM サービスによって管理されます。</span><span class="sxs-lookup"><span data-stu-id="7915c-126">Token is managed by another MDM Service.</span></span>|




