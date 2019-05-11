---
title: deliveryOptimizationGroupIdSourceOptions リソースの種類
description: グループ id オプションの種類
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8931c2e2a8a6dc3848b4ec73236443f9707aacea
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33947226"
---
# <a name="deliveryoptimizationgroupidsourceoptions-resource-type"></a><span data-ttu-id="65392-103">deliveryOptimizationGroupIdSourceOptions リソースの種類</span><span class="sxs-lookup"><span data-stu-id="65392-103">deliveryOptimizationGroupIdSourceOptions resource type</span></span>

> <span data-ttu-id="65392-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="65392-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="65392-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="65392-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65392-106">グループ id オプションの種類</span><span class="sxs-lookup"><span data-stu-id="65392-106">Group id options type</span></span>


<span data-ttu-id="65392-107">[DeliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="65392-107">Inherits from [deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span></span>

## <a name="properties"></a><span data-ttu-id="65392-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="65392-108">Properties</span></span>
|<span data-ttu-id="65392-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="65392-109">Property</span></span>|<span data-ttu-id="65392-110">型</span><span class="sxs-lookup"><span data-stu-id="65392-110">Type</span></span>|<span data-ttu-id="65392-111">説明</span><span class="sxs-lookup"><span data-stu-id="65392-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65392-112">groupIdSourceOption</span><span class="sxs-lookup"><span data-stu-id="65392-112">groupIdSourceOption</span></span>|[<span data-ttu-id="65392-113">deliveryOptimizationGroupIdOptionsType</span><span class="sxs-lookup"><span data-stu-id="65392-113">deliveryOptimizationGroupIdOptionsType</span></span>](../resources/intune-deviceconfig-deliveryoptimizationgroupidoptionstype.md)|<span data-ttu-id="65392-114">このポリシーを設定すると、ピアの選択が特定のソースに制限されます。</span><span class="sxs-lookup"><span data-stu-id="65392-114">Set this policy to restrict peer selection to a specific source.</span></span> <span data-ttu-id="65392-115">可能な値は、`notConfigured`、`adSite`、`authenticatedDomainSid`、`dhcpUserOption`、`dnsSuffix` です。</span><span class="sxs-lookup"><span data-stu-id="65392-115">Possible values are: `notConfigured`, `adSite`, `authenticatedDomainSid`, `dhcpUserOption`, `dnsSuffix`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="65392-116">関係</span><span class="sxs-lookup"><span data-stu-id="65392-116">Relationships</span></span>
<span data-ttu-id="65392-117">なし</span><span class="sxs-lookup"><span data-stu-id="65392-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="65392-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="65392-118">JSON Representation</span></span>
<span data-ttu-id="65392-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="65392-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationGroupIdSourceOptions"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationGroupIdSourceOptions",
  "groupIdSourceOption": "String"
}
```




