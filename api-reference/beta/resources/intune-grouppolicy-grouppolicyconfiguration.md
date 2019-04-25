---
title: grouppolicyconfiguration リソースの種類
description: グループポリシー構成エンティティには、1つまたは複数のグループポリシー定義の構成済みの値が含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f9c925ba10b1dde26e51a64b912c33143d58def3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32564065"
---
# <a name="grouppolicyconfiguration-resource-type"></a>grouppolicyconfiguration リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

グループポリシー構成エンティティには、1つまたは複数のグループポリシー定義の構成済みの値が含まれています。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[grouppolicyconfigurations を一覧表示する](../api/intune-grouppolicy-grouppolicyconfiguration-list.md)|[grouppolicyconfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)コレクション|[grouppolicyconfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[grouppolicyconfiguration の取得](../api/intune-grouppolicy-grouppolicyconfiguration-get.md)|[grouppolicyconfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|[grouppolicyconfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[grouppolicyconfiguration の作成](../api/intune-grouppolicy-grouppolicyconfiguration-create.md)|[grouppolicyconfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|新しい[grouppolicyconfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)オブジェクトを作成します。|
|[grouppolicyconfiguration の削除](../api/intune-grouppolicy-grouppolicyconfiguration-delete.md)|なし|[grouppolicyconfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)を削除します。|
|[grouppolicyconfiguration を更新する](../api/intune-grouppolicy-grouppolicyconfiguration-update.md)|[grouppolicyconfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|[grouppolicyconfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)オブジェクトのプロパティを更新します。|
|[assign アクション](../api/intune-grouppolicy-grouppolicyconfiguration-assign.md)|[grouppolicyconfigurationassignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)コレクション|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|オブジェクトが作成された日付と時刻。|
|displayName|String|ユーザーが指定した resource オブジェクトの名前。|
|説明|String|ユーザーが指定した resource オブジェクトの説明。|
|id|String|エンティティのキー。|
|lastModifiedDateTime|DateTimeOffset|エンティティが最後に変更された日付と時刻。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|definitionvalues|[grouppolicydefinitionvalue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)コレクション|構成に対して有効または無効にされたグループポリシー定義の値のリスト。|
|assignments|[grouppolicyconfigurationassignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)コレクション|構成のグループの割り当てのリスト。|

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





