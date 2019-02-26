---
title: devicemanagementpartnertenantstate 列挙型
description: このテナントのパートナーの状態。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c14c1806e65ba180837082288b76e047055f8a9f
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30257982"
---
# <a name="devicemanagementpartnertenantstate-enum-type"></a><span data-ttu-id="6360e-103">devicemanagementpartnertenantstate 列挙型</span><span class="sxs-lookup"><span data-stu-id="6360e-103">deviceManagementPartnerTenantState enum type</span></span>

> <span data-ttu-id="6360e-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6360e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6360e-105">このテナントのパートナーの状態。</span><span class="sxs-lookup"><span data-stu-id="6360e-105">Partner state of this tenant.</span></span>

## <a name="members"></a><span data-ttu-id="6360e-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="6360e-106">Members</span></span>
|<span data-ttu-id="6360e-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="6360e-107">Member</span></span>|<span data-ttu-id="6360e-108">値</span><span class="sxs-lookup"><span data-stu-id="6360e-108">Value</span></span>|<span data-ttu-id="6360e-109">説明</span><span class="sxs-lookup"><span data-stu-id="6360e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6360e-110">不明</span><span class="sxs-lookup"><span data-stu-id="6360e-110">unknown</span></span>|<span data-ttu-id="6360e-111">.0</span><span class="sxs-lookup"><span data-stu-id="6360e-111">0</span></span>|<span data-ttu-id="6360e-112">パートナーの状態が不明です。</span><span class="sxs-lookup"><span data-stu-id="6360e-112">Partner state is unknown.</span></span>|
|<span data-ttu-id="6360e-113">無効</span><span class="sxs-lookup"><span data-stu-id="6360e-113">unavailable</span></span>|<span data-ttu-id="6360e-114">1-d</span><span class="sxs-lookup"><span data-stu-id="6360e-114">1</span></span>|<span data-ttu-id="6360e-115">パートナーは利用できません。</span><span class="sxs-lookup"><span data-stu-id="6360e-115">Partner is unavailable.</span></span>|
|<span data-ttu-id="6360e-116">enabled</span><span class="sxs-lookup"><span data-stu-id="6360e-116">enabled</span></span>|<span data-ttu-id="6360e-117">pbm-2</span><span class="sxs-lookup"><span data-stu-id="6360e-117">2</span></span>|<span data-ttu-id="6360e-118">パートナーが有効になっている。</span><span class="sxs-lookup"><span data-stu-id="6360e-118">Partner is enabled.</span></span>|
|<span data-ttu-id="6360e-119">停止</span><span class="sxs-lookup"><span data-stu-id="6360e-119">terminated</span></span>|<span data-ttu-id="6360e-120">1/3</span><span class="sxs-lookup"><span data-stu-id="6360e-120">3</span></span>|<span data-ttu-id="6360e-121">パートナー接続が終了します。</span><span class="sxs-lookup"><span data-stu-id="6360e-121">Partner connection is terminated.</span></span>|
|<span data-ttu-id="6360e-122">rejected</span><span class="sxs-lookup"><span data-stu-id="6360e-122">rejected</span></span>|<span data-ttu-id="6360e-123">2/4</span><span class="sxs-lookup"><span data-stu-id="6360e-123">4</span></span>|<span data-ttu-id="6360e-124">パートナーメッセージは拒否されます。</span><span class="sxs-lookup"><span data-stu-id="6360e-124">Partner messages are rejected.</span></span>|
|<span data-ttu-id="6360e-125">なかっ</span><span class="sxs-lookup"><span data-stu-id="6360e-125">unresponsive</span></span>|<span data-ttu-id="6360e-126">5</span><span class="sxs-lookup"><span data-stu-id="6360e-126">5</span></span>|<span data-ttu-id="6360e-127">パートナーが応答していません。</span><span class="sxs-lookup"><span data-stu-id="6360e-127">Partner is unresponsive.</span></span>|



