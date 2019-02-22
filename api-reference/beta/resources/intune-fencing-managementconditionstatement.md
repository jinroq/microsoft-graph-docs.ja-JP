---
title: managementconditionstatement リソースの種類
description: 管理条件ステートメントは、含まれている管理条件がすべて満たされたときに、デバイス/アプリケーション構成を有効/無効にする管理条件のグループです。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 41b696ee92b3098ea06c55c923fb3058706414ce
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30167474"
---
# <a name="managementconditionstatement-resource-type"></a>managementconditionstatement リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

管理条件ステートメントは、含まれている管理条件がすべて満たされたときに、デバイス/アプリケーション構成を有効/無効にする管理条件のグループです。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[managementconditionstatements を一覧表示する](../api/intune-fencing-managementconditionstatement-list.md)|[managementconditionstatement](../resources/intune-fencing-managementconditionstatement.md)コレクション|[managementconditionstatement](../resources/intune-fencing-managementconditionstatement.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[managementconditionstatement の取得](../api/intune-fencing-managementconditionstatement-get.md)|[managementconditionstatement](../resources/intune-fencing-managementconditionstatement.md)|[managementconditionstatement](../resources/intune-fencing-managementconditionstatement.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[managementconditionstatement の作成](../api/intune-fencing-managementconditionstatement-create.md)|[managementconditionstatement](../resources/intune-fencing-managementconditionstatement.md)|新しい[managementconditionstatement](../resources/intune-fencing-managementconditionstatement.md)オブジェクトを作成します。|
|[managementconditionstatement の削除](../api/intune-fencing-managementconditionstatement-delete.md)|なし|[managementconditionstatement](../resources/intune-fencing-managementconditionstatement.md)を削除します。|
|[managementconditionstatement の更新](../api/intune-fencing-managementconditionstatement-update.md)|[managementconditionstatement](../resources/intune-fencing-managementconditionstatement.md)|[managementconditionstatement](../resources/intune-fencing-managementconditionstatement.md)オブジェクトのプロパティを更新します。|
|[getManagementConditionStatementExpressionString 関数](../api/intune-fencing-managementconditionstatement-getmanagementconditionstatementexpressionstring.md)|[managementcondition式文字列](../resources/intune-fencing-managementconditionexpressionstring.md)|まだ文書化されていません|
|[getManagementConditionStatementsForPlatform 関数](../api/intune-fencing-managementconditionstatement-getmanagementconditionstatementsforplatform.md)|[managementconditionstatement](../resources/intune-fencing-managementconditionstatement.md)コレクション|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|管理条件ステートメントの一意識別子。 作成時に割り当てられたシステム生成値。|
|displayName|String|管理条件ステートメントの管理者定義の名前。|
|説明|String|管理条件ステートメントの管理者定義の説明。|
|createdDateTime|DateTimeOffset|管理条件ステートメントが作成された時刻。 サービス側を生成しました。|
|変更された日時|DateTimeOffset|管理条件ステートメントが最後に変更された時刻。 サービス側を更新しました。|
|式|[managementconditionexpression](../resources/intune-fencing-managementconditionexpression.md)|管理条件ステートメントがアクティブ化/非アクティブ化されたかどうかを評価するために使用される管理条件ステートメント式。|
|eTag|String|管理条件ステートメントの ETag。 サービス側を更新しました。|
|アプリケーションのプラットフォーム|[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)コレクション|この管理条件ステートメントの適用可能なプラットフォーム。
これは、管理条件ステートメントに関連付けられている管理条件を参照して、適用可能なプラットフォームの共通部分を検索することによって計算されます。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|managementconditions|[managementcondition](../resources/intune-fencing-managementcondition.md)コレクション|管理条件ステートメントに関連付けられている管理条件。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managementConditionStatement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managementConditionStatement",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "expression": {
    "@odata.type": "microsoft.graph.managementConditionExpression"
  },
  "eTag": "String",
  "applicablePlatforms": [
    "String"
  ]
}
```




