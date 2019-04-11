---
title: deliveryOptimizationGroupIdSourceOptions リソースの種類
description: グループ id オプションの種類
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0cd541fd9ff3a91f40be1b6ccea67787cdad2567
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31784867"
---
# <a name="deliveryoptimizationgroupidsourceoptions-resource-type"></a><span data-ttu-id="231a8-103">deliveryOptimizationGroupIdSourceOptions リソースの種類</span><span class="sxs-lookup"><span data-stu-id="231a8-103">deliveryOptimizationGroupIdSourceOptions resource type</span></span>

> <span data-ttu-id="231a8-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="231a8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="231a8-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="231a8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="231a8-106">グループ id オプションの種類</span><span class="sxs-lookup"><span data-stu-id="231a8-106">Group id options type</span></span>


<span data-ttu-id="231a8-107">[deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="231a8-107">Inherits from [deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span></span>

## <a name="properties"></a><span data-ttu-id="231a8-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="231a8-108">Properties</span></span>
|<span data-ttu-id="231a8-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="231a8-109">Property</span></span>|<span data-ttu-id="231a8-110">型</span><span class="sxs-lookup"><span data-stu-id="231a8-110">Type</span></span>|<span data-ttu-id="231a8-111">説明</span><span class="sxs-lookup"><span data-stu-id="231a8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="231a8-112">groupidsourceoption</span><span class="sxs-lookup"><span data-stu-id="231a8-112">groupIdSourceOption</span></span>|[<span data-ttu-id="231a8-113">deliveryOptimizationGroupIdOptionsType</span><span class="sxs-lookup"><span data-stu-id="231a8-113">deliveryOptimizationGroupIdOptionsType</span></span>](../resources/intune-deviceconfig-deliveryoptimizationgroupidoptionstype.md)|<span data-ttu-id="231a8-114">このポリシーを設定すると、ピアの選択が特定のソースに制限されます。</span><span class="sxs-lookup"><span data-stu-id="231a8-114">Set this policy to restrict peer selection to a specific source.</span></span> <span data-ttu-id="231a8-115">可能な値は、`notConfigured`、`adSite`、`authenticatedDomainSid`、`dhcpUserOption`、`dnsSuffix` です。</span><span class="sxs-lookup"><span data-stu-id="231a8-115">Possible values are: `notConfigured`, `adSite`, `authenticatedDomainSid`, `dhcpUserOption`, `dnsSuffix`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="231a8-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="231a8-116">Relationships</span></span>
<span data-ttu-id="231a8-117">なし</span><span class="sxs-lookup"><span data-stu-id="231a8-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="231a8-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="231a8-118">JSON Representation</span></span>
<span data-ttu-id="231a8-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="231a8-119">Here is a JSON representation of the resource.</span></span>
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





