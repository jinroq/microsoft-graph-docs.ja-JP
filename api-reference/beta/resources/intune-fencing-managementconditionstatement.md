---
title: managementConditionStatement リソースの種類
description: 管理条件ステートメントは、含まれている管理条件がすべて満たされたときに、デバイス/アプリケーション構成を有効/無効にする管理条件のグループです。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 37718b5efaa34680f3b990fe61421d0faf24dac5
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34979173"
---
# <a name="managementconditionstatement-resource-type"></a>managementConditionStatement リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

管理条件ステートメントは、含まれている管理条件がすべて満たされたときに、デバイス/アプリケーション構成を有効/無効にする管理条件のグループです。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[ManagementConditionStatements を一覧表示する](../api/intune-fencing-managementconditionstatement-list.md)|[Managementconditionstatement](../resources/intune-fencing-managementconditionstatement.md)コレクション|[Managementconditionstatement](../resources/intune-fencing-managementconditionstatement.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[ManagementConditionStatement の取得](../api/intune-fencing-managementconditionstatement-get.md)|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)|[Managementconditionstatement](../resources/intune-fencing-managementconditionstatement.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[ManagementConditionStatement の作成](../api/intune-fencing-managementconditionstatement-create.md)|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)|新しい[Managementconditionstatement](../resources/intune-fencing-managementconditionstatement.md)オブジェクトを作成します。|
|[ManagementConditionStatement の削除](../api/intune-fencing-managementconditionstatement-delete.md)|None|[Managementconditionstatement](../resources/intune-fencing-managementconditionstatement.md)を削除します。|
|[ManagementConditionStatement の更新](../api/intune-fencing-managementconditionstatement-update.md)|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)|[Managementconditionstatement](../resources/intune-fencing-managementconditionstatement.md)オブジェクトのプロパティを更新します。|
|[getManagementConditionStatementExpressionString 関数](../api/intune-fencing-managementconditionstatement-getmanagementconditionstatementexpressionstring.md)|[Managementcondition式文字列](../resources/intune-fencing-managementconditionexpressionstring.md)|まだ文書化されていません|
|[getManagementConditionStatementsForPlatform 関数](../api/intune-fencing-managementconditionstatement-getmanagementconditionstatementsforplatform.md)|[Managementconditionstatement](../resources/intune-fencing-managementconditionstatement.md)コレクション|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|管理条件ステートメントの一意識別子。 作成時に割り当てられたシステム生成値。|
|displayName|String|管理条件ステートメントの管理者定義の名前。|
|description|String|管理条件ステートメントの管理者定義の説明。|
|createdDateTime|DateTimeOffset|管理条件ステートメントが作成された時刻。 サービス側を生成しました。|
|modifiedDateTime|DateTimeOffset|管理条件ステートメントが最後に変更された時刻。 サービス側を更新しました。|
|式|[managementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)|管理条件ステートメントがアクティブ化/非アクティブ化されたかどうかを評価するために使用される管理条件ステートメント式。|
|eTag|String|管理条件ステートメントの ETag。 サービス側を更新しました。|
|アプリケーションのプラットフォーム|[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)コレクション|この管理条件ステートメントの適用可能なプラットフォーム。
これは、管理条件ステートメントに関連付けられている管理条件を参照して、適用可能なプラットフォームの共通部分を検索することによって計算されます。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|managementConditions|[Managementcondition](../resources/intune-fencing-managementcondition.md)コレクション|管理条件ステートメントに関連付けられている管理条件。|

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





