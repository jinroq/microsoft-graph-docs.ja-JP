---
title: groupPolicyDefinitionValue リソースの種類
description: 定義値のエンティティは、1 つのグループ ポリシーの定義の値を格納します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b7e98a41409efba60ee1431fac82a49be2029039
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430510"
---
# <a name="grouppolicydefinitionvalue-resource-type"></a>groupPolicyDefinitionValue リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

定義値のエンティティは、1 つのグループ ポリシーの定義の値を格納します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト groupPolicyDefinitionValues](../api/intune-grouppolicy-grouppolicydefinitionvalue-list.md)|[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)コレクション|[GroupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)オブジェクトのプロパティと関係を一覧表示します。|
|[GroupPolicyDefinitionValue を取得します。](../api/intune-grouppolicy-grouppolicydefinitionvalue-get.md)|[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|[GroupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)オブジェクトのプロパティと関係を参照してください。|
|[GroupPolicyDefinitionValue を作成します。](../api/intune-grouppolicy-grouppolicydefinitionvalue-create.md)|[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|新しい[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)オブジェクトを作成します。|
|[GroupPolicyDefinitionValue を削除します。](../api/intune-grouppolicy-grouppolicydefinitionvalue-delete.md)|なし|の[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)を削除します。|
|[GroupPolicyDefinitionValue を更新します。](../api/intune-grouppolicy-grouppolicydefinitionvalue-update.md)|[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|[GroupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|日付と時刻オブジェクトを作成します。|
|enabled|Boolean|有効または、関連付けられているグループ ポリシーの定義を無効にします。|
|configurationType|[groupPolicyConfigurationType](../resources/intune-grouppolicy-grouppolicyconfigurationtype.md)|値を構成する方法を指定します。 ポリシーとして、または環境設定のいずれかを指定できます。 使用可能な値は、`policy`、`preference` です。|
|id|String|エンティティのキー。|
|lastModifiedDateTime|DateTimeOffset|日付と時刻、エンティティが最後に修正されました。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|presentationValues|[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)コレクション|定義の値に関連付けられたグループ ポリシー プレゼンテーション値です。|
|definition|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|値に関連付けられているグループ ポリシーの定義です。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyDefinitionValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionValue",
  "createdDateTime": "String (timestamp)",
  "enabled": true,
  "configurationType": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```




