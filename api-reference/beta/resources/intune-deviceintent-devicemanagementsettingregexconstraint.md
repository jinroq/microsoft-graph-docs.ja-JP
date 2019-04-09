---
title: deviceManagementSettingRegexConstraint リソースの種類
description: 指定された RegEx パターンに対して設定の一致を強制する制約
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 52369b5309768bd5530d176a7ccfbfabb1365b62
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/08/2019
ms.locfileid: "31522378"
---
# <a name="devicemanagementsettingregexconstraint-resource-type"></a>deviceManagementSettingRegexConstraint リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

指定された RegEx パターンに対して設定の一致を強制する制約


[devicemanagementconstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)から継承します

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|pcre|文字列|照合する正規表現パターン|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingRegexConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingRegexConstraint",
  "regex": "String"
}
```







