---
title: deliveryOptimizationGroupIdSourceOptions リソースの種類
description: グループ id オプションの種類
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fc2c900828526ac4d2788c2b91e669bae04f452f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35970746"
---
# <a name="deliveryoptimizationgroupidsourceoptions-resource-type"></a><span data-ttu-id="b31ef-103">deliveryOptimizationGroupIdSourceOptions リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b31ef-103">deliveryOptimizationGroupIdSourceOptions resource type</span></span>

> <span data-ttu-id="b31ef-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b31ef-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b31ef-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b31ef-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b31ef-106">グループ id オプションの種類</span><span class="sxs-lookup"><span data-stu-id="b31ef-106">Group id options type</span></span>


<span data-ttu-id="b31ef-107">[DeliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="b31ef-107">Inherits from [deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b31ef-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b31ef-108">Properties</span></span>
|<span data-ttu-id="b31ef-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b31ef-109">Property</span></span>|<span data-ttu-id="b31ef-110">型</span><span class="sxs-lookup"><span data-stu-id="b31ef-110">Type</span></span>|<span data-ttu-id="b31ef-111">説明</span><span class="sxs-lookup"><span data-stu-id="b31ef-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b31ef-112">groupIdSourceOption</span><span class="sxs-lookup"><span data-stu-id="b31ef-112">groupIdSourceOption</span></span>|[<span data-ttu-id="b31ef-113">deliveryOptimizationGroupIdOptionsType</span><span class="sxs-lookup"><span data-stu-id="b31ef-113">deliveryOptimizationGroupIdOptionsType</span></span>](../resources/intune-deviceconfig-deliveryoptimizationgroupidoptionstype.md)|<span data-ttu-id="b31ef-114">このポリシーを設定すると、ピアの選択が特定のソースに制限されます。</span><span class="sxs-lookup"><span data-stu-id="b31ef-114">Set this policy to restrict peer selection to a specific source.</span></span> <span data-ttu-id="b31ef-115">可能な値は、`notConfigured`、`adSite`、`authenticatedDomainSid`、`dhcpUserOption`、`dnsSuffix` です。</span><span class="sxs-lookup"><span data-stu-id="b31ef-115">Possible values are: `notConfigured`, `adSite`, `authenticatedDomainSid`, `dhcpUserOption`, `dnsSuffix`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b31ef-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b31ef-116">Relationships</span></span>
<span data-ttu-id="b31ef-117">なし</span><span class="sxs-lookup"><span data-stu-id="b31ef-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b31ef-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b31ef-118">JSON Representation</span></span>
<span data-ttu-id="b31ef-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b31ef-119">Here is a JSON representation of the resource.</span></span>
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





