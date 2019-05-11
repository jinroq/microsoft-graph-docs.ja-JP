---
title: deviceManagementEnumValue リソースの種類
description: 列挙値の定義情報
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 016c20153d7e4d9e970d5c10038aad4616a8e952
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943460"
---
# <a name="devicemanagementenumvalue-resource-type"></a>deviceManagementEnumValue リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

列挙値の定義情報

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|value|文字列型 (String)|生の列挙値のテキスト|
|displayName|String|この列挙値の表示名|

## <a name="relationships"></a>関係
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




