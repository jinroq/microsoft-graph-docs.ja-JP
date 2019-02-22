---
title: mobileAppProvisioningConfigGroupAssignment リソースの種類
description: アプリのプロビジョニング構成をグループに割り当てるために使用されるプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 884ddf889b755aa174a93e07584d39ff1d2a8ddf
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156239"
---
# <a name="mobileappprovisioningconfiggroupassignment-resource-type"></a>mobileAppProvisioningConfigGroupAssignment リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

アプリのプロビジョニング構成をグループに割り当てるために使用されるプロパティが含まれています。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト mobileAppProvisioningConfigGroupAssignments](../api/intune-apps-mobileappprovisioningconfiggroupassignment-list.md)|[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)コレクション|[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[mobileAppProvisioningConfigGroupAssignment を取得する](../api/intune-apps-mobileappprovisioningconfiggroupassignment-get.md)|[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)|[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[mobileAppProvisioningConfigGroupAssignment を作成する](../api/intune-apps-mobileappprovisioningconfiggroupassignment-create.md)|[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)|新しい[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)オブジェクトを作成します。|
|[mobileAppProvisioningConfigGroupAssignment の削除](../api/intune-apps-mobileappprovisioningconfiggroupassignment-delete.md)|なし|[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)を削除します。|
|[mobileAppProvisioningConfigGroupAssignment の更新](../api/intune-apps-mobileappprovisioningconfiggroupassignment-update.md)|[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)|[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|targetgroupid|String|アプリのプロビジョニング構成を対象とする AAD グループの ID。|
|id|String|エンティティのキー。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppProvisioningConfigGroupAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
  "targetGroupId": "String",
  "id": "String (identifier)"
}
```




