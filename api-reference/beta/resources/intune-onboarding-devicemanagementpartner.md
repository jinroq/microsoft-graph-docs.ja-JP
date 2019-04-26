---
title: deviceManagementPartner リソースの種類
description: デバイス管理パートナーとの接続を表すエンティティです。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1586f767f8576a1dae94e435ca25056a7b686b93
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566557"
---
# <a name="devicemanagementpartner-resource-type"></a>deviceManagementPartner リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

デバイス管理パートナーとの接続を表すエンティティです。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[List deviceManagementPartners](../api/intune-onboarding-devicemanagementpartner-list.md)|[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) コレクション|[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[Get deviceManagementPartner](../api/intune-onboarding-devicemanagementpartner-get.md)|[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md)|[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Create deviceManagementPartner](../api/intune-onboarding-devicemanagementpartner-create.md)|[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md)|新しい [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) オブジェクトを作成します。|
|[Delete deviceManagementPartner](../api/intune-onboarding-devicemanagementpartner-delete.md)|なし|[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) を削除します。|
|[Update deviceManagementPartner](../api/intune-onboarding-devicemanagementpartner-update.md)|[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md)|[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティの Id|
|lastHeartbeatDateTime|DateTimeOffset|管理者が [デバイス管理パートナーに接続] オプションを有効にした後の最終ハートビートのタイムスタンプ|
|partnerState|[devicemanagementpartnertenantstate](../resources/intune-onboarding-devicemanagementpartnertenantstate.md)|このテナントのパートナーの状態。 使用可能な値: `unknown`、`unavailable`、`enabled`、`terminated`、`rejected`、`unresponsive`。|
|partnerAppType|[deviceManagementPartnerAppType](../resources/intune-onboarding-devicemanagementpartnerapptype.md)|パートナーアプリの種類。 可能な値は `unknown`、`singleTenantApp`、`multiTenantApp` です。|
|singleTenantAppId|String|パートナーのシングル テナントのアプリ ID|
|displayName|String|パートナー表示名|
|isConfigured|ブール型 (Boolean)|デバイス管理パートナーが構成されているかどうかを指定します|
|whenPartnerDevicesWillBeRemoved|DateTimeOffset|パートナーデバイスが削除される日時 (UTC)。 これはすぐに obselete になります。|
|whenPartnerDevicesWillBeMarkedAsNonCompliant|DateTimeOffset|パートナーデバイスが準拠していないとマークされるときの、UTC の DateTime。 これはすぐに obselete になります。|
|whenPartnerDevicesWillBeRemovedDateTime|DateTimeOffset|パートナー デバイスが削除されるときの日時 (UTC)|
|whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime|DateTimeOffset|パートナー デバイスが準拠していないとマークされるときの日時 (UTC)|

## <a name="relationships"></a>関係
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementPartner"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementPartner",
  "id": "String (identifier)",
  "lastHeartbeatDateTime": "String (timestamp)",
  "partnerState": "String",
  "partnerAppType": "String",
  "singleTenantAppId": "String",
  "displayName": "String",
  "isConfigured": true,
  "whenPartnerDevicesWillBeRemoved": "String (timestamp)",
  "whenPartnerDevicesWillBeMarkedAsNonCompliant": "String (timestamp)",
  "whenPartnerDevicesWillBeRemovedDateTime": "String (timestamp)",
  "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "String (timestamp)"
}
```





