---
title: user リソースの種類
description: Azure Active Directory ユーザー オブジェクトを表します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: daa6f7a4802341347f364040504368dc96d75e33
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32548321"
---
# <a name="user-resource-type"></a>user リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Azure Active Directory ユーザー オブジェクトを表します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[ユーザーオブジェクトを一覧表示](../api/intune-shared-user-list.md)します。|[user](../resources/intune-shared-user.md) コレクション|[user](../resources/intune-shared-user.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[ユーザー](../api/intune-shared-user-get.md)オブジェクトを取得します。|[ユーザー](../resources/intune-shared-user.md)|[user](../resources/intune-shared-user.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[ユーザー](../api/intune-shared-user-create.md)オブジェクトを作成します。|[ユーザー](../resources/intune-shared-user.md)|新しい [user](../resources/intune-shared-user.md) オブジェクトを作成します。|
|[ユーザーを削除](../api/intune-shared-user-delete.md)します。|なし|[user](../resources/intune-shared-user.md) を削除します。|
|[ユーザー](../api/intune-shared-user-update.md)オブジェクトを更新します。|[user](../resources/intune-shared-user.md)|[user](../resources/intune-shared-user.md) オブジェクトのプロパティを更新します。|
|**デバイスの管理**|
|[getLoggedOnManagedDevices 関数](../api/intune-shared-user-getloggedonmanageddevices.md)|[managedDevice](../resources/intune-devices-manageddevice.md) コレクション|まだ文書化されていません|
|[removeAllDevicesFromManagement アクション](../api/intune-shared-user-removealldevicesfrommanagement.md)|なし|対象ユーザーの管理からすべてのデバイスを破棄します|
|**モバイルアプリケーション管理 (MAM)**|
|[getManagedAppDiagnosticStatuses 関数](../api/intune-shared-user-getmanagedappdiagnosticstatuses.md)|[managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) コレクション|特定のユーザーの診断検証状態を取得します。|
|[getManagedAppPolicies 関数](../api/intune-shared-user-getmanagedapppolicies.md)|[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) コレクション|特定のユーザーのアプリ制限を取得します。|
|[wipeManagedAppRegistrationByDeviceTag アクション](../api/intune-shared-user-wipemanagedappregistrationbydevicetag.md)|なし|指定されたデバイス タグが含まれるアプリ登録でワイプ操作を実行します。|
|[wipeManagedAppRegistrationsByDeviceTag アクション](../api/intune-shared-user-wipemanagedappregistrationsbydevicetag.md)|なし|指定されたデバイス タグが含まれるアプリ登録でワイプ操作を実行します。|
|**オンボーディング**|
|[exportdeviceandappmanagementdata 関数](../api/intune-shared-user-exportdeviceandappmanagementdata.md)|[deviceAndAppManagementData](../resources/intune-onboarding-deviceandappmanagementdata.md)|まだ文書化されていません|
|[getEffectiveDeviceEnrollmentConfigurations 関数](../api/intune-shared-user-geteffectivedeviceenrollmentconfigurations.md)|[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) コレクション|まだ文書化されていません|
|**トラブルシューティング**|
|[getManagedDevicesWithAppFailures 関数](../api/intune-shared-user-getmanageddeviceswithappfailures.md)|String collection|エラーが発生したアプリが含まれているデバイスの一覧を取得します。|


## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|ユーザーの一意識別子。|
|**オンボーディング**|
|deviceEnrollmentLimit|Int32|ユーザーが登録を許可されているデバイスの最大数。 使用できる値は 5 または 1000 です。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|**デバイスの管理**|
|managedDevices|[managedDevice](../resources/intune-devices-manageddevice.md) コレクション|対象ユーザーに関連付けられている管理対象デバイス。|
|**モバイルアプリケーション管理 (MAM)**|
|managedAppRegistrations|[managedAppRegistration](../resources/intune-mam-managedappregistration.md) コレクション|対象ユーザーに属する 0 個以上の管理対象アプリ登録。|
|**オンボーディング**|
|deviceEnrollmentConfigurations|[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) コレクション|ユーザーを対象とした登録構成を取得する|
|**トラブルシューティング**|
|deviceManagementTroubleshootingEvents|[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) コレクション|対象ユーザーのトラブルシューティング イベントの一覧です。|
|mobileAppIntentAndStates|[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)コレクション|対象ユーザーのトラブルシューティング イベントの一覧です。|
|mobileAppTroubleshootingEvents|[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)コレクション|このユーザーのモバイルアプリトラブルシューティングイベントのリスト。|

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



