---
title: devicemanagementenumconstraint リソースの種類
description: 設定値を適用する制約が、許可された文字列のセットを超えている
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 71af621a27830695bf4638715573299a163fda58
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/08/2019
ms.locfileid: "31523680"
---
# <a name="devicemanagementenumconstraint-resource-type"></a>devicemanagementenumconstraint リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

設定値を適用する制約が、許可された文字列のセットを超えている


[devicemanagementconstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)から継承します

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|values|[devicemanagementenumvalue](../resources/intune-deviceintent-devicemanagementenumvalue.md)コレクション|この文字列の有効な値のリスト|

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







