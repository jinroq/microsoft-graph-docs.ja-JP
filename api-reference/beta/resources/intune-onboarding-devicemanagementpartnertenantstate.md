---
title: devicemanagementpartnertenantstate 列挙型
description: このテナントのパートナーの状態。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 11276fa24b5128c52c39fcc4c8a944df39c865b2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30153334"
---
# <a name="devicemanagementpartnertenantstate-enum-type"></a><span data-ttu-id="efd63-103">devicemanagementpartnertenantstate 列挙型</span><span class="sxs-lookup"><span data-stu-id="efd63-103">deviceManagementPartnerTenantState enum type</span></span>

> <span data-ttu-id="efd63-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="efd63-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="efd63-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="efd63-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="efd63-106">このテナントのパートナーの状態。</span><span class="sxs-lookup"><span data-stu-id="efd63-106">Partner state of this tenant.</span></span>

## <a name="members"></a><span data-ttu-id="efd63-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="efd63-107">Members</span></span>
|<span data-ttu-id="efd63-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="efd63-108">Member</span></span>|<span data-ttu-id="efd63-109">値</span><span class="sxs-lookup"><span data-stu-id="efd63-109">Value</span></span>|<span data-ttu-id="efd63-110">説明</span><span class="sxs-lookup"><span data-stu-id="efd63-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="efd63-111">不明</span><span class="sxs-lookup"><span data-stu-id="efd63-111">unknown</span></span>|<span data-ttu-id="efd63-112">.0</span><span class="sxs-lookup"><span data-stu-id="efd63-112">0</span></span>|<span data-ttu-id="efd63-113">パートナーの状態が不明です。</span><span class="sxs-lookup"><span data-stu-id="efd63-113">Partner state is unknown.</span></span>|
|<span data-ttu-id="efd63-114">無効</span><span class="sxs-lookup"><span data-stu-id="efd63-114">unavailable</span></span>|<span data-ttu-id="efd63-115">1-d</span><span class="sxs-lookup"><span data-stu-id="efd63-115">1</span></span>|<span data-ttu-id="efd63-116">パートナーは利用できません。</span><span class="sxs-lookup"><span data-stu-id="efd63-116">Partner is unavailable.</span></span>|
|<span data-ttu-id="efd63-117">enabled</span><span class="sxs-lookup"><span data-stu-id="efd63-117">enabled</span></span>|<span data-ttu-id="efd63-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="efd63-118">2</span></span>|<span data-ttu-id="efd63-119">パートナーが有効になっている。</span><span class="sxs-lookup"><span data-stu-id="efd63-119">Partner is enabled.</span></span>|
|<span data-ttu-id="efd63-120">停止</span><span class="sxs-lookup"><span data-stu-id="efd63-120">terminated</span></span>|<span data-ttu-id="efd63-121">1/3</span><span class="sxs-lookup"><span data-stu-id="efd63-121">3</span></span>|<span data-ttu-id="efd63-122">パートナー接続が終了します。</span><span class="sxs-lookup"><span data-stu-id="efd63-122">Partner connection is terminated.</span></span>|
|<span data-ttu-id="efd63-123">rejected</span><span class="sxs-lookup"><span data-stu-id="efd63-123">rejected</span></span>|<span data-ttu-id="efd63-124">2/4</span><span class="sxs-lookup"><span data-stu-id="efd63-124">4</span></span>|<span data-ttu-id="efd63-125">パートナーメッセージは拒否されます。</span><span class="sxs-lookup"><span data-stu-id="efd63-125">Partner messages are rejected.</span></span>|
|<span data-ttu-id="efd63-126">なかっ</span><span class="sxs-lookup"><span data-stu-id="efd63-126">unresponsive</span></span>|<span data-ttu-id="efd63-127">5</span><span class="sxs-lookup"><span data-stu-id="efd63-127">5</span></span>|<span data-ttu-id="efd63-128">パートナーが応答していません。</span><span class="sxs-lookup"><span data-stu-id="efd63-128">Partner is unresponsive.</span></span>|




