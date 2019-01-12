---
title: locationManagementCondition リソースの種類
description: 場所の管理条件を監視するのには、興味のあるエリアを定義する情報が含まれています。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 541cf74decad641f6dc7751945e1d0ffceee1366
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27922978"
---
# <a name="locationmanagementcondition-resource-type"></a>locationManagementCondition リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

場所の管理条件を監視するのには、興味のあるエリアを定義する情報が含まれています。

[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト locationManagementConditions](../api/intune-fencing-locationmanagementcondition-list.md)|[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md)コレクション|[LocationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md)オブジェクトのプロパティと関係を一覧表示します。|
|[LocationManagementCondition を取得します。](../api/intune-fencing-locationmanagementcondition-get.md)|[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md)|[LocationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md)オブジェクトのプロパティと関係を参照してください。|

## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|ID|String|管理条件の一意の識別子です。 システムでは、作成時に割り当てられた値が生成されます。 [ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。|
|一意な名前|String|管理条件の一意の名前です。 管理条件式で使用されます。 [ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。|
|displayName|String|管理者は、管理の条件の名前を定義します。 [ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。|
|説明|String|管理者は、管理状態の説明を定義します。 [ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。|
|createdDateTime|DateTimeOffset|管理条件が作成された時刻。 サービス側が生成されます。 [ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。|
|変更された日時|DateTimeOffset|管理条件が最後に修正された時間です。 サービス側を更新します。 [ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。|
|eTag|String|管理条件の ETag。 サービス側を更新します。 [ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。|
|applicablePlatforms|[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)コレクション|この管理条件に該当するプラットフォームです。 [ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|managementConditionStatements|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)コレクション|管理条件に関連付けられている管理の条件ステートメントです。 [ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.locationManagementCondition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.locationManagementCondition",
  "id": "String (identifier)",
  "uniqueName": "String",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "eTag": "String",
  "applicablePlatforms": [
    "String"
  ]
}
```





