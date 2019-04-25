---
title: grouppolicypresentationvalue リソースの種類
description: 単一のグループポリシープレゼンテーションの値を格納する基本のプレゼンテーション値エンティティ。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8d4f3d1493e85708335797252301b451f5e41520
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32575850"
---
# <a name="grouppolicypresentationvalue-resource-type"></a>grouppolicypresentationvalue リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

単一のグループポリシープレゼンテーションの値を格納する基本のプレゼンテーション値エンティティ。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[grouppolicypresentationvalues を一覧表示する](../api/intune-grouppolicy-grouppolicypresentationvalue-list.md)|[grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)コレクション|[grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[grouppolicypresentationvalue の取得](../api/intune-grouppolicy-grouppolicypresentationvalue-get.md)|[grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|[grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[grouppolicypresentationvalue の作成](../api/intune-grouppolicy-grouppolicypresentationvalue-create.md)|[grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|新しい[grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)オブジェクトを作成します。|
|[grouppolicypresentationvalue の削除](../api/intune-grouppolicy-grouppolicypresentationvalue-delete.md)|なし|[grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)を削除します。|
|[grouppolicypresentationvalue の更新](../api/intune-grouppolicy-grouppolicypresentationvalue-update.md)|[grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|[grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|lastModifiedDateTime|DateTimeOffset|オブジェクトが最後に変更された日付と時刻。|
|createdDateTime|DateTimeOffset|オブジェクトが作成された日付と時刻。|
|id|String|エンティティのキー。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|definitionvalue|[grouppolicydefinitionvalue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|プレゼンテーション値に関連付けられているグループポリシー定義の値。|
|プレゼンテーション|[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|プレゼンテーション値に関連付けられたグループポリシーのプレゼンテーション。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValue",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)"
}
```





