---
title: ioslobappプロビジョニング configurationassignment リソースの種類
description: iOS LOB アプリのプロビジョニングと構成のグループ割り当てに使用されるプロパティを含むクラス。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d6a87b3cc18724007a948935ef5a00a1341efc6b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32553030"
---
# <a name="ioslobappprovisioningconfigurationassignment-resource-type"></a>ioslobappプロビジョニング configurationassignment リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

iOS LOB アプリのプロビジョニングと構成のグループ割り当てに使用されるプロパティを含むクラス。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[ioslobappプロビジョニング configurationassignments のリスト](../api/intune-apps-ioslobappprovisioningconfigurationassignment-list.md)|[ioslobappプロビジョニング configurationassignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)コレクション|[ioslobappプロビジョニング configurationassignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[ioslobappプロビジョニング configurationassignment の取得](../api/intune-apps-ioslobappprovisioningconfigurationassignment-get.md)|[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)|[ioslobappプロビジョニング configurationassignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[ioslobappプロビジョニング configurationassignment の作成](../api/intune-apps-ioslobappprovisioningconfigurationassignment-create.md)|[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)|新しい[ioslobappプロビジョニング configurationassignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)オブジェクトを作成します。|
|[ioslobappプロビジョニング configurationassignment の削除](../api/intune-apps-ioslobappprovisioningconfigurationassignment-delete.md)|なし|[ioslobappプロビジョニング configurationassignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)を削除します。|
|[ioslobappプロビジョニング configurationassignment の更新](../api/intune-apps-ioslobappprovisioningconfigurationassignment-update.md)|[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)|[ioslobappプロビジョニング configurationassignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|管理者によって定義された、ターゲット グループの割り当て。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosLobAppProvisioningConfigurationAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfigurationAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





