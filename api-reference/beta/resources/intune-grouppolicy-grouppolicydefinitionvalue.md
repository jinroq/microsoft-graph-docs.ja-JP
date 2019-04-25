---
title: grouppolicydefinitionvalue リソースの種類
description: 定義値エンティティは、1つのグループポリシー定義の値を格納します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2aa0eef1b4921d1b364486b9af254fba2a8322c0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32575808"
---
# <a name="grouppolicydefinitionvalue-resource-type"></a>grouppolicydefinitionvalue リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

定義値エンティティは、1つのグループポリシー定義の値を格納します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[grouppolicydefinitionvalues のリスト](../api/intune-grouppolicy-grouppolicydefinitionvalue-list.md)|[grouppolicydefinitionvalue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)コレクション|[grouppolicydefinitionvalue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[grouppolicydefinitionvalue の取得](../api/intune-grouppolicy-grouppolicydefinitionvalue-get.md)|[grouppolicydefinitionvalue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|[grouppolicydefinitionvalue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[grouppolicydefinitionvalue の作成](../api/intune-grouppolicy-grouppolicydefinitionvalue-create.md)|[grouppolicydefinitionvalue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|新しい[grouppolicydefinitionvalue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)オブジェクトを作成します。|
|[grouppolicydefinitionvalue の削除](../api/intune-grouppolicy-grouppolicydefinitionvalue-delete.md)|なし|[grouppolicydefinitionvalue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)を削除します。|
|[grouppolicydefinitionvalue の更新](../api/intune-grouppolicy-grouppolicydefinitionvalue-update.md)|[grouppolicydefinitionvalue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|[grouppolicydefinitionvalue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|オブジェクトが作成された日付と時刻。|
|enabled|ブール型 (Boolean)|関連付けられたグループポリシー定義を有効または無効にします。|
|configurationType|[groupPolicyConfigurationType](../resources/intune-grouppolicy-grouppolicyconfigurationtype.md)|値の構成方法を指定します。 これは、ポリシーとして、または設定することができます。 可能な値は、`policy`、`preference` です。|
|id|String|エンティティのキー。|
|lastModifiedDateTime|DateTimeOffset|エンティティが最後に変更された日付と時刻。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|プレゼンテーションの値|[grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)コレクション|関連付けられたグループポリシーの値が定義値と共に表示されます。|
|definition|[grouppolicydefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|関連付けられたグループポリシー定義の値を指定します。|

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





