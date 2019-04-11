---
title: sharedPCAccountManagerPolicy リソース タイプ
description: 共有 PC アカウント マネージャー ポリシーです。 アカウント マネージャーが有効になっている場合にのみ適用されます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5d81a3fdf14daf71d70b013bb10a5d1fdba825aa
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31771111"
---
# <a name="sharedpcaccountmanagerpolicy-resource-type"></a><span data-ttu-id="fe5ce-104">sharedPCAccountManagerPolicy リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="fe5ce-104">sharedPCAccountManagerPolicy resource type</span></span>

> <span data-ttu-id="fe5ce-105">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fe5ce-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fe5ce-106">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="fe5ce-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe5ce-107">共有 PC アカウント マネージャー ポリシーです。</span><span class="sxs-lookup"><span data-stu-id="fe5ce-107">SharedPC Account Manager Policy.</span></span> <span data-ttu-id="fe5ce-108">アカウント マネージャーが有効になっている場合にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="fe5ce-108">Only applies when the account manager is enabled.</span></span>

## <a name="properties"></a><span data-ttu-id="fe5ce-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fe5ce-109">Properties</span></span>
|<span data-ttu-id="fe5ce-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fe5ce-110">Property</span></span>|<span data-ttu-id="fe5ce-111">型</span><span class="sxs-lookup"><span data-stu-id="fe5ce-111">Type</span></span>|<span data-ttu-id="fe5ce-112">説明</span><span class="sxs-lookup"><span data-stu-id="fe5ce-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe5ce-113">accountDeletionPolicy</span><span class="sxs-lookup"><span data-stu-id="fe5ce-113">accountDeletionPolicy</span></span>|[<span data-ttu-id="fe5ce-114">sharedPCAccountDeletionPolicyType</span><span class="sxs-lookup"><span data-stu-id="fe5ce-114">sharedPCAccountDeletionPolicyType</span></span>](../resources/intune-deviceconfig-sharedpcaccountdeletionpolicytype.md)|<span data-ttu-id="fe5ce-115">アカウントがいつ削除されるかを構成します。</span><span class="sxs-lookup"><span data-stu-id="fe5ce-115">Configures when accounts are deleted.</span></span> <span data-ttu-id="fe5ce-116">可能な値は、`immediate`、`diskSpaceThreshold`、`diskSpaceThresholdOrInactiveThreshold` です。</span><span class="sxs-lookup"><span data-stu-id="fe5ce-116">Possible values are: `immediate`, `diskSpaceThreshold`, `diskSpaceThresholdOrInactiveThreshold`.</span></span>|
|<span data-ttu-id="fe5ce-117">cacheAccountsAboveDiskFreePercentage</span><span class="sxs-lookup"><span data-stu-id="fe5ce-117">cacheAccountsAboveDiskFreePercentage</span></span>|<span data-ttu-id="fe5ce-118">Int32</span><span class="sxs-lookup"><span data-stu-id="fe5ce-118">Int32</span></span>|<span data-ttu-id="fe5ce-119">キャッシュされている共有 PC アカウントの削除が停止される前に、PC に必要な使用可能なディスク領域の割合を設定します。</span><span class="sxs-lookup"><span data-stu-id="fe5ce-119">Sets the percentage of available disk space a PC should have before it stops deleting cached shared PC accounts.</span></span> <span data-ttu-id="fe5ce-120">AccountDeletionPolicy が DiskSpaceThreshold または DiskSpaceThresholdOrInactiveThreshold の場合にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="fe5ce-120">Only applies when AccountDeletionPolicy is DiskSpaceThreshold or DiskSpaceThresholdOrInactiveThreshold.</span></span> <span data-ttu-id="fe5ce-121">有効な値は 0 から 100 までです</span><span class="sxs-lookup"><span data-stu-id="fe5ce-121">Valid values 0 to 100</span></span>|
|<span data-ttu-id="fe5ce-122">inactiveThresholdDays</span><span class="sxs-lookup"><span data-stu-id="fe5ce-122">inactiveThresholdDays</span></span>|<span data-ttu-id="fe5ce-123">Int32</span><span class="sxs-lookup"><span data-stu-id="fe5ce-123">Int32</span></span>|<span data-ttu-id="fe5ce-124">指定した期間にわたってログオンしていない場合にアカウントの削除が始まるタイミングを日数で指定します。</span><span class="sxs-lookup"><span data-stu-id="fe5ce-124">Specifies when the accounts will start being deleted when they have not been logged on during the specified period, given as number of days.</span></span> <span data-ttu-id="fe5ce-125">AccountDeletionPolicy が DiskSpaceThreshold または DiskSpaceThresholdOrInactiveThreshold の場合にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="fe5ce-125">Only applies when AccountDeletionPolicy is DiskSpaceThreshold or DiskSpaceThresholdOrInactiveThreshold.</span></span>|
|<span data-ttu-id="fe5ce-126">removeAccountsBelowDiskFreePercentage</span><span class="sxs-lookup"><span data-stu-id="fe5ce-126">removeAccountsBelowDiskFreePercentage</span></span>|<span data-ttu-id="fe5ce-127">Int32</span><span class="sxs-lookup"><span data-stu-id="fe5ce-127">Int32</span></span>|<span data-ttu-id="fe5ce-128">キャッシュ済みのアカウントを削除してディスク領域を空ける前に、PC に残っているディスク領域の割合を設定します。</span><span class="sxs-lookup"><span data-stu-id="fe5ce-128">Sets the percentage of disk space remaining on a PC before cached accounts will be deleted to free disk space.</span></span> <span data-ttu-id="fe5ce-129">非アクティブの状態が最長のアカウントから削除されます。</span><span class="sxs-lookup"><span data-stu-id="fe5ce-129">Accounts that have been inactive the longest will be deleted first.</span></span> <span data-ttu-id="fe5ce-130">AccountDeletionPolicy が DiskSpaceThresholdOrInactiveThreshold の場合にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="fe5ce-130">Only applies when AccountDeletionPolicy is DiskSpaceThresholdOrInactiveThreshold.</span></span> <span data-ttu-id="fe5ce-131">有効な値は 0 から 100 までです</span><span class="sxs-lookup"><span data-stu-id="fe5ce-131">Valid values 0 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="fe5ce-132">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fe5ce-132">Relationships</span></span>
<span data-ttu-id="fe5ce-133">なし</span><span class="sxs-lookup"><span data-stu-id="fe5ce-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fe5ce-134">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fe5ce-134">JSON Representation</span></span>
<span data-ttu-id="fe5ce-135">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="fe5ce-135">Here is a JSON representation of the resource.</span></span>
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





