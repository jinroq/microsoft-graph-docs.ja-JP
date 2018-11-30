---
title: circularGeofenceManagementCondition リソースの種類
description: Geo フェンス-循環管理の条件を監視するのには、興味のあるエリアを定義するための情報が含まれています。
ms.openlocfilehash: 0ae10d226b48772bb70e975496295afd2d67229d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070553"
---
# <a name="circulargeofencemanagementcondition-resource-type"></a>circularGeofenceManagementCondition リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Geo フェンス-循環管理の条件を監視するのには、興味のあるエリアを定義するための情報が含まれています。

[LocationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md)から継承します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト circularGeofenceManagementConditions](../api/intune-fencing-circulargeofencemanagementcondition-list.md)|[circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)コレクション|[CircularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)オブジェクトのプロパティと関係を一覧表示します。|
|[CircularGeofenceManagementCondition を取得します。](../api/intune-fencing-circulargeofencemanagementcondition-get.md)|[circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)|[CircularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)オブジェクトのプロパティと関係を参照してください。|
|[CircularGeofenceManagementCondition を作成します。](../api/intune-fencing-circulargeofencemanagementcondition-create.md)|[circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)|新しい[circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)オブジェクトを作成します。|
|[CircularGeofenceManagementCondition を削除します。](../api/intune-fencing-circulargeofencemanagementcondition-delete.md)|なし|の[circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)を削除します。|
|[CircularGeofenceManagementCondition を更新します。](../api/intune-fencing-circulargeofencemanagementcondition-update.md)|[circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)|[CircularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|管理条件の一意の識別子です。 システムでは、作成時に割り当てられた値が生成されます。 [ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。|
|一意な名前|String|管理条件の一意の名前です。 管理条件式で使用されます。 [ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。|
|displayName|String|管理者は、管理の条件の名前を定義します。 [ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。|
|説明|String|管理者は、管理状態の説明を定義します。 [ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。|
|createdDateTime|DateTimeOffset|管理条件が作成された時刻。 サービス側が生成されます。 [ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。|
|変更された日時|DateTimeOffset|管理条件が最後に修正された時間です。 サービス側を更新します。 [ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。|
|eTag|String|管理条件の ETag。 サービス側を更新します。 [ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。|
|applicablePlatforms|[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)コレクション|この管理条件に該当するプラットフォームです。 [ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。|
|latitude|倍精度浮動小数点数|度、-90 °、および包括的 +90 の間の緯度です。|
|longitude|倍精度浮動小数点数|-180 と包括的な +180 度の経度です。|
|radiusInMeters|単精度浮動小数点型 (Single)|メートル単位の半径です。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|managementConditionStatements|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)コレクション|管理条件に関連付けられている管理の条件ステートメントです。 [ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.circularGeofenceManagementCondition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.circularGeofenceManagementCondition",
  "id": "String (identifier)",
  "uniqueName": "String",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "eTag": "String",
  "applicablePlatforms": [
    "String"
  ],
  "latitude": "<Unknown Primitive Type Edm.Double>",
  "longitude": "<Unknown Primitive Type Edm.Double>",
  "radiusInMeters": "<Unknown Primitive Type Edm.Single>"
}
```





