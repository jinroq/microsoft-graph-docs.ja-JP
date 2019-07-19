---
title: deviceManagementEnumConstraint リソースの種類
description: 設定値を適用する制約が、許可された文字列のセットを超えている
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 64c07f663d034cf6fa758155294730015ca6e3b4
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34964102"
---
# <a name="devicemanagementenumconstraint-resource-type"></a><span data-ttu-id="09695-103">deviceManagementEnumConstraint リソースの種類</span><span class="sxs-lookup"><span data-stu-id="09695-103">deviceManagementEnumConstraint resource type</span></span>

> <span data-ttu-id="09695-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="09695-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="09695-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="09695-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09695-106">設定値を適用する制約が、許可された文字列のセットを超えている</span><span class="sxs-lookup"><span data-stu-id="09695-106">Constraint that enforces the setting value is from a permitted set of strings</span></span>


<span data-ttu-id="09695-107">[Devicemanagementconstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="09695-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="09695-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="09695-108">Properties</span></span>
|<span data-ttu-id="09695-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="09695-109">Property</span></span>|<span data-ttu-id="09695-110">型</span><span class="sxs-lookup"><span data-stu-id="09695-110">Type</span></span>|<span data-ttu-id="09695-111">説明</span><span class="sxs-lookup"><span data-stu-id="09695-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09695-112">values</span><span class="sxs-lookup"><span data-stu-id="09695-112">values</span></span>|<span data-ttu-id="09695-113">[Devicemanagementenumvalue](../resources/intune-deviceintent-devicemanagementenumvalue.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="09695-113">[deviceManagementEnumValue](../resources/intune-deviceintent-devicemanagementenumvalue.md) collection</span></span>|<span data-ttu-id="09695-114">この文字列の有効な値のリスト</span><span class="sxs-lookup"><span data-stu-id="09695-114">List of valid values for this string</span></span>|

## <a name="relationships"></a><span data-ttu-id="09695-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="09695-115">Relationships</span></span>
<span data-ttu-id="09695-116">なし</span><span class="sxs-lookup"><span data-stu-id="09695-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="09695-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="09695-117">JSON Representation</span></span>
<span data-ttu-id="09695-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="09695-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementEnumConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementEnumConstraint",
  "values": [
    {
      "@odata.type": "microsoft.graph.deviceManagementEnumValue",
      "value": "String",
      "displayName": "String"
    }
  ]
}
```





