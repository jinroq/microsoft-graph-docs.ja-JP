---
title: variableManagementConditionExpression リソースの種類
description: 管理条件の状態をブール式として評価します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 39ca9ae676afa5e7bf39af8ebe936d3df0acd162
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34990079"
---
# <a name="variablemanagementconditionexpression-resource-type"></a>variableManagementConditionExpression リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

管理条件の状態をブール式として評価します。


[Managementconditionexpression モデル](../resources/intune-fencing-managementconditionexpressionmodel.md)から継承します

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|managementConditionId|String|式の評価に使用される管理条件 id。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.variableManagementConditionExpression"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.variableManagementConditionExpression",
  "managementConditionId": "String"
}
```





