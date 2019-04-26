---
title: auditResource リソースの種類
description: 監査のリソースのプロパティが含まれるクラス。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9e2a6b2309e831a872c4cde04a951819cac292ec
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534347"
---
# <a name="auditresource-resource-type"></a>auditResource リソースの種類

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

監査のリソースのプロパティが含まれるクラス。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|displayName|String|表示名。|
|modifiedProperties|[auditProperty](../resources/intune-auditing-auditproperty.md) コレクション|変更されたプロパティの一覧。|
|type|String|監査のリソースの種類。|
|resourceId|文字列型 (String)|監査のリソースの ID。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditResource"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditResource",
  "displayName": "String",
  "modifiedProperties": [
    {
      "@odata.type": "microsoft.graph.auditProperty",
      "displayName": "String",
      "oldValue": "String",
      "newValue": "String"
    }
  ],
  "type": "String",
  "resourceId": "String"
}
```



