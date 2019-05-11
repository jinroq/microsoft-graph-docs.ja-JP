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
# <a name="devicemanagementenumconstraint-resource-type"></a>deviceManagementEnumConstraint リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

設定値を適用する制約が、許可された文字列のセットを超えている


[Devicemanagementconstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)から継承します

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|values|[Devicemanagementenumvalue](../resources/intune-deviceintent-devicemanagementenumvalue.md)コレクション|この文字列の有効な値のリスト|

## <a name="relationships"></a>関係
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




