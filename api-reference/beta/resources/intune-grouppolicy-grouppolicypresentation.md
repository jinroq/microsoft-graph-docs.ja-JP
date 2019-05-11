---
title: groupPolicyPresentation リソースの種類
description: グループポリシー定義の追加オプションを表示するための基本エンティティ。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a8a1e4a615999a899712ad82d2177fbb862328c2
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941129"
---
# <a name="grouppolicypresentation-resource-type"></a>groupPolicyPresentation リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

グループポリシー定義の追加オプションを表示するための基本エンティティ。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[GroupPolicyPresentation を取得する](../api/intune-grouppolicy-grouppolicypresentation-get.md)|[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[GroupPolicyPresentation の更新](../api/intune-grouppolicy-grouppolicypresentation-update.md)|[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|label|String|任意のプレゼンテーションエンティティのローカライズされたテキストラベル。 既定値は空白です。|
|id|String|エンティティのキー。|
|lastModifiedDateTime|DateTimeOffset|エンティティが最後に変更された日付と時刻。|

## <a name="relationships"></a>関係
|リレーションシップ|型|説明|
|:---|:---|:---|
|definition|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|プレゼンテーションに関連付けられたグループポリシーの定義。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentation",
  "label": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```




