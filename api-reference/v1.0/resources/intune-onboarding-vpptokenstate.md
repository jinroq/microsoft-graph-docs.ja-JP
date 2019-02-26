---
title: vpptokenstate 列挙型
description: Apple volume purchase program のトークンに関連付けられている状態。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 573fe27064881f670e642e7c3727b8c9eb7db5a9
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254934"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="7d62c-103">vpptokenstate 列挙型</span><span class="sxs-lookup"><span data-stu-id="7d62c-103">vppTokenState enum type</span></span>

> <span data-ttu-id="7d62c-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7d62c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7d62c-105">Apple volume purchase program のトークンに関連付けられている状態。</span><span class="sxs-lookup"><span data-stu-id="7d62c-105">Possible states associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="7d62c-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="7d62c-106">Members</span></span>
|<span data-ttu-id="7d62c-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="7d62c-107">Member</span></span>|<span data-ttu-id="7d62c-108">値</span><span class="sxs-lookup"><span data-stu-id="7d62c-108">Value</span></span>|<span data-ttu-id="7d62c-109">説明</span><span class="sxs-lookup"><span data-stu-id="7d62c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d62c-110">不明</span><span class="sxs-lookup"><span data-stu-id="7d62c-110">unknown</span></span>|<span data-ttu-id="7d62c-111">.0</span><span class="sxs-lookup"><span data-stu-id="7d62c-111">0</span></span>|<span data-ttu-id="7d62c-112">既定の状態です。</span><span class="sxs-lookup"><span data-stu-id="7d62c-112">Default state.</span></span>|
|<span data-ttu-id="7d62c-113">有効な</span><span class="sxs-lookup"><span data-stu-id="7d62c-113">valid</span></span>|<span data-ttu-id="7d62c-114">1-d</span><span class="sxs-lookup"><span data-stu-id="7d62c-114">1</span></span>|<span data-ttu-id="7d62c-115">トークンが有効です。</span><span class="sxs-lookup"><span data-stu-id="7d62c-115">Token is valid.</span></span>|
|<span data-ttu-id="7d62c-116">終了</span><span class="sxs-lookup"><span data-stu-id="7d62c-116">expired</span></span>|<span data-ttu-id="7d62c-117">pbm-2</span><span class="sxs-lookup"><span data-stu-id="7d62c-117">2</span></span>|<span data-ttu-id="7d62c-118">トークンの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="7d62c-118">Token is expired.</span></span>|
|<span data-ttu-id="7d62c-119">無効です</span><span class="sxs-lookup"><span data-stu-id="7d62c-119">invalid</span></span>|<span data-ttu-id="7d62c-120">1/3</span><span class="sxs-lookup"><span data-stu-id="7d62c-120">3</span></span>|<span data-ttu-id="7d62c-121">トークンが無効です。</span><span class="sxs-lookup"><span data-stu-id="7d62c-121">Token is invalid.</span></span>|
|<span data-ttu-id="7d62c-122">assignedToExternalMDM</span><span class="sxs-lookup"><span data-stu-id="7d62c-122">assignedToExternalMDM</span></span>|<span data-ttu-id="7d62c-123">2/4</span><span class="sxs-lookup"><span data-stu-id="7d62c-123">4</span></span>|<span data-ttu-id="7d62c-124">トークンは別の MDM サービスによって管理されています。</span><span class="sxs-lookup"><span data-stu-id="7d62c-124">Token is managed by another MDM Service.</span></span>|



