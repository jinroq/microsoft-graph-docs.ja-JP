---
title: deviceManagementExchangeAccessState 列挙型
description: デバイスの Exchange のアクセスの状態です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f66f8372b5bd087ad620fa86d8e0beff8b3eb3a0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401069"
---
# <a name="devicemanagementexchangeaccessstate-enum-type"></a><span data-ttu-id="285ba-103">deviceManagementExchangeAccessState 列挙型</span><span class="sxs-lookup"><span data-stu-id="285ba-103">deviceManagementExchangeAccessState enum type</span></span>

> <span data-ttu-id="285ba-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="285ba-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="285ba-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="285ba-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="285ba-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="285ba-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="285ba-107">デバイスの Exchange のアクセスの状態です。</span><span class="sxs-lookup"><span data-stu-id="285ba-107">Device Exchange Access State.</span></span>

## <a name="members"></a><span data-ttu-id="285ba-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="285ba-108">Members</span></span>
|<span data-ttu-id="285ba-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="285ba-109">Member</span></span>|<span data-ttu-id="285ba-110">値</span><span class="sxs-lookup"><span data-stu-id="285ba-110">Value</span></span>|<span data-ttu-id="285ba-111">説明</span><span class="sxs-lookup"><span data-stu-id="285ba-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="285ba-112">none</span><span class="sxs-lookup"><span data-stu-id="285ba-112">none</span></span>|<span data-ttu-id="285ba-113">0</span><span class="sxs-lookup"><span data-stu-id="285ba-113">0</span></span>|<span data-ttu-id="285ba-114">Exchange から検出アクセス状態がないです。</span><span class="sxs-lookup"><span data-stu-id="285ba-114">No access state discovered from Exchange</span></span>|
|<span data-ttu-id="285ba-115">不明</span><span class="sxs-lookup"><span data-stu-id="285ba-115">unknown</span></span>|<span data-ttu-id="285ba-116">1</span><span class="sxs-lookup"><span data-stu-id="285ba-116">1</span></span>|<span data-ttu-id="285ba-117">Exchange へのデバイスのアクセス状態は不明です。</span><span class="sxs-lookup"><span data-stu-id="285ba-117">Device access state to Exchange is unknown</span></span>|
|<span data-ttu-id="285ba-118">許可</span><span class="sxs-lookup"><span data-stu-id="285ba-118">allowed</span></span>|<span data-ttu-id="285ba-119">2</span><span class="sxs-lookup"><span data-stu-id="285ba-119">2</span></span>|<span data-ttu-id="285ba-120">デバイスが Exchange へのアクセス権を持つ</span><span class="sxs-lookup"><span data-stu-id="285ba-120">Device has access to Exchange</span></span>|
|<span data-ttu-id="285ba-121">ブロック</span><span class="sxs-lookup"><span data-stu-id="285ba-121">blocked</span></span>|<span data-ttu-id="285ba-122">3</span><span class="sxs-lookup"><span data-stu-id="285ba-122">3</span></span>|<span data-ttu-id="285ba-123">デバイスが Exchange でブロックされています。</span><span class="sxs-lookup"><span data-stu-id="285ba-123">Device is Blocked in Exchange</span></span>|
|<span data-ttu-id="285ba-124">検疫</span><span class="sxs-lookup"><span data-stu-id="285ba-124">quarantined</span></span>|<span data-ttu-id="285ba-125">4</span><span class="sxs-lookup"><span data-stu-id="285ba-125">4</span></span>|<span data-ttu-id="285ba-126">デバイスが Exchange の検疫します。</span><span class="sxs-lookup"><span data-stu-id="285ba-126">Device is Quarantined in Exchange</span></span>|




