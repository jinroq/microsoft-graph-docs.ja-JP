---
title: devicemanagementenumconstraint リソースの種類
description: 設定値を適用する制約が、許可された文字列のセットを超えている
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 457582a5160aa9e17beb06d3b169c3817d216e4e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523302"
---
# <a name="devicemanagementenumconstraint-resource-type"></a><span data-ttu-id="4c377-103">devicemanagementenumconstraint リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4c377-103">deviceManagementEnumConstraint resource type</span></span>

> <span data-ttu-id="4c377-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4c377-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4c377-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4c377-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4c377-106">設定値を適用する制約が、許可された文字列のセットを超えている</span><span class="sxs-lookup"><span data-stu-id="4c377-106">Constraint that enforces the setting value is from a permitted set of strings</span></span>


<span data-ttu-id="4c377-107">[devicemanagementconstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="4c377-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4c377-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4c377-108">Properties</span></span>
|<span data-ttu-id="4c377-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4c377-109">Property</span></span>|<span data-ttu-id="4c377-110">型</span><span class="sxs-lookup"><span data-stu-id="4c377-110">Type</span></span>|<span data-ttu-id="4c377-111">説明</span><span class="sxs-lookup"><span data-stu-id="4c377-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c377-112">values</span><span class="sxs-lookup"><span data-stu-id="4c377-112">values</span></span>|<span data-ttu-id="4c377-113">[devicemanagementenumvalue](../resources/intune-deviceintent-devicemanagementenumvalue.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="4c377-113">[deviceManagementEnumValue](../resources/intune-deviceintent-devicemanagementenumvalue.md) collection</span></span>|<span data-ttu-id="4c377-114">この文字列の有効な値のリスト</span><span class="sxs-lookup"><span data-stu-id="4c377-114">List of valid values for this string</span></span>|

## <a name="relationships"></a><span data-ttu-id="4c377-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4c377-115">Relationships</span></span>
<span data-ttu-id="4c377-116">なし</span><span class="sxs-lookup"><span data-stu-id="4c377-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4c377-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4c377-117">JSON Representation</span></span>
<span data-ttu-id="4c377-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4c377-118">Here is a JSON representation of the resource.</span></span>
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





