---
title: sharedPCAccountManagerPolicy リソース タイプ
description: 共有 PC アカウント マネージャー ポリシーです。 アカウント マネージャーが有効になっている場合にのみ適用されます。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3d6b7e0ab86af78380f85da8ec37c643e662838c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410995"
---
# <a name="sharedpcaccountmanagerpolicy-resource-type"></a><span data-ttu-id="5bbcc-104">sharedPCAccountManagerPolicy リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="5bbcc-104">sharedPCAccountManagerPolicy resource type</span></span>

> <span data-ttu-id="5bbcc-105">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5bbcc-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5bbcc-106">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5bbcc-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5bbcc-107">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="5bbcc-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5bbcc-108">共有 PC アカウント マネージャー ポリシーです。</span><span class="sxs-lookup"><span data-stu-id="5bbcc-108">SharedPC Account Manager Policy.</span></span> <span data-ttu-id="5bbcc-109">アカウント マネージャーが有効になっている場合にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="5bbcc-109">Only applies when the account manager is enabled.</span></span>

## <a name="properties"></a><span data-ttu-id="5bbcc-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5bbcc-110">Properties</span></span>
|<span data-ttu-id="5bbcc-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5bbcc-111">Property</span></span>|<span data-ttu-id="5bbcc-112">型</span><span class="sxs-lookup"><span data-stu-id="5bbcc-112">Type</span></span>|<span data-ttu-id="5bbcc-113">説明</span><span class="sxs-lookup"><span data-stu-id="5bbcc-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5bbcc-114">accountDeletionPolicy</span><span class="sxs-lookup"><span data-stu-id="5bbcc-114">accountDeletionPolicy</span></span>|[<span data-ttu-id="5bbcc-115">sharedPCAccountDeletionPolicyType</span><span class="sxs-lookup"><span data-stu-id="5bbcc-115">sharedPCAccountDeletionPolicyType</span></span>](../resources/intune-deviceconfig-sharedpcaccountdeletionpolicytype.md)|<span data-ttu-id="5bbcc-116">アカウントがいつ削除されるかを構成します。</span><span class="sxs-lookup"><span data-stu-id="5bbcc-116">Configures when accounts are deleted.</span></span> <span data-ttu-id="5bbcc-117">可能な値は、`immediate`、`diskSpaceThreshold`、`diskSpaceThresholdOrInactiveThreshold` です。</span><span class="sxs-lookup"><span data-stu-id="5bbcc-117">Possible values are: `immediate`, `diskSpaceThreshold`, `diskSpaceThresholdOrInactiveThreshold`.</span></span>|
|<span data-ttu-id="5bbcc-118">cacheAccountsAboveDiskFreePercentage</span><span class="sxs-lookup"><span data-stu-id="5bbcc-118">cacheAccountsAboveDiskFreePercentage</span></span>|<span data-ttu-id="5bbcc-119">Int32</span><span class="sxs-lookup"><span data-stu-id="5bbcc-119">Int32</span></span>|<span data-ttu-id="5bbcc-120">キャッシュされている共有 PC アカウントの削除が停止される前に、PC に必要な使用可能なディスク領域の割合を設定します。</span><span class="sxs-lookup"><span data-stu-id="5bbcc-120">Sets the percentage of available disk space a PC should have before it stops deleting cached shared PC accounts.</span></span> <span data-ttu-id="5bbcc-121">AccountDeletionPolicy が DiskSpaceThreshold または DiskSpaceThresholdOrInactiveThreshold の場合にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="5bbcc-121">Only applies when AccountDeletionPolicy is DiskSpaceThreshold or DiskSpaceThresholdOrInactiveThreshold.</span></span> <span data-ttu-id="5bbcc-122">有効な値は 0 から 100 までです</span><span class="sxs-lookup"><span data-stu-id="5bbcc-122">Valid values 0 to 100</span></span>|
|<span data-ttu-id="5bbcc-123">inactiveThresholdDays</span><span class="sxs-lookup"><span data-stu-id="5bbcc-123">inactiveThresholdDays</span></span>|<span data-ttu-id="5bbcc-124">Int32</span><span class="sxs-lookup"><span data-stu-id="5bbcc-124">Int32</span></span>|<span data-ttu-id="5bbcc-125">指定した期間にわたってログオンしていない場合にアカウントの削除が始まるタイミングを日数で指定します。</span><span class="sxs-lookup"><span data-stu-id="5bbcc-125">Specifies when the accounts will start being deleted when they have not been logged on during the specified period, given as number of days.</span></span> <span data-ttu-id="5bbcc-126">AccountDeletionPolicy が DiskSpaceThreshold または DiskSpaceThresholdOrInactiveThreshold の場合にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="5bbcc-126">Only applies when AccountDeletionPolicy is DiskSpaceThreshold or DiskSpaceThresholdOrInactiveThreshold.</span></span>|
|<span data-ttu-id="5bbcc-127">removeAccountsBelowDiskFreePercentage</span><span class="sxs-lookup"><span data-stu-id="5bbcc-127">removeAccountsBelowDiskFreePercentage</span></span>|<span data-ttu-id="5bbcc-128">Int32</span><span class="sxs-lookup"><span data-stu-id="5bbcc-128">Int32</span></span>|<span data-ttu-id="5bbcc-129">キャッシュ済みのアカウントを削除してディスク領域を空ける前に、PC に残っているディスク領域の割合を設定します。</span><span class="sxs-lookup"><span data-stu-id="5bbcc-129">Sets the percentage of disk space remaining on a PC before cached accounts will be deleted to free disk space.</span></span> <span data-ttu-id="5bbcc-130">非アクティブの状態が最長のアカウントから削除されます。</span><span class="sxs-lookup"><span data-stu-id="5bbcc-130">Accounts that have been inactive the longest will be deleted first.</span></span> <span data-ttu-id="5bbcc-131">AccountDeletionPolicy が DiskSpaceThresholdOrInactiveThreshold の場合にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="5bbcc-131">Only applies when AccountDeletionPolicy is DiskSpaceThresholdOrInactiveThreshold.</span></span> <span data-ttu-id="5bbcc-132">有効な値は 0 から 100 までです</span><span class="sxs-lookup"><span data-stu-id="5bbcc-132">Valid values 0 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="5bbcc-133">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5bbcc-133">Relationships</span></span>
<span data-ttu-id="5bbcc-134">なし</span><span class="sxs-lookup"><span data-stu-id="5bbcc-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5bbcc-135">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5bbcc-135">JSON Representation</span></span>
<span data-ttu-id="5bbcc-136">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5bbcc-136">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharedPCAccountManagerPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sharedPCAccountManagerPolicy",
  "accountDeletionPolicy": "String",
  "cacheAccountsAboveDiskFreePercentage": 1024,
  "inactiveThresholdDays": 1024,
  "removeAccountsBelowDiskFreePercentage": 1024
}
```




