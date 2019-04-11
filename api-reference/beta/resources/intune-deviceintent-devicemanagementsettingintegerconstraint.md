---
title: devicemanagementsetting整数制約リソースの種類
description: 整数設定に許可されている値の範囲を適用する制約
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9bf28c3f3942e99841b43f1cd7ff5304fd81d800
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31781261"
---
# <a name="devicemanagementsettingintegerconstraint-resource-type"></a>devicemanagementsetting整数制約リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

整数設定に許可されている値の範囲を適用する制約


[devicemanagementconstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)から継承します

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|minimumvalue|Int32|許可される最小値|
|maximumValue|Int32|許可される最大値|

## <a name="relationships"></a>リレーションシップ
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





