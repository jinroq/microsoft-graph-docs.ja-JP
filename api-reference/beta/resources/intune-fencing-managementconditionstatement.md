---
title: managementConditionStatement リソースの種類
description: 管理条件ステートメントは、管理の条件が含まれている管理のすべての条件が満たされたときにデバイスとアプリケーションの構成を有効または無効のグループです。
author: tfitzmac
ms.openlocfilehash: ca0966edd64166479361f42816e36fd278dbc6b1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27347678"
---
# <a name="managementconditionstatement-resource-type"></a>managementConditionStatement リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

管理条件ステートメントは、管理の条件が含まれている管理のすべての条件が満たされたときにデバイスとアプリケーションの構成を有効または無効のグループです。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト managementConditionStatements](../api/intune-fencing-managementconditionstatement-list.md)|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)コレクション|[ManagementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)オブジェクトのプロパティと関係を一覧表示します。|
|[ManagementConditionStatement を取得します。](../api/intune-fencing-managementconditionstatement-get.md)|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)|[ManagementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)オブジェクトのプロパティと関係を参照してください。|
|[ManagementConditionStatement を作成します。](../api/intune-fencing-managementconditionstatement-create.md)|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)|新しい[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)オブジェクトを作成します。|
|[ManagementConditionStatement を削除します。](../api/intune-fencing-managementconditionstatement-delete.md)|なし|の[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)を削除します。|
|[ManagementConditionStatement を更新します。](../api/intune-fencing-managementconditionstatement-update.md)|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)|[ManagementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)オブジェクトのプロパティを更新します。|
|[getManagementConditionStatementExpressionString 関数](../api/intune-fencing-managementconditionstatement-getmanagementconditionstatementexpressionstring.md)|[managementConditionExpressionString](../resources/intune-fencing-managementconditionexpressionstring.md)|まだ文書化されていません|
|[getManagementConditionStatementsForPlatform 関数](../api/intune-fencing-managementconditionstatement-getmanagementconditionstatementsforplatform.md)|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)コレクション|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|ID|String|管理条件付きステートメントの一意の識別子です。 システムでは、作成時に割り当てられた値が生成されます。|
|displayName|String|管理者は、管理条件ステートメントの名前を定義します。|
|説明|String|管理者は、管理条件付きステートメントの説明を定義します。|
|createdDateTime|DateTimeOffset|管理条件付きステートメントが作成された時刻。 サービス側が生成されます。|
|変更された日時|DateTimeOffset|管理条件付きステートメントが最後に修正された時間です。 サービス側を更新します。|
|式|[managementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)|場合は、管理条件ステートメントを評価するために使用、管理条件ステートメントの式は、アクティブ/非アクティブでした。|
|eTag|String|管理条件付きステートメントの ETag。 サービス側を更新します。|
|applicablePlatforms|[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)コレクション|この管理条件ステートメントに適用可能なプラットフォームです。
管理に関連付けられている管理の条件を見てからこの計算は、ステートメントと該当するプラットフォームの交点の検出の条件です。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|managementConditions|[managementCondition](../resources/intune-fencing-managementcondition.md)コレクション|管理条件ステートメントに関連付けられている管理の条件です。|

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





