---
title: Devicemanagementsetting整数制約リソースの種類
description: 整数設定に許可されている値の範囲を適用する制約
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c58572b1fb30a3270b58070f917c90a38a4ddd72
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943418"
---
# <a name="devicemanagementsettingintegerconstraint-resource-type"></a>Devicemanagementsetting整数制約リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

整数設定に許可されている値の範囲を適用する制約


[Devicemanagementconstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)から継承します

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|minimumValue|Int32|許可される最小値|
|maximumValue|Int32|許可される最大値|

## <a name="relationships"></a>関係
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingIntegerConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingIntegerConstraint",
  "minimumValue": 1024,
  "maximumValue": 1024
}
```




