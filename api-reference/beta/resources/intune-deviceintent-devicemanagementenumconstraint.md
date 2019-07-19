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
# <a name="devicemanagementenumconstraint-resource-type"></a>deviceManagementEnumConstraint リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

設定値を適用する制約が、許可された文字列のセットを超えている


[Devicemanagementconstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)から継承します

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|values|[Devicemanagementenumvalue](../resources/intune-deviceintent-devicemanagementenumvalue.md)コレクション|この文字列の有効な値のリスト|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
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





