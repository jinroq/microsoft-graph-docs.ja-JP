---
title: devicemanagementenumvalue リソースの種類
description: 列挙値の定義情報
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: de1340223d45361825b2b8d8fc4e57194437f6b6
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/08/2019
ms.locfileid: "31523736"
---
# <a name="devicemanagementenumvalue-resource-type"></a>devicemanagementenumvalue リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

列挙値の定義情報

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|value|文字列型 (String)|生の列挙値のテキスト|
|displayName|String|この列挙値の表示名|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementEnumValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementEnumValue",
  "value": "String",
  "displayName": "String"
}
```







