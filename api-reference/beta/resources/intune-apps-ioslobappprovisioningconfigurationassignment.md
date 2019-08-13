---
title: Ioslobappプロビジョニング Configurationassignment リソースの種類
description: IOS LOB アプリのプロビジョニングと構成のグループ割り当てに使用されるプロパティを含むクラス。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: adaf1bb989d30ab4afc7c534ca374bd014217164
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36366036"
---
# <a name="ioslobappprovisioningconfigurationassignment-resource-type"></a>Ioslobappプロビジョニング Configurationassignment リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

IOS LOB アプリのプロビジョニングと構成のグループ割り当てに使用されるプロパティを含むクラス。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[Ioslobappプロビジョニング Configurationassignments のリスト](../api/intune-apps-ioslobappprovisioningconfigurationassignment-list.md)|[Ioslobappプロビジョニング Configurationassignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)コレクション|[Ioslobappプロビジョニング Configurationassignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[Ioslobappプロビジョニング Configurationassignment の取得](../api/intune-apps-ioslobappprovisioningconfigurationassignment-get.md)|[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)|[Ioslobappプロビジョニング Configurationassignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Ioslobappプロビジョニング Configurationassignment の作成](../api/intune-apps-ioslobappprovisioningconfigurationassignment-create.md)|[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)|新しい[Ioslobappプロビジョニング Configurationassignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)オブジェクトを作成します。|
|[Ioslobappプロビジョニング Configurationassignment の削除](../api/intune-apps-ioslobappprovisioningconfigurationassignment-delete.md)|None|[Ioslobappプロビジョニング Configurationassignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)を削除します。|
|[Ioslobappプロビジョニング Configurationassignment の更新](../api/intune-apps-ioslobappprovisioningconfigurationassignment-update.md)|[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)|[Ioslobappプロビジョニング Configurationassignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)オブジェクトのプロパティを更新します。|

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



