---
title: vppTokenState 列挙型
description: Apple Volume Purchase Program のトークンに関連付けられている状態。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: c1effcc94eb7ed0929902c935c848e4610c1971b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037232"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="cdf7b-103">vppTokenState 列挙型</span><span class="sxs-lookup"><span data-stu-id="cdf7b-103">vppTokenState enum type</span></span>

> <span data-ttu-id="cdf7b-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="cdf7b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cdf7b-105">Apple Volume Purchase Program のトークンに関連付けられている状態。</span><span class="sxs-lookup"><span data-stu-id="cdf7b-105">Possible states associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="cdf7b-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="cdf7b-106">Members</span></span>
|<span data-ttu-id="cdf7b-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="cdf7b-107">Member</span></span>|<span data-ttu-id="cdf7b-108">値</span><span class="sxs-lookup"><span data-stu-id="cdf7b-108">Value</span></span>|<span data-ttu-id="cdf7b-109">説明</span><span class="sxs-lookup"><span data-stu-id="cdf7b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cdf7b-110">不明</span><span class="sxs-lookup"><span data-stu-id="cdf7b-110">unknown</span></span>|<span data-ttu-id="cdf7b-111">.0</span><span class="sxs-lookup"><span data-stu-id="cdf7b-111">0</span></span>|<span data-ttu-id="cdf7b-112">既定の状態です。</span><span class="sxs-lookup"><span data-stu-id="cdf7b-112">Default state.</span></span>|
|<span data-ttu-id="cdf7b-113">有効な</span><span class="sxs-lookup"><span data-stu-id="cdf7b-113">valid</span></span>|<span data-ttu-id="cdf7b-114">1-d</span><span class="sxs-lookup"><span data-stu-id="cdf7b-114">1</span></span>|<span data-ttu-id="cdf7b-115">トークンが有効です。</span><span class="sxs-lookup"><span data-stu-id="cdf7b-115">Token is valid.</span></span>|
|<span data-ttu-id="cdf7b-116">終了</span><span class="sxs-lookup"><span data-stu-id="cdf7b-116">expired</span></span>|<span data-ttu-id="cdf7b-117">pbm-2</span><span class="sxs-lookup"><span data-stu-id="cdf7b-117">2</span></span>|<span data-ttu-id="cdf7b-118">トークンの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="cdf7b-118">Token is expired.</span></span>|
|<span data-ttu-id="cdf7b-119">無効です</span><span class="sxs-lookup"><span data-stu-id="cdf7b-119">invalid</span></span>|<span data-ttu-id="cdf7b-120">1/3</span><span class="sxs-lookup"><span data-stu-id="cdf7b-120">3</span></span>|<span data-ttu-id="cdf7b-121">トークンが無効です。</span><span class="sxs-lookup"><span data-stu-id="cdf7b-121">Token is invalid.</span></span>|
|<span data-ttu-id="cdf7b-122">assignedToExternalMDM</span><span class="sxs-lookup"><span data-stu-id="cdf7b-122">assignedToExternalMDM</span></span>|<span data-ttu-id="cdf7b-123">2/4</span><span class="sxs-lookup"><span data-stu-id="cdf7b-123">4</span></span>|<span data-ttu-id="cdf7b-124">トークンは別の MDM サービスによって管理されています。</span><span class="sxs-lookup"><span data-stu-id="cdf7b-124">Token is managed by another MDM Service.</span></span>|



