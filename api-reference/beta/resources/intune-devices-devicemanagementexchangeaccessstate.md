---
title: deviceManagementExchangeAccessState 列挙型
description: デバイスの Exchange アクセス状態。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 35c110734078484f7bec5aac1ad31df0b66a0473
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34983037"
---
# <a name="devicemanagementexchangeaccessstate-enum-type"></a><span data-ttu-id="b36fa-103">deviceManagementExchangeAccessState 列挙型</span><span class="sxs-lookup"><span data-stu-id="b36fa-103">deviceManagementExchangeAccessState enum type</span></span>

> <span data-ttu-id="b36fa-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b36fa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b36fa-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b36fa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b36fa-106">デバイスの Exchange アクセス状態。</span><span class="sxs-lookup"><span data-stu-id="b36fa-106">Device Exchange Access State.</span></span>

## <a name="members"></a><span data-ttu-id="b36fa-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="b36fa-107">Members</span></span>
|<span data-ttu-id="b36fa-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="b36fa-108">Member</span></span>|<span data-ttu-id="b36fa-109">値</span><span class="sxs-lookup"><span data-stu-id="b36fa-109">Value</span></span>|<span data-ttu-id="b36fa-110">説明</span><span class="sxs-lookup"><span data-stu-id="b36fa-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b36fa-111">none</span><span class="sxs-lookup"><span data-stu-id="b36fa-111">none</span></span>|<span data-ttu-id="b36fa-112">.0</span><span class="sxs-lookup"><span data-stu-id="b36fa-112">0</span></span>|<span data-ttu-id="b36fa-113">Exchange から検出されたアクセス状態なし</span><span class="sxs-lookup"><span data-stu-id="b36fa-113">No access state discovered from Exchange</span></span>|
|<span data-ttu-id="b36fa-114">不明</span><span class="sxs-lookup"><span data-stu-id="b36fa-114">unknown</span></span>|<span data-ttu-id="b36fa-115">1-d</span><span class="sxs-lookup"><span data-stu-id="b36fa-115">1</span></span>|<span data-ttu-id="b36fa-116">Exchange へのデバイスアクセス状態が不明です</span><span class="sxs-lookup"><span data-stu-id="b36fa-116">Device access state to Exchange is unknown</span></span>|
|<span data-ttu-id="b36fa-117">れる</span><span class="sxs-lookup"><span data-stu-id="b36fa-117">allowed</span></span>|<span data-ttu-id="b36fa-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="b36fa-118">2</span></span>|<span data-ttu-id="b36fa-119">デバイスが Exchange にアクセスできる</span><span class="sxs-lookup"><span data-stu-id="b36fa-119">Device has access to Exchange</span></span>|
|<span data-ttu-id="b36fa-120">ブロック</span><span class="sxs-lookup"><span data-stu-id="b36fa-120">blocked</span></span>|<span data-ttu-id="b36fa-121">1/3</span><span class="sxs-lookup"><span data-stu-id="b36fa-121">3</span></span>|<span data-ttu-id="b36fa-122">Exchange でデバイスがブロックされている</span><span class="sxs-lookup"><span data-stu-id="b36fa-122">Device is Blocked in Exchange</span></span>|
|<span data-ttu-id="b36fa-123">隔離</span><span class="sxs-lookup"><span data-stu-id="b36fa-123">quarantined</span></span>|<span data-ttu-id="b36fa-124">2/4</span><span class="sxs-lookup"><span data-stu-id="b36fa-124">4</span></span>|<span data-ttu-id="b36fa-125">Exchange でのデバイスの検疫</span><span class="sxs-lookup"><span data-stu-id="b36fa-125">Device is Quarantined in Exchange</span></span>|





