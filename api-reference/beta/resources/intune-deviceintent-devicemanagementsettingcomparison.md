---
title: deviceManagementSettingComparison リソースの種類
description: 比較結果の設定を表すエンティティ
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f68ffd08945662fc291fb5489de67967d3cd1cbf
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "35002001"
---
# <a name="devicemanagementsettingcomparison-resource-type"></a>deviceManagementSettingComparison リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

比較結果の設定を表すエンティティ

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|設定 ID|
|displayName|String|設定の表示名|
|definitionId|String|このインスタンスの設定定義の ID|
|currentValueJson|String|現在のインテント (または) テンプレート設定の値の JSON 表現|
|newValueJson|String|新しいテンプレート設定の値の JSON 表記|
|comparisonResult|[deviceManagementComparisonResult](../resources/intune-deviceintent-devicemanagementcomparisonresult.md)|比較結果を設定します。 可能な値は、`unknown`、`equal`、`notEqual`、`added`、`removed` です。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingComparison"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingComparison",
  "id": "String (identifier)",
  "displayName": "String",
  "definitionId": "String",
  "currentValueJson": "String",
  "newValueJson": "String",
  "comparisonResult": "String"
}
```





