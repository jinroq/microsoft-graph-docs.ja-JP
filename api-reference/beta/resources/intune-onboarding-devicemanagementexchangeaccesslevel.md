---
title: deviceManagementExchangeAccessLevel 列挙型
description: Exchange のアクセスレベル。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5b2c2c4e4a34a9a28dd10350bee592f9ba5dc63d
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34993117"
---
# <a name="devicemanagementexchangeaccesslevel-enum-type"></a><span data-ttu-id="a8594-103">deviceManagementExchangeAccessLevel 列挙型</span><span class="sxs-lookup"><span data-stu-id="a8594-103">deviceManagementExchangeAccessLevel enum type</span></span>

> <span data-ttu-id="a8594-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a8594-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a8594-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a8594-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8594-106">Exchange のアクセスレベル。</span><span class="sxs-lookup"><span data-stu-id="a8594-106">Access Level in Exchange.</span></span>

## <a name="members"></a><span data-ttu-id="a8594-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="a8594-107">Members</span></span>
|<span data-ttu-id="a8594-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="a8594-108">Member</span></span>|<span data-ttu-id="a8594-109">値</span><span class="sxs-lookup"><span data-stu-id="a8594-109">Value</span></span>|<span data-ttu-id="a8594-110">説明</span><span class="sxs-lookup"><span data-stu-id="a8594-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8594-111">none</span><span class="sxs-lookup"><span data-stu-id="a8594-111">none</span></span>|<span data-ttu-id="a8594-112">.0</span><span class="sxs-lookup"><span data-stu-id="a8594-112">0</span></span>|<span data-ttu-id="a8594-113">Exchange でデバイスアクセスルールが構成されていません。</span><span class="sxs-lookup"><span data-stu-id="a8594-113">No device access rule has been configured in Exchange.</span></span>|
|<span data-ttu-id="a8594-114">使う</span><span class="sxs-lookup"><span data-stu-id="a8594-114">allow</span></span>|<span data-ttu-id="a8594-115">1-d</span><span class="sxs-lookup"><span data-stu-id="a8594-115">1</span></span>|<span data-ttu-id="a8594-116">デバイスへのアクセスを Exchange に許可します。</span><span class="sxs-lookup"><span data-stu-id="a8594-116">Allow the device access to Exchange.</span></span>|
|<span data-ttu-id="a8594-117">拒否</span><span class="sxs-lookup"><span data-stu-id="a8594-117">block</span></span>|<span data-ttu-id="a8594-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="a8594-118">2</span></span>|<span data-ttu-id="a8594-119">デバイスによる Exchange へのアクセスをブロックします。</span><span class="sxs-lookup"><span data-stu-id="a8594-119">Block the device from accessing Exchange.</span></span>|
|<span data-ttu-id="a8594-120">済み</span><span class="sxs-lookup"><span data-stu-id="a8594-120">quarantine</span></span>|<span data-ttu-id="a8594-121">1/3</span><span class="sxs-lookup"><span data-stu-id="a8594-121">3</span></span>|<span data-ttu-id="a8594-122">Exchange でデバイスを検疫します。</span><span class="sxs-lookup"><span data-stu-id="a8594-122">Quarantine the device in Exchange.</span></span>|





