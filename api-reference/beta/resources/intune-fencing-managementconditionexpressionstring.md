---
title: managementConditionExpressionString リソースの種類
description: 管理条件の式の文字列は、管理条件式の文字列表現です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8b8abc3492690afe6709070decbfe050356fd614
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419192"
---
# <a name="managementconditionexpressionstring-resource-type"></a>managementConditionExpressionString リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

管理条件の式の文字列は、管理条件式の文字列表現です。


[ManagementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)から継承します。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|value|文字列|管理条件ステートメント式の文字列値。|

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




