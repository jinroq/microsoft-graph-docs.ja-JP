---
title: devicemanagementexchangeaccessstate 列挙型
description: デバイスの Exchange アクセス状態。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fedbd157c4668397256971c57a4cb5fa355f78c1
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30257604"
---
# <a name="devicemanagementexchangeaccessstate-enum-type"></a><span data-ttu-id="027d7-103">devicemanagementexchangeaccessstate 列挙型</span><span class="sxs-lookup"><span data-stu-id="027d7-103">deviceManagementExchangeAccessState enum type</span></span>

> <span data-ttu-id="027d7-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="027d7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="027d7-105">デバイスの Exchange アクセス状態。</span><span class="sxs-lookup"><span data-stu-id="027d7-105">Device Exchange Access State.</span></span>

## <a name="members"></a><span data-ttu-id="027d7-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="027d7-106">Members</span></span>
|<span data-ttu-id="027d7-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="027d7-107">Member</span></span>|<span data-ttu-id="027d7-108">値</span><span class="sxs-lookup"><span data-stu-id="027d7-108">Value</span></span>|<span data-ttu-id="027d7-109">説明</span><span class="sxs-lookup"><span data-stu-id="027d7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="027d7-110">none</span><span class="sxs-lookup"><span data-stu-id="027d7-110">none</span></span>|<span data-ttu-id="027d7-111">.0</span><span class="sxs-lookup"><span data-stu-id="027d7-111">0</span></span>|<span data-ttu-id="027d7-112">Exchange から検出されたアクセス状態なし</span><span class="sxs-lookup"><span data-stu-id="027d7-112">No access state discovered from Exchange</span></span>|
|<span data-ttu-id="027d7-113">不明</span><span class="sxs-lookup"><span data-stu-id="027d7-113">unknown</span></span>|<span data-ttu-id="027d7-114">1-d</span><span class="sxs-lookup"><span data-stu-id="027d7-114">1</span></span>|<span data-ttu-id="027d7-115">Exchange へのデバイスアクセス状態が不明です</span><span class="sxs-lookup"><span data-stu-id="027d7-115">Device access state to Exchange is unknown</span></span>|
|<span data-ttu-id="027d7-116">れる</span><span class="sxs-lookup"><span data-stu-id="027d7-116">allowed</span></span>|<span data-ttu-id="027d7-117">pbm-2</span><span class="sxs-lookup"><span data-stu-id="027d7-117">2</span></span>|<span data-ttu-id="027d7-118">デバイスが Exchange にアクセスできる</span><span class="sxs-lookup"><span data-stu-id="027d7-118">Device has access to Exchange</span></span>|
|<span data-ttu-id="027d7-119">ブロック</span><span class="sxs-lookup"><span data-stu-id="027d7-119">blocked</span></span>|<span data-ttu-id="027d7-120">1/3</span><span class="sxs-lookup"><span data-stu-id="027d7-120">3</span></span>|<span data-ttu-id="027d7-121">Exchange でデバイスがブロックされている</span><span class="sxs-lookup"><span data-stu-id="027d7-121">Device is Blocked in Exchange</span></span>|
|<span data-ttu-id="027d7-122">隔離</span><span class="sxs-lookup"><span data-stu-id="027d7-122">quarantined</span></span>|<span data-ttu-id="027d7-123">2/4</span><span class="sxs-lookup"><span data-stu-id="027d7-123">4</span></span>|<span data-ttu-id="027d7-124">Exchange でのデバイスの検疫</span><span class="sxs-lookup"><span data-stu-id="027d7-124">Device is Quarantined in Exchange</span></span>|



