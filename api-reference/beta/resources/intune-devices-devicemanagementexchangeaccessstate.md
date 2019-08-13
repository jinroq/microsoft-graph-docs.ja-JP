---
title: deviceManagementExchangeAccessState 列挙型
description: デバイスの Exchange アクセス状態。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 497838ee7cd27600d892b7c7db544e3aa306295e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36370110"
---
# <a name="devicemanagementexchangeaccessstate-enum-type"></a><span data-ttu-id="4f1e3-103">deviceManagementExchangeAccessState 列挙型</span><span class="sxs-lookup"><span data-stu-id="4f1e3-103">deviceManagementExchangeAccessState enum type</span></span>

> <span data-ttu-id="4f1e3-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4f1e3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4f1e3-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4f1e3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f1e3-106">デバイスの Exchange アクセス状態。</span><span class="sxs-lookup"><span data-stu-id="4f1e3-106">Device Exchange Access State.</span></span>

## <a name="members"></a><span data-ttu-id="4f1e3-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="4f1e3-107">Members</span></span>
|<span data-ttu-id="4f1e3-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="4f1e3-108">Member</span></span>|<span data-ttu-id="4f1e3-109">値</span><span class="sxs-lookup"><span data-stu-id="4f1e3-109">Value</span></span>|<span data-ttu-id="4f1e3-110">説明</span><span class="sxs-lookup"><span data-stu-id="4f1e3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f1e3-111">none</span><span class="sxs-lookup"><span data-stu-id="4f1e3-111">none</span></span>|<span data-ttu-id="4f1e3-112">.0</span><span class="sxs-lookup"><span data-stu-id="4f1e3-112">0</span></span>|<span data-ttu-id="4f1e3-113">Exchange から検出されたアクセス状態なし</span><span class="sxs-lookup"><span data-stu-id="4f1e3-113">No access state discovered from Exchange</span></span>|
|<span data-ttu-id="4f1e3-114">不明</span><span class="sxs-lookup"><span data-stu-id="4f1e3-114">unknown</span></span>|<span data-ttu-id="4f1e3-115">1-d</span><span class="sxs-lookup"><span data-stu-id="4f1e3-115">1</span></span>|<span data-ttu-id="4f1e3-116">Exchange へのデバイスアクセス状態が不明です</span><span class="sxs-lookup"><span data-stu-id="4f1e3-116">Device access state to Exchange is unknown</span></span>|
|<span data-ttu-id="4f1e3-117">れる</span><span class="sxs-lookup"><span data-stu-id="4f1e3-117">allowed</span></span>|<span data-ttu-id="4f1e3-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="4f1e3-118">2</span></span>|<span data-ttu-id="4f1e3-119">デバイスが Exchange にアクセスできる</span><span class="sxs-lookup"><span data-stu-id="4f1e3-119">Device has access to Exchange</span></span>|
|<span data-ttu-id="4f1e3-120">ブロック</span><span class="sxs-lookup"><span data-stu-id="4f1e3-120">blocked</span></span>|<span data-ttu-id="4f1e3-121">1/3</span><span class="sxs-lookup"><span data-stu-id="4f1e3-121">3</span></span>|<span data-ttu-id="4f1e3-122">Exchange でデバイスがブロックされている</span><span class="sxs-lookup"><span data-stu-id="4f1e3-122">Device is Blocked in Exchange</span></span>|
|<span data-ttu-id="4f1e3-123">隔離</span><span class="sxs-lookup"><span data-stu-id="4f1e3-123">quarantined</span></span>|<span data-ttu-id="4f1e3-124">2/4</span><span class="sxs-lookup"><span data-stu-id="4f1e3-124">4</span></span>|<span data-ttu-id="4f1e3-125">Exchange でのデバイスの検疫</span><span class="sxs-lookup"><span data-stu-id="4f1e3-125">Device is Quarantined in Exchange</span></span>|



