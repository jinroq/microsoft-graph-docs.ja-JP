---
title: auditResource リソースの種類
description: 監査のリソースのプロパティが含まれるクラス。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ac7da99203631696b8c93fbde62db906143ffe38
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952245"
---
# <a name="auditresource-resource-type"></a>auditResource リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

監査のリソースのプロパティが含まれるクラス。
## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|displayName|文字列型 (String)|表示名。|
|modifiedProperties|[auditProperty](../resources/intune-auditing-auditproperty.md) コレクション|変更されたプロパティの一覧。|
|type|文字列型 (String)|監査のリソースの種類。|
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





