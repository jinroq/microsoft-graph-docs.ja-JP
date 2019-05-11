---
title: deviceManagementEnumConstraint リソースの種類
description: 設定値を適用する制約が、許可された文字列のセットを超えている
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2979f189921c0c9e7240cc5287a072b27e12b96e
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943432"
---
# <a name="devicemanagementenumconstraint-resource-type"></a><span data-ttu-id="34a85-103">deviceManagementEnumConstraint リソースの種類</span><span class="sxs-lookup"><span data-stu-id="34a85-103">deviceManagementEnumConstraint resource type</span></span>

> <span data-ttu-id="34a85-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="34a85-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="34a85-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="34a85-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34a85-106">設定値を適用する制約が、許可された文字列のセットを超えている</span><span class="sxs-lookup"><span data-stu-id="34a85-106">Constraint that enforces the setting value is from a permitted set of strings</span></span>


<span data-ttu-id="34a85-107">[Devicemanagementconstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="34a85-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="34a85-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="34a85-108">Properties</span></span>
|<span data-ttu-id="34a85-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="34a85-109">Property</span></span>|<span data-ttu-id="34a85-110">型</span><span class="sxs-lookup"><span data-stu-id="34a85-110">Type</span></span>|<span data-ttu-id="34a85-111">説明</span><span class="sxs-lookup"><span data-stu-id="34a85-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34a85-112">values</span><span class="sxs-lookup"><span data-stu-id="34a85-112">values</span></span>|<span data-ttu-id="34a85-113">[Devicemanagementenumvalue](../resources/intune-deviceintent-devicemanagementenumvalue.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="34a85-113">[deviceManagementEnumValue](../resources/intune-deviceintent-devicemanagementenumvalue.md) collection</span></span>|<span data-ttu-id="34a85-114">この文字列の有効な値のリスト</span><span class="sxs-lookup"><span data-stu-id="34a85-114">List of valid values for this string</span></span>|

## <a name="relationships"></a><span data-ttu-id="34a85-115">関係</span><span class="sxs-lookup"><span data-stu-id="34a85-115">Relationships</span></span>
<span data-ttu-id="34a85-116">なし</span><span class="sxs-lookup"><span data-stu-id="34a85-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="34a85-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="34a85-117">JSON Representation</span></span>
<span data-ttu-id="34a85-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="34a85-118">Here is a JSON representation of the resource.</span></span>
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




