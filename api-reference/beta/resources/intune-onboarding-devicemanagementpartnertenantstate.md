---
title: deviceManagementPartnerTenantState 列挙型
description: このテナントのパートナーの状態です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0044aae0069ceb87f8a8820e49a114b814da62c6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407292"
---
# <a name="devicemanagementpartnertenantstate-enum-type"></a><span data-ttu-id="52e38-103">deviceManagementPartnerTenantState 列挙型</span><span class="sxs-lookup"><span data-stu-id="52e38-103">deviceManagementPartnerTenantState enum type</span></span>

> <span data-ttu-id="52e38-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="52e38-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="52e38-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="52e38-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="52e38-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="52e38-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="52e38-107">このテナントのパートナーの状態です。</span><span class="sxs-lookup"><span data-stu-id="52e38-107">Partner state of this tenant.</span></span>

## <a name="members"></a><span data-ttu-id="52e38-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="52e38-108">Members</span></span>
|<span data-ttu-id="52e38-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="52e38-109">Member</span></span>|<span data-ttu-id="52e38-110">値</span><span class="sxs-lookup"><span data-stu-id="52e38-110">Value</span></span>|<span data-ttu-id="52e38-111">説明</span><span class="sxs-lookup"><span data-stu-id="52e38-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52e38-112">不明</span><span class="sxs-lookup"><span data-stu-id="52e38-112">unknown</span></span>|<span data-ttu-id="52e38-113">0</span><span class="sxs-lookup"><span data-stu-id="52e38-113">0</span></span>|<span data-ttu-id="52e38-114">パートナーの状態は不明です。</span><span class="sxs-lookup"><span data-stu-id="52e38-114">Partner state is unknown.</span></span>|
|<span data-ttu-id="52e38-115">利用不可</span><span class="sxs-lookup"><span data-stu-id="52e38-115">unavailable</span></span>|<span data-ttu-id="52e38-116">1</span><span class="sxs-lookup"><span data-stu-id="52e38-116">1</span></span>|<span data-ttu-id="52e38-117">パートナーが利用可能ではありません。</span><span class="sxs-lookup"><span data-stu-id="52e38-117">Partner is unavailable.</span></span>|
|<span data-ttu-id="52e38-118">enabled</span><span class="sxs-lookup"><span data-stu-id="52e38-118">enabled</span></span>|<span data-ttu-id="52e38-119">2</span><span class="sxs-lookup"><span data-stu-id="52e38-119">2</span></span>|<span data-ttu-id="52e38-120">パートナーが有効になります。</span><span class="sxs-lookup"><span data-stu-id="52e38-120">Partner is enabled.</span></span>|
|<span data-ttu-id="52e38-121">終了</span><span class="sxs-lookup"><span data-stu-id="52e38-121">terminated</span></span>|<span data-ttu-id="52e38-122">3</span><span class="sxs-lookup"><span data-stu-id="52e38-122">3</span></span>|<span data-ttu-id="52e38-123">パートナー接続は終了します。</span><span class="sxs-lookup"><span data-stu-id="52e38-123">Partner connection is terminated.</span></span>|
|<span data-ttu-id="52e38-124">rejected</span><span class="sxs-lookup"><span data-stu-id="52e38-124">rejected</span></span>|<span data-ttu-id="52e38-125">4</span><span class="sxs-lookup"><span data-stu-id="52e38-125">4</span></span>|<span data-ttu-id="52e38-126">パートナーのメッセージは拒否されます。</span><span class="sxs-lookup"><span data-stu-id="52e38-126">Partner messages are rejected.</span></span>|
|<span data-ttu-id="52e38-127">応答しません。</span><span class="sxs-lookup"><span data-stu-id="52e38-127">unresponsive</span></span>|<span data-ttu-id="52e38-128">5</span><span class="sxs-lookup"><span data-stu-id="52e38-128">5</span></span>|<span data-ttu-id="52e38-129">パートナーは、応答ではありません。</span><span class="sxs-lookup"><span data-stu-id="52e38-129">Partner is unresponsive.</span></span>|




