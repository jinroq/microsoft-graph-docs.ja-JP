---
title: devicemanagementexchangeaccessstate 列挙型
description: デバイスの Exchange アクセス状態。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fedbd157c4668397256971c57a4cb5fa355f78c1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32584664"
---
# <a name="devicemanagementexchangeaccessstate-enum-type"></a><span data-ttu-id="01106-103">devicemanagementexchangeaccessstate 列挙型</span><span class="sxs-lookup"><span data-stu-id="01106-103">deviceManagementExchangeAccessState enum type</span></span>

> <span data-ttu-id="01106-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="01106-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="01106-105">デバイスの Exchange アクセス状態。</span><span class="sxs-lookup"><span data-stu-id="01106-105">Device Exchange Access State.</span></span>

## <a name="members"></a><span data-ttu-id="01106-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="01106-106">Members</span></span>
|<span data-ttu-id="01106-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="01106-107">Member</span></span>|<span data-ttu-id="01106-108">値</span><span class="sxs-lookup"><span data-stu-id="01106-108">Value</span></span>|<span data-ttu-id="01106-109">説明</span><span class="sxs-lookup"><span data-stu-id="01106-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01106-110">なし</span><span class="sxs-lookup"><span data-stu-id="01106-110">none</span></span>|<span data-ttu-id="01106-111">.0</span><span class="sxs-lookup"><span data-stu-id="01106-111">0</span></span>|<span data-ttu-id="01106-112">Exchange から検出されたアクセス状態なし</span><span class="sxs-lookup"><span data-stu-id="01106-112">No access state discovered from Exchange</span></span>|
|<span data-ttu-id="01106-113">不明</span><span class="sxs-lookup"><span data-stu-id="01106-113">unknown</span></span>|<span data-ttu-id="01106-114">1-d</span><span class="sxs-lookup"><span data-stu-id="01106-114">1</span></span>|<span data-ttu-id="01106-115">Exchange へのデバイスアクセス状態が不明です</span><span class="sxs-lookup"><span data-stu-id="01106-115">Device access state to Exchange is unknown</span></span>|
|<span data-ttu-id="01106-116">れる</span><span class="sxs-lookup"><span data-stu-id="01106-116">allowed</span></span>|<span data-ttu-id="01106-117">pbm-2</span><span class="sxs-lookup"><span data-stu-id="01106-117">2</span></span>|<span data-ttu-id="01106-118">デバイスが Exchange にアクセスできる</span><span class="sxs-lookup"><span data-stu-id="01106-118">Device has access to Exchange</span></span>|
|<span data-ttu-id="01106-119">ブロック</span><span class="sxs-lookup"><span data-stu-id="01106-119">blocked</span></span>|<span data-ttu-id="01106-120">1/3</span><span class="sxs-lookup"><span data-stu-id="01106-120">3</span></span>|<span data-ttu-id="01106-121">Exchange でデバイスがブロックされている</span><span class="sxs-lookup"><span data-stu-id="01106-121">Device is Blocked in Exchange</span></span>|
|<span data-ttu-id="01106-122">隔離</span><span class="sxs-lookup"><span data-stu-id="01106-122">quarantined</span></span>|<span data-ttu-id="01106-123">2/4</span><span class="sxs-lookup"><span data-stu-id="01106-123">4</span></span>|<span data-ttu-id="01106-124">Exchange でのデバイスの検疫</span><span class="sxs-lookup"><span data-stu-id="01106-124">Device is Quarantined in Exchange</span></span>|



