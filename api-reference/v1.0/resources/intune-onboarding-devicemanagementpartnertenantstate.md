---
title: deviceManagementPartnerTenantState 列挙型
description: このテナントのパートナーの状態。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 103fd9149e7bc17a7f72a5af5ab002f136e616d7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037388"
---
# <a name="devicemanagementpartnertenantstate-enum-type"></a><span data-ttu-id="9ebcd-103">deviceManagementPartnerTenantState 列挙型</span><span class="sxs-lookup"><span data-stu-id="9ebcd-103">deviceManagementPartnerTenantState enum type</span></span>

> <span data-ttu-id="9ebcd-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9ebcd-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ebcd-105">このテナントのパートナーの状態。</span><span class="sxs-lookup"><span data-stu-id="9ebcd-105">Partner state of this tenant.</span></span>

## <a name="members"></a><span data-ttu-id="9ebcd-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="9ebcd-106">Members</span></span>
|<span data-ttu-id="9ebcd-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="9ebcd-107">Member</span></span>|<span data-ttu-id="9ebcd-108">値</span><span class="sxs-lookup"><span data-stu-id="9ebcd-108">Value</span></span>|<span data-ttu-id="9ebcd-109">説明</span><span class="sxs-lookup"><span data-stu-id="9ebcd-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ebcd-110">不明</span><span class="sxs-lookup"><span data-stu-id="9ebcd-110">unknown</span></span>|<span data-ttu-id="9ebcd-111">.0</span><span class="sxs-lookup"><span data-stu-id="9ebcd-111">0</span></span>|<span data-ttu-id="9ebcd-112">パートナーの状態が不明です。</span><span class="sxs-lookup"><span data-stu-id="9ebcd-112">Partner state is unknown.</span></span>|
|<span data-ttu-id="9ebcd-113">無効</span><span class="sxs-lookup"><span data-stu-id="9ebcd-113">unavailable</span></span>|<span data-ttu-id="9ebcd-114">1-d</span><span class="sxs-lookup"><span data-stu-id="9ebcd-114">1</span></span>|<span data-ttu-id="9ebcd-115">パートナーは利用できません。</span><span class="sxs-lookup"><span data-stu-id="9ebcd-115">Partner is unavailable.</span></span>|
|<span data-ttu-id="9ebcd-116">enabled</span><span class="sxs-lookup"><span data-stu-id="9ebcd-116">enabled</span></span>|<span data-ttu-id="9ebcd-117">pbm-2</span><span class="sxs-lookup"><span data-stu-id="9ebcd-117">2</span></span>|<span data-ttu-id="9ebcd-118">パートナーが有効になっている。</span><span class="sxs-lookup"><span data-stu-id="9ebcd-118">Partner is enabled.</span></span>|
|<span data-ttu-id="9ebcd-119">停止</span><span class="sxs-lookup"><span data-stu-id="9ebcd-119">terminated</span></span>|<span data-ttu-id="9ebcd-120">1/3</span><span class="sxs-lookup"><span data-stu-id="9ebcd-120">3</span></span>|<span data-ttu-id="9ebcd-121">パートナー接続が終了します。</span><span class="sxs-lookup"><span data-stu-id="9ebcd-121">Partner connection is terminated.</span></span>|
|<span data-ttu-id="9ebcd-122">拒否</span><span class="sxs-lookup"><span data-stu-id="9ebcd-122">rejected</span></span>|<span data-ttu-id="9ebcd-123">2/4</span><span class="sxs-lookup"><span data-stu-id="9ebcd-123">4</span></span>|<span data-ttu-id="9ebcd-124">パートナーメッセージは拒否されます。</span><span class="sxs-lookup"><span data-stu-id="9ebcd-124">Partner messages are rejected.</span></span>|
|<span data-ttu-id="9ebcd-125">なかっ</span><span class="sxs-lookup"><span data-stu-id="9ebcd-125">unresponsive</span></span>|<span data-ttu-id="9ebcd-126">5</span><span class="sxs-lookup"><span data-stu-id="9ebcd-126">5</span></span>|<span data-ttu-id="9ebcd-127">パートナーが応答していません。</span><span class="sxs-lookup"><span data-stu-id="9ebcd-127">Partner is unresponsive.</span></span>|



