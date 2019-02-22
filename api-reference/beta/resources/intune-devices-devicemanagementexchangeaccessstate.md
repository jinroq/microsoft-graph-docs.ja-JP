---
title: devicemanagementexchangeaccessstate 列挙型
description: デバイスの Exchange アクセス状態。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 15b0dd7b99d8395b7c66171969bad1cb79bce0b8
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159585"
---
# <a name="devicemanagementexchangeaccessstate-enum-type"></a><span data-ttu-id="8f9ff-103">devicemanagementexchangeaccessstate 列挙型</span><span class="sxs-lookup"><span data-stu-id="8f9ff-103">deviceManagementExchangeAccessState enum type</span></span>

> <span data-ttu-id="8f9ff-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8f9ff-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8f9ff-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8f9ff-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f9ff-106">デバイスの Exchange アクセス状態。</span><span class="sxs-lookup"><span data-stu-id="8f9ff-106">Device Exchange Access State.</span></span>

## <a name="members"></a><span data-ttu-id="8f9ff-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="8f9ff-107">Members</span></span>
|<span data-ttu-id="8f9ff-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="8f9ff-108">Member</span></span>|<span data-ttu-id="8f9ff-109">値</span><span class="sxs-lookup"><span data-stu-id="8f9ff-109">Value</span></span>|<span data-ttu-id="8f9ff-110">説明</span><span class="sxs-lookup"><span data-stu-id="8f9ff-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f9ff-111">none</span><span class="sxs-lookup"><span data-stu-id="8f9ff-111">none</span></span>|<span data-ttu-id="8f9ff-112">.0</span><span class="sxs-lookup"><span data-stu-id="8f9ff-112">0</span></span>|<span data-ttu-id="8f9ff-113">Exchange から検出されたアクセス状態なし</span><span class="sxs-lookup"><span data-stu-id="8f9ff-113">No access state discovered from Exchange</span></span>|
|<span data-ttu-id="8f9ff-114">不明</span><span class="sxs-lookup"><span data-stu-id="8f9ff-114">unknown</span></span>|<span data-ttu-id="8f9ff-115">1-d</span><span class="sxs-lookup"><span data-stu-id="8f9ff-115">1</span></span>|<span data-ttu-id="8f9ff-116">Exchange へのデバイスアクセス状態が不明です</span><span class="sxs-lookup"><span data-stu-id="8f9ff-116">Device access state to Exchange is unknown</span></span>|
|<span data-ttu-id="8f9ff-117">れる</span><span class="sxs-lookup"><span data-stu-id="8f9ff-117">allowed</span></span>|<span data-ttu-id="8f9ff-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="8f9ff-118">2</span></span>|<span data-ttu-id="8f9ff-119">デバイスが Exchange にアクセスできる</span><span class="sxs-lookup"><span data-stu-id="8f9ff-119">Device has access to Exchange</span></span>|
|<span data-ttu-id="8f9ff-120">ブロック</span><span class="sxs-lookup"><span data-stu-id="8f9ff-120">blocked</span></span>|<span data-ttu-id="8f9ff-121">1/3</span><span class="sxs-lookup"><span data-stu-id="8f9ff-121">3</span></span>|<span data-ttu-id="8f9ff-122">Exchange でデバイスがブロックされている</span><span class="sxs-lookup"><span data-stu-id="8f9ff-122">Device is Blocked in Exchange</span></span>|
|<span data-ttu-id="8f9ff-123">隔離</span><span class="sxs-lookup"><span data-stu-id="8f9ff-123">quarantined</span></span>|<span data-ttu-id="8f9ff-124">2/4</span><span class="sxs-lookup"><span data-stu-id="8f9ff-124">4</span></span>|<span data-ttu-id="8f9ff-125">Exchange でのデバイスの検疫</span><span class="sxs-lookup"><span data-stu-id="8f9ff-125">Device is Quarantined in Exchange</span></span>|




