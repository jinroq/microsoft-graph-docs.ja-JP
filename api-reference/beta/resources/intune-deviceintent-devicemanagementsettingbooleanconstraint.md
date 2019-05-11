---
title: deviceManagementSettingBooleanConstraint リソースの種類
description: 制約によって特定のブール値が適用されます。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ba1b40d5481e6fc239aeea46a859d6d4a88294f2
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943440"
---
# <a name="devicemanagementsettingbooleanconstraint-resource-type"></a>deviceManagementSettingBooleanConstraint リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

制約によって特定のブール値が適用されます。


[Devicemanagementconstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)から継承します

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|value|ブール型 (Boolean)|比較するブール値|

## <a name="relationships"></a>関係
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingBooleanConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingBooleanConstraint",
  "value": true
}
```




