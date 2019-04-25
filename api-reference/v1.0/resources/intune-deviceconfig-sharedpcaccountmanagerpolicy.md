---
title: sharedPCAccountManagerPolicy リソース タイプ
description: 共有 PC アカウント マネージャー ポリシーです。 アカウント マネージャーが有効になっている場合にのみ適用されます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 683915fdf1a0878e72229ed98cca457fbf77082d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534613"
---
# <a name="sharedpcaccountmanagerpolicy-resource-type"></a><span data-ttu-id="0e4cd-104">sharedPCAccountManagerPolicy リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="0e4cd-104">sharedPCAccountManagerPolicy resource type</span></span>

> <span data-ttu-id="0e4cd-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0e4cd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e4cd-106">共有 PC アカウント マネージャー ポリシーです。</span><span class="sxs-lookup"><span data-stu-id="0e4cd-106">SharedPC Account Manager Policy.</span></span> <span data-ttu-id="0e4cd-107">アカウント マネージャーが有効になっている場合にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="0e4cd-107">Only applies when the account manager is enabled.</span></span>

## <a name="properties"></a><span data-ttu-id="0e4cd-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0e4cd-108">Properties</span></span>
|<span data-ttu-id="0e4cd-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0e4cd-109">Property</span></span>|<span data-ttu-id="0e4cd-110">型</span><span class="sxs-lookup"><span data-stu-id="0e4cd-110">Type</span></span>|<span data-ttu-id="0e4cd-111">説明</span><span class="sxs-lookup"><span data-stu-id="0e4cd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e4cd-112">accountDeletionPolicy</span><span class="sxs-lookup"><span data-stu-id="0e4cd-112">accountDeletionPolicy</span></span>|[<span data-ttu-id="0e4cd-113">sharedPCAccountDeletionPolicyType</span><span class="sxs-lookup"><span data-stu-id="0e4cd-113">sharedPCAccountDeletionPolicyType</span></span>](../resources/intune-deviceconfig-sharedpcaccountdeletionpolicytype.md)|<span data-ttu-id="0e4cd-114">アカウントがいつ削除されるかを構成します。</span><span class="sxs-lookup"><span data-stu-id="0e4cd-114">Configures when accounts are deleted.</span></span> <span data-ttu-id="0e4cd-115">可能な値は、`immediate`、`diskSpaceThreshold`、`diskSpaceThresholdOrInactiveThreshold` です。</span><span class="sxs-lookup"><span data-stu-id="0e4cd-115">Possible values are: `immediate`, `diskSpaceThreshold`, `diskSpaceThresholdOrInactiveThreshold`.</span></span>|
|<span data-ttu-id="0e4cd-116">cacheAccountsAboveDiskFreePercentage</span><span class="sxs-lookup"><span data-stu-id="0e4cd-116">cacheAccountsAboveDiskFreePercentage</span></span>|<span data-ttu-id="0e4cd-117">Int32</span><span class="sxs-lookup"><span data-stu-id="0e4cd-117">Int32</span></span>|<span data-ttu-id="0e4cd-118">キャッシュされている共有 PC アカウントの削除が停止される前に、PC に必要な使用可能なディスク領域の割合を設定します。</span><span class="sxs-lookup"><span data-stu-id="0e4cd-118">Sets the percentage of available disk space a PC should have before it stops deleting cached shared PC accounts.</span></span> <span data-ttu-id="0e4cd-119">AccountDeletionPolicy が DiskSpaceThreshold または DiskSpaceThresholdOrInactiveThreshold の場合にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="0e4cd-119">Only applies when AccountDeletionPolicy is DiskSpaceThreshold or DiskSpaceThresholdOrInactiveThreshold.</span></span> <span data-ttu-id="0e4cd-120">有効な値は 0 から 100 までです</span><span class="sxs-lookup"><span data-stu-id="0e4cd-120">Valid values 0 to 100</span></span>|
|<span data-ttu-id="0e4cd-121">inactiveThresholdDays</span><span class="sxs-lookup"><span data-stu-id="0e4cd-121">inactiveThresholdDays</span></span>|<span data-ttu-id="0e4cd-122">Int32</span><span class="sxs-lookup"><span data-stu-id="0e4cd-122">Int32</span></span>|<span data-ttu-id="0e4cd-123">指定した期間にわたってログオンしていない場合にアカウントの削除が始まるタイミングを日数で指定します。</span><span class="sxs-lookup"><span data-stu-id="0e4cd-123">Specifies when the accounts will start being deleted when they have not been logged on during the specified period, given as number of days.</span></span> <span data-ttu-id="0e4cd-124">AccountDeletionPolicy が DiskSpaceThreshold または DiskSpaceThresholdOrInactiveThreshold の場合にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="0e4cd-124">Only applies when AccountDeletionPolicy is DiskSpaceThreshold or DiskSpaceThresholdOrInactiveThreshold.</span></span>|
|<span data-ttu-id="0e4cd-125">removeAccountsBelowDiskFreePercentage</span><span class="sxs-lookup"><span data-stu-id="0e4cd-125">removeAccountsBelowDiskFreePercentage</span></span>|<span data-ttu-id="0e4cd-126">Int32</span><span class="sxs-lookup"><span data-stu-id="0e4cd-126">Int32</span></span>|<span data-ttu-id="0e4cd-127">キャッシュ済みのアカウントを削除してディスク領域を空ける前に、PC に残っているディスク領域の割合を設定します。</span><span class="sxs-lookup"><span data-stu-id="0e4cd-127">Sets the percentage of disk space remaining on a PC before cached accounts will be deleted to free disk space.</span></span> <span data-ttu-id="0e4cd-128">非アクティブの状態が最長のアカウントから削除されます。</span><span class="sxs-lookup"><span data-stu-id="0e4cd-128">Accounts that have been inactive the longest will be deleted first.</span></span> <span data-ttu-id="0e4cd-129">AccountDeletionPolicy が DiskSpaceThresholdOrInactiveThreshold の場合にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="0e4cd-129">Only applies when AccountDeletionPolicy is DiskSpaceThresholdOrInactiveThreshold.</span></span> <span data-ttu-id="0e4cd-130">有効な値は 0 から 100 までです</span><span class="sxs-lookup"><span data-stu-id="0e4cd-130">Valid values 0 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="0e4cd-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0e4cd-131">Relationships</span></span>
<span data-ttu-id="0e4cd-132">なし</span><span class="sxs-lookup"><span data-stu-id="0e4cd-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0e4cd-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0e4cd-133">JSON Representation</span></span>
<span data-ttu-id="0e4cd-134">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0e4cd-134">Here is a JSON representation of the resource.</span></span>
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



