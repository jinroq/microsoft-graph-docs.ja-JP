---
title: devicemanagementexchangeaccesslevel 列挙型
description: Exchange のアクセスレベル。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c235d31e97b570f70145884349eaef6e2254194c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566627"
---
# <a name="devicemanagementexchangeaccesslevel-enum-type"></a><span data-ttu-id="f3153-103">devicemanagementexchangeaccesslevel 列挙型</span><span class="sxs-lookup"><span data-stu-id="f3153-103">deviceManagementExchangeAccessLevel enum type</span></span>

> <span data-ttu-id="f3153-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f3153-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3153-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f3153-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3153-106">Exchange のアクセスレベル。</span><span class="sxs-lookup"><span data-stu-id="f3153-106">Access Level in Exchange.</span></span>

## <a name="members"></a><span data-ttu-id="f3153-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="f3153-107">Members</span></span>
|<span data-ttu-id="f3153-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="f3153-108">Member</span></span>|<span data-ttu-id="f3153-109">値</span><span class="sxs-lookup"><span data-stu-id="f3153-109">Value</span></span>|<span data-ttu-id="f3153-110">説明</span><span class="sxs-lookup"><span data-stu-id="f3153-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3153-111">なし</span><span class="sxs-lookup"><span data-stu-id="f3153-111">none</span></span>|<span data-ttu-id="f3153-112">.0</span><span class="sxs-lookup"><span data-stu-id="f3153-112">0</span></span>|<span data-ttu-id="f3153-113">Exchange でデバイスアクセスルールが構成されていません。</span><span class="sxs-lookup"><span data-stu-id="f3153-113">No device access rule has been configured in Exchange.</span></span>|
|<span data-ttu-id="f3153-114">使う</span><span class="sxs-lookup"><span data-stu-id="f3153-114">allow</span></span>|<span data-ttu-id="f3153-115">1 </span><span class="sxs-lookup"><span data-stu-id="f3153-115">1</span></span>|<span data-ttu-id="f3153-116">デバイスへのアクセスを Exchange に許可します。</span><span class="sxs-lookup"><span data-stu-id="f3153-116">Allow the device access to Exchange.</span></span>|
|<span data-ttu-id="f3153-117">拒否</span><span class="sxs-lookup"><span data-stu-id="f3153-117">block</span></span>|<span data-ttu-id="f3153-118">2 </span><span class="sxs-lookup"><span data-stu-id="f3153-118">2</span></span>|<span data-ttu-id="f3153-119">デバイスによる Exchange へのアクセスをブロックします。</span><span class="sxs-lookup"><span data-stu-id="f3153-119">Block the device from accessing Exchange.</span></span>|
|<span data-ttu-id="f3153-120">済み</span><span class="sxs-lookup"><span data-stu-id="f3153-120">quarantine</span></span>|<span data-ttu-id="f3153-121">3 </span><span class="sxs-lookup"><span data-stu-id="f3153-121">3</span></span>|<span data-ttu-id="f3153-122">Exchange でデバイスを検疫します。</span><span class="sxs-lookup"><span data-stu-id="f3153-122">Quarantine the device in Exchange.</span></span>|





