---
title: user リソースの種類
description: Azure Active Directory ユーザー オブジェクトを表します。
ms.openlocfilehash: ec28b7ec44eddfa1e1e8b372956d1a29dc78553d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070981"
---
# <a name="user-resource-type"></a>user リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Azure Active Directory ユーザー オブジェクトを表します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[ユーザーの一覧](../api/intune-shared-user-list.md)のオブジェクトです。|[user](../resources/intune-shared-user.md) コレクション|[user](../resources/intune-shared-user.md) オブジェクトのプロパティとリレーションシップをリストします。|
|オブジェクトの[ユーザーを取得](../api/intune-shared-user-get.md)します。|[user](../resources/intune-shared-user.md)|[user](../resources/intune-shared-user.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[作成するユーザー](../api/intune-shared-user-create.md)オブジェクトです。|[user](../resources/intune-shared-user.md)|新しい [user](../resources/intune-shared-user.md) オブジェクトを作成します。|
|[ユーザーを削除](../api/intune-shared-user-delete.md)します。|なし|[user](../resources/intune-shared-user.md) を削除します。|
|[更新プログラムのユーザー](../api/intune-shared-user-update.md)オブジェクトです。|[user](../resources/intune-shared-user.md)|[user](../resources/intune-shared-user.md) オブジェクトのプロパティを更新します。|
|**デバイスの管理**|
|[getLoggedOnManagedDevices 関数](../api/intune-shared-user-getloggedonmanageddevices.md)|[managedDevice](../resources/intune-devices-manageddevice.md) コレクション|まだ文書化されていません|
|[removeAllDevicesFromManagement アクション](../api/intune-shared-user-removealldevicesfrommanagement.md)|なし|対象ユーザーの管理からすべてのデバイスを破棄します|
|**モバイル アプリケーション管理 (MAM)**|
|[getManagedAppDiagnosticStatuses 関数](../api/intune-shared-user-getmanagedappdiagnosticstatuses.md)|[managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) コレクション|特定のユーザーの診断検証状態を取得します。|
|[getManagedAppPolicies 関数](../api/intune-shared-user-getmanagedapppolicies.md)|[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) コレクション|特定のユーザーのアプリ制限を取得します。|
|[wipeManagedAppRegistrationByDeviceTag アクション](../api/intune-shared-user-wipemanagedappregistrationbydevicetag.md)|なし|指定されたデバイス タグが含まれるアプリ登録でワイプ操作を実行します。|
|[wipeManagedAppRegistrationsByDeviceTag アクション](../api/intune-shared-user-wipemanagedappregistrationsbydevicetag.md)|なし|指定されたデバイス タグが含まれるアプリ登録でワイプ操作を実行します。|
|**契約時**|
|[exportDeviceAndAppManagementData 関数](../api/intune-shared-user-exportdeviceandappmanagementdata.md)|[deviceAndAppManagementData](../resources/intune-onboarding-deviceandappmanagementdata.md)|まだ文書化されていません|
|[getEffectiveDeviceEnrollmentConfigurations 関数](../api/intune-shared-user-geteffectivedeviceenrollmentconfigurations.md)|[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) コレクション|まだ文書化されていません|
|**トラブルシューティング**|
|[getManagedDevicesWithAppFailures 関数](../api/intune-shared-user-getmanageddeviceswithappfailures.md)|String コレクション|失敗したアプリを使用してデバイスの一覧を取得します。|


## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|ユーザーの一意識別子。|
|**契約時**|
|deviceEnrollmentLimit|Int32|ユーザーが登録を許可されているデバイスの最大数。 使用できる値は 5 または 1000 です。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|**デバイスの管理**|
|managedDevices|[managedDevice](../resources/intune-devices-manageddevice.md) コレクション|対象ユーザーに関連付けられている管理対象デバイス。|
|**モバイル アプリケーション管理 (MAM)**|
|managedAppRegistrations|[managedAppRegistration](../resources/intune-mam-managedappregistration.md) コレクション|対象ユーザーに属する 0 個以上の管理対象アプリ登録。|
|**契約時**|
|deviceEnrollmentConfigurations|[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) コレクション|ユーザーを対象とした登録の構成を取得します。|
|**トラブルシューティング**|
|deviceManagementTroubleshootingEvents|[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) コレクション|対象ユーザーのトラブルシューティング イベントの一覧です。|
|mobileAppIntentAndStates|[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)コレクション|対象ユーザーのトラブルシューティング イベントの一覧です。|
|mobileAppTroubleshootingEvents|[mobileAppTroubleshootingEvent](../resources/intune-troubleshooting-mobileapptroubleshootingevent.md)コレクション|モバイル アプリケーションがこのユーザーのイベントをトラブルシューティングの一覧です。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.user"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.user",
  "id": "String (identifier)"
}
```



