---
title: groupPolicyConfiguration リソースの種類
description: グループ ポリシーの構成エンティティには、1 つまたは複数のグループ ポリシーの定義の設定値が含まれています。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: be3b43ab0e9e3f87f53ed0dae144f2b6f4dce7b7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431665"
---
# <a name="grouppolicyconfiguration-resource-type"></a>groupPolicyConfiguration リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

グループ ポリシーの構成エンティティには、1 つまたは複数のグループ ポリシーの定義の設定値が含まれています。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト groupPolicyConfigurations](../api/intune-grouppolicy-grouppolicyconfiguration-list.md)|[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)コレクション|[GroupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)オブジェクトのプロパティと関係を一覧表示します。|
|[GroupPolicyConfiguration を取得します。](../api/intune-grouppolicy-grouppolicyconfiguration-get.md)|[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|[GroupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)オブジェクトのプロパティと関係を参照してください。|
|[GroupPolicyConfiguration を作成します。](../api/intune-grouppolicy-grouppolicyconfiguration-create.md)|[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|新しい[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)オブジェクトを作成します。|
|[GroupPolicyConfiguration を削除します。](../api/intune-grouppolicy-grouppolicyconfiguration-delete.md)|なし|の[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)を削除します。|
|[GroupPolicyConfiguration を更新します。](../api/intune-grouppolicy-grouppolicyconfiguration-update.md)|[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|[GroupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)オブジェクトのプロパティを更新します。|
|[assign action](../api/intune-grouppolicy-grouppolicyconfiguration-assign.md)|[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)コレクション|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|日付と時刻オブジェクトを作成します。|
|displayName|String|リソース オブジェクトの名前をユーザーに提供されます。|
|説明|String|ユーザーは、リソース オブジェクトの説明を提供します。|
|id|String|エンティティのキー。|
|lastModifiedDateTime|DateTimeOffset|日付と時刻、エンティティが最後に修正されました。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|definitionValues|[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)コレクション|一覧は、有効または、構成のグループ ポリシーの定義の値を無効にします。|
|assignments|[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)コレクション|構成のグループの割り当ての一覧です。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyConfiguration",
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "description": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```




