---
title: devicemanagementexchangeaccessstate 列挙型
description: デバイスの Exchange アクセス状態。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c3cbe04dee84418d43dc610253522174caad9b2f
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31788493"
---
# <a name="devicemanagementexchangeaccessstate-enum-type"></a><span data-ttu-id="90919-103">devicemanagementexchangeaccessstate 列挙型</span><span class="sxs-lookup"><span data-stu-id="90919-103">deviceManagementExchangeAccessState enum type</span></span>

> <span data-ttu-id="90919-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="90919-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="90919-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="90919-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90919-106">デバイスの Exchange アクセス状態。</span><span class="sxs-lookup"><span data-stu-id="90919-106">Device Exchange Access State.</span></span>

## <a name="members"></a><span data-ttu-id="90919-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="90919-107">Members</span></span>
|<span data-ttu-id="90919-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="90919-108">Member</span></span>|<span data-ttu-id="90919-109">値</span><span class="sxs-lookup"><span data-stu-id="90919-109">Value</span></span>|<span data-ttu-id="90919-110">説明</span><span class="sxs-lookup"><span data-stu-id="90919-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90919-111">none</span><span class="sxs-lookup"><span data-stu-id="90919-111">none</span></span>|<span data-ttu-id="90919-112">.0</span><span class="sxs-lookup"><span data-stu-id="90919-112">0</span></span>|<span data-ttu-id="90919-113">Exchange から検出されたアクセス状態なし</span><span class="sxs-lookup"><span data-stu-id="90919-113">No access state discovered from Exchange</span></span>|
|<span data-ttu-id="90919-114">不明</span><span class="sxs-lookup"><span data-stu-id="90919-114">unknown</span></span>|<span data-ttu-id="90919-115">1-d</span><span class="sxs-lookup"><span data-stu-id="90919-115">1</span></span>|<span data-ttu-id="90919-116">Exchange へのデバイスアクセス状態が不明です</span><span class="sxs-lookup"><span data-stu-id="90919-116">Device access state to Exchange is unknown</span></span>|
|<span data-ttu-id="90919-117">れる</span><span class="sxs-lookup"><span data-stu-id="90919-117">allowed</span></span>|<span data-ttu-id="90919-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="90919-118">2</span></span>|<span data-ttu-id="90919-119">デバイスが Exchange にアクセスできる</span><span class="sxs-lookup"><span data-stu-id="90919-119">Device has access to Exchange</span></span>|
|<span data-ttu-id="90919-120">ブロック</span><span class="sxs-lookup"><span data-stu-id="90919-120">blocked</span></span>|<span data-ttu-id="90919-121">1/3</span><span class="sxs-lookup"><span data-stu-id="90919-121">3</span></span>|<span data-ttu-id="90919-122">Exchange でデバイスがブロックされている</span><span class="sxs-lookup"><span data-stu-id="90919-122">Device is Blocked in Exchange</span></span>|
|<span data-ttu-id="90919-123">隔離</span><span class="sxs-lookup"><span data-stu-id="90919-123">quarantined</span></span>|<span data-ttu-id="90919-124">2/4</span><span class="sxs-lookup"><span data-stu-id="90919-124">4</span></span>|<span data-ttu-id="90919-125">Exchange でのデバイスの検疫</span><span class="sxs-lookup"><span data-stu-id="90919-125">Device is Quarantined in Exchange</span></span>|





