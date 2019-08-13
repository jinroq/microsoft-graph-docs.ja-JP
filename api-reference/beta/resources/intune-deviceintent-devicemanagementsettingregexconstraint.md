---
title: deviceManagementSettingRegexConstraint リソースの種類
description: 指定された RegEx パターンに対して設定の一致を強制する制約
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d0f9a04583bfb9b28546e9057f0530f72558a0be
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36364636"
---
# <a name="devicemanagementsettingregexconstraint-resource-type"></a>deviceManagementSettingRegexConstraint リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

指定された RegEx パターンに対して設定の一致を強制する制約


[Devicemanagementconstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)から継承します

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|pcre|String|照合する正規表現パターン|

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



