---
title: Managementcondition式 String リソースの種類
description: 管理条件式文字列は、管理条件式の文字列表現です。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 510a12e38415b002e62c23891acf95cff7d6fd5a
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941269"
---
# <a name="managementconditionexpressionstring-resource-type"></a>Managementcondition式 String リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

管理条件式文字列は、管理条件式の文字列表現です。


[Managementconditionexpression](../resources/intune-fencing-managementconditionexpression.md)から継承します

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|value|文字列型 (String)|管理条件ステートメントの式文字列値。|

## <a name="relationships"></a>関係
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




