---
title: deviceManagementSettingDependency リソースの種類
description: 設定の依存関係情報
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 100a6d441e161c353425f2d890e9468ebb32f3e8
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36364664"
---
# <a name="devicemanagementsettingdependency-resource-type"></a>deviceManagementSettingDependency リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

設定の依存関係情報

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|definitionId|String|設定の設定定義 ID が依存している|
|式|[Devicemanagementconstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)コレクション|依存関係設定値の制約のコレクション|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingDependency"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingDependency",
  "definitionId": "String",
  "constraints": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingXmlConstraint"
    }
  ]
}
```



