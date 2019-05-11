---
title: deviceManagementSettingDependency リソースの種類
description: 設定の依存関係情報
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3353ef63aab0336a42fad3ac500115adc70a4e24
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943327"
---
# <a name="devicemanagementsettingdependency-resource-type"></a>deviceManagementSettingDependency リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

設定の依存関係情報

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|definitionId|String|設定の設定定義 ID が依存している|
|式|[Devicemanagementconstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)コレクション|依存関係設定値の制約のコレクション|

## <a name="relationships"></a>関係
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingDependency"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingDependency",
  "definitionId": "String",
  "constraints": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingXmlConstraint"
    }
  ]
}
```




