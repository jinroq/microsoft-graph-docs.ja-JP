---
title: sharedPCAccountManagerPolicy リソース タイプ
description: 共有 PC アカウント マネージャー ポリシーです。 アカウント マネージャーが有効になっている場合にのみ適用されます。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 42b8824f3f9b18722f69db4f3d0d116b2f46dfd2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914886"
---
# <a name="sharedpcaccountmanagerpolicy-resource-type"></a><span data-ttu-id="cfa5e-104">sharedPCAccountManagerPolicy リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="cfa5e-104">sharedPCAccountManagerPolicy resource type</span></span>

> <span data-ttu-id="cfa5e-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="cfa5e-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cfa5e-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cfa5e-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cfa5e-107">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="cfa5e-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cfa5e-108">共有 PC アカウント マネージャー ポリシーです。</span><span class="sxs-lookup"><span data-stu-id="cfa5e-108">SharedPC Account Manager Policy.</span></span> <span data-ttu-id="cfa5e-109">アカウント マネージャーが有効になっている場合にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="cfa5e-109">Only applies when the account manager is enabled.</span></span>
## <a name="properties"></a><span data-ttu-id="cfa5e-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cfa5e-110">Properties</span></span>
|<span data-ttu-id="cfa5e-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cfa5e-111">Property</span></span>|<span data-ttu-id="cfa5e-112">種類</span><span class="sxs-lookup"><span data-stu-id="cfa5e-112">Type</span></span>|<span data-ttu-id="cfa5e-113">説明</span><span class="sxs-lookup"><span data-stu-id="cfa5e-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cfa5e-114">accountDeletionPolicy</span><span class="sxs-lookup"><span data-stu-id="cfa5e-114">accountDeletionPolicy</span></span>|[<span data-ttu-id="cfa5e-115">sharedPCAccountDeletionPolicyType</span><span class="sxs-lookup"><span data-stu-id="cfa5e-115">sharedPCAccountDeletionPolicyType</span></span>](../resources/intune-deviceconfig-sharedpcaccountdeletionpolicytype.md)|<span data-ttu-id="cfa5e-116">アカウントがいつ削除されるかを構成します。</span><span class="sxs-lookup"><span data-stu-id="cfa5e-116">Configures when accounts are deleted.</span></span> <span data-ttu-id="cfa5e-117">可能な値は、`immediate`、`diskSpaceThreshold`、`diskSpaceThresholdOrInactiveThreshold` です。</span><span class="sxs-lookup"><span data-stu-id="cfa5e-117">Possible values are: `immediate`, `diskSpaceThreshold`, `diskSpaceThresholdOrInactiveThreshold`.</span></span>|
|<span data-ttu-id="cfa5e-118">cacheAccountsAboveDiskFreePercentage</span><span class="sxs-lookup"><span data-stu-id="cfa5e-118">cacheAccountsAboveDiskFreePercentage</span></span>|<span data-ttu-id="cfa5e-119">Int32</span><span class="sxs-lookup"><span data-stu-id="cfa5e-119">Int32</span></span>|<span data-ttu-id="cfa5e-120">キャッシュされている共有 PC アカウントの削除が停止される前に、PC に必要な使用可能なディスク領域の割合を設定します。</span><span class="sxs-lookup"><span data-stu-id="cfa5e-120">Sets the percentage of available disk space a PC should have before it stops deleting cached shared PC accounts.</span></span> <span data-ttu-id="cfa5e-121">AccountDeletionPolicy が DiskSpaceThreshold または DiskSpaceThresholdOrInactiveThreshold の場合にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="cfa5e-121">Only applies when AccountDeletionPolicy is DiskSpaceThreshold or DiskSpaceThresholdOrInactiveThreshold.</span></span> <span data-ttu-id="cfa5e-122">有効な値は 0 から 100 までです</span><span class="sxs-lookup"><span data-stu-id="cfa5e-122">Valid values 0 to 100</span></span>|
|<span data-ttu-id="cfa5e-123">inactiveThresholdDays</span><span class="sxs-lookup"><span data-stu-id="cfa5e-123">inactiveThresholdDays</span></span>|<span data-ttu-id="cfa5e-124">Int32</span><span class="sxs-lookup"><span data-stu-id="cfa5e-124">Int32</span></span>|<span data-ttu-id="cfa5e-125">指定した期間にわたってログオンしていない場合にアカウントの削除が始まるタイミングを日数で指定します。</span><span class="sxs-lookup"><span data-stu-id="cfa5e-125">Specifies when the accounts will start being deleted when they have not been logged on during the specified period, given as number of days.</span></span> <span data-ttu-id="cfa5e-126">AccountDeletionPolicy が DiskSpaceThreshold または DiskSpaceThresholdOrInactiveThreshold の場合にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="cfa5e-126">Only applies when AccountDeletionPolicy is DiskSpaceThreshold or DiskSpaceThresholdOrInactiveThreshold.</span></span>|
|<span data-ttu-id="cfa5e-127">removeAccountsBelowDiskFreePercentage</span><span class="sxs-lookup"><span data-stu-id="cfa5e-127">removeAccountsBelowDiskFreePercentage</span></span>|<span data-ttu-id="cfa5e-128">Int32</span><span class="sxs-lookup"><span data-stu-id="cfa5e-128">Int32</span></span>|<span data-ttu-id="cfa5e-129">キャッシュ済みのアカウントを削除してディスク領域を空ける前に、PC に残っているディスク領域の割合を設定します。</span><span class="sxs-lookup"><span data-stu-id="cfa5e-129">Sets the percentage of disk space remaining on a PC before cached accounts will be deleted to free disk space.</span></span> <span data-ttu-id="cfa5e-130">非アクティブの状態が最長のアカウントから削除されます。</span><span class="sxs-lookup"><span data-stu-id="cfa5e-130">Accounts that have been inactive the longest will be deleted first.</span></span> <span data-ttu-id="cfa5e-131">AccountDeletionPolicy が DiskSpaceThresholdOrInactiveThreshold の場合にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="cfa5e-131">Only applies when AccountDeletionPolicy is DiskSpaceThresholdOrInactiveThreshold.</span></span> <span data-ttu-id="cfa5e-132">有効な値は 0 から 100 までです</span><span class="sxs-lookup"><span data-stu-id="cfa5e-132">Valid values 0 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="cfa5e-133">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="cfa5e-133">Relationships</span></span>
<span data-ttu-id="cfa5e-134">なし</span><span class="sxs-lookup"><span data-stu-id="cfa5e-134">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="cfa5e-135">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cfa5e-135">JSON Representation</span></span>
<span data-ttu-id="cfa5e-136">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="cfa5e-136">Here is a JSON representation of the resource.</span></span>
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





