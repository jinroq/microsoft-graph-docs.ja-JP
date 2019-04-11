---
title: devicemanagementexchangeaccesslevel 列挙型
description: Exchange のアクセスレベル。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c235d31e97b570f70145884349eaef6e2254194c
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31802465"
---
# <a name="devicemanagementexchangeaccesslevel-enum-type"></a><span data-ttu-id="73cbe-103">devicemanagementexchangeaccesslevel 列挙型</span><span class="sxs-lookup"><span data-stu-id="73cbe-103">deviceManagementExchangeAccessLevel enum type</span></span>

> <span data-ttu-id="73cbe-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="73cbe-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="73cbe-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="73cbe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73cbe-106">Exchange のアクセスレベル。</span><span class="sxs-lookup"><span data-stu-id="73cbe-106">Access Level in Exchange.</span></span>

## <a name="members"></a><span data-ttu-id="73cbe-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="73cbe-107">Members</span></span>
|<span data-ttu-id="73cbe-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="73cbe-108">Member</span></span>|<span data-ttu-id="73cbe-109">値</span><span class="sxs-lookup"><span data-stu-id="73cbe-109">Value</span></span>|<span data-ttu-id="73cbe-110">説明</span><span class="sxs-lookup"><span data-stu-id="73cbe-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73cbe-111">none</span><span class="sxs-lookup"><span data-stu-id="73cbe-111">none</span></span>|<span data-ttu-id="73cbe-112">.0</span><span class="sxs-lookup"><span data-stu-id="73cbe-112">0</span></span>|<span data-ttu-id="73cbe-113">Exchange でデバイスアクセスルールが構成されていません。</span><span class="sxs-lookup"><span data-stu-id="73cbe-113">No device access rule has been configured in Exchange.</span></span>|
|<span data-ttu-id="73cbe-114">使う</span><span class="sxs-lookup"><span data-stu-id="73cbe-114">allow</span></span>|<span data-ttu-id="73cbe-115">1-d</span><span class="sxs-lookup"><span data-stu-id="73cbe-115">1</span></span>|<span data-ttu-id="73cbe-116">デバイスへのアクセスを Exchange に許可します。</span><span class="sxs-lookup"><span data-stu-id="73cbe-116">Allow the device access to Exchange.</span></span>|
|<span data-ttu-id="73cbe-117">拒否</span><span class="sxs-lookup"><span data-stu-id="73cbe-117">block</span></span>|<span data-ttu-id="73cbe-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="73cbe-118">2</span></span>|<span data-ttu-id="73cbe-119">デバイスによる Exchange へのアクセスをブロックします。</span><span class="sxs-lookup"><span data-stu-id="73cbe-119">Block the device from accessing Exchange.</span></span>|
|<span data-ttu-id="73cbe-120">済み</span><span class="sxs-lookup"><span data-stu-id="73cbe-120">quarantine</span></span>|<span data-ttu-id="73cbe-121">1/3</span><span class="sxs-lookup"><span data-stu-id="73cbe-121">3</span></span>|<span data-ttu-id="73cbe-122">Exchange でデバイスを検疫します。</span><span class="sxs-lookup"><span data-stu-id="73cbe-122">Quarantine the device in Exchange.</span></span>|





