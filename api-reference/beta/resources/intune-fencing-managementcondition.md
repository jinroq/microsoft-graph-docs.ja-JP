---
title: managementCondition リソースの種類
description: 管理条件は、geo の囲いのように動的に発生することをイベントのタイム ・ フェンスとネットワーク フェンスです。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c41b4cb3143349ba0fdd97633a70ec7b38e266ec
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405857"
---
# <a name="managementcondition-resource-type"></a>managementCondition リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

管理条件は、geo の囲いのように動的に発生することをイベントのタイム ・ フェンスとネットワーク フェンスです。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト managementConditions](../api/intune-fencing-managementcondition-list.md)|[managementCondition](../resources/intune-fencing-managementcondition.md)コレクション|[ManagementCondition](../resources/intune-fencing-managementcondition.md)オブジェクトのプロパティと関係を一覧表示します。|
|[ManagementCondition を取得します。](../api/intune-fencing-managementcondition-get.md)|[managementCondition](../resources/intune-fencing-managementcondition.md)|[ManagementCondition](../resources/intune-fencing-managementcondition.md)オブジェクトのプロパティと関係を参照してください。|
|[getManagementConditionsForPlatform 関数](../api/intune-fencing-managementcondition-getmanagementconditionsforplatform.md)|[managementCondition](../resources/intune-fencing-managementcondition.md)コレクション|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|管理条件の一意の識別子です。 システムでは、作成時に割り当てられた値が生成されます。|
|一意な名前|String|管理条件の一意の名前です。 管理条件式で使用されます。|
|displayName|String|管理者は、管理の条件の名前を定義します。|
|説明|String|管理者は、管理状態の説明を定義します。|
|createdDateTime|DateTimeOffset|管理条件が作成された時刻。 サービス側が生成されます。|
|変更された日時|DateTimeOffset|管理条件が最後に修正された時間です。 サービス側を更新します。|
|eTag|String|管理条件の ETag。 サービス側を更新します。|
|applicablePlatforms|[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)コレクション|この管理条件に該当するプラットフォームです。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|managementConditionStatements|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)コレクション|管理条件に関連付けられている管理の条件ステートメントです。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managementCondition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managementCondition",
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




