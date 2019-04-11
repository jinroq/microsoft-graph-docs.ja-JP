---
title: managementcondition式 string リソースの種類
description: 管理条件式文字列は、管理条件式の文字列表現です。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f3dac405c71e4e85cc29bb36d335a57bb51fbe0f
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31783739"
---
# <a name="managementconditionexpressionstring-resource-type"></a>managementcondition式 string リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

管理条件式文字列は、管理条件式の文字列表現です。


[managementconditionexpression](../resources/intune-fencing-managementconditionexpression.md)から継承します

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|value|文字列型 (String)|管理条件ステートメントの式文字列値。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managementConditionExpressionString"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managementConditionExpressionString",
  "value": "String"
}
```





