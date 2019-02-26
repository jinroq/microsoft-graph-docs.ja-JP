---
title: user リソースの種類
description: Azure Active Directory ユーザー オブジェクトを表します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a7a6c87b5c073e00b660db807ff38c454c302d94
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253408"
---
# <a name="user-resource-type"></a>user リソースの種類

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Azure Active Directory ユーザー オブジェクトを表します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[ユーザーオブジェクトを一覧表示](../api/intune-shared-user-list.md)します。|[user](../resources/intune-shared-user.md) コレクション|[user](../resources/intune-shared-user.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[ユーザー](../api/intune-shared-user-get.md)オブジェクトを取得します。|[user](../resources/intune-shared-user.md) コレクション|[user](../resources/intune-shared-user.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[ユーザー](../api/intune-shared-user-create.md)オブジェクトを作成します。|[user](../resources/intune-shared-user.md) コレクション|新しい [user](../resources/intune-shared-user.md) オブジェクトを作成します。|
|[ユーザーを削除](../api/intune-shared-user-delete.md)します。|なし|[user](../resources/intune-shared-user.md) を削除します。|
|[ユーザー](../api/intune-shared-user-update.md)オブジェクトを更新します。|[user](../resources/intune-shared-user.md)|[user](../resources/intune-shared-user.md) オブジェクトのプロパティを更新します。|
|**デバイスの管理**|
|[removeAllDevicesFromManagement アクション](../api/intune-shared-user-removealldevicesfrommanagement.md)|なし|対象ユーザーの管理からすべてのデバイスを破棄します|
|**モバイルアプリ管理 (MAM)**|
|[getManagedAppDiagnosticStatuses 関数](../api/intune-shared-user-getmanagedappdiagnosticstatuses.md)|[managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) コレクション|特定のユーザーの診断検証状態を取得します。|
|[getManagedAppPolicies 関数](../api/intune-shared-user-getmanagedapppolicies.md)|[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) コレクション|特定のユーザーのアプリ制限を取得します。|
|[wipeManagedAppRegistrationsByDeviceTag アクション](../api/intune-shared-user-wipemanagedappregistrationsbydevicetag.md)|なし|指定されたデバイス タグが含まれるアプリ登録でワイプ操作を実行します。|

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
|**モバイルアプリ管理 (MAM)**|
|managedAppRegistrations|[managedAppRegistration](../resources/intune-mam-managedappregistration.md) コレクション|対象ユーザーに属する 0 個以上の管理対象アプリ登録。|
|**トラブルシューティング**|
|deviceManagementTroubleshootingEvents|[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) コレクション|対象ユーザーのトラブルシューティング イベントの一覧です。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.directoryObject",
  "openType": true,
  "@odata.type": "microsoft.graph.user"
}
--> 
``` json
{
  "@odata.type": "#microsoft.graph.user",
  "id": "String (identifier)",
  "deviceEnrollmentLimit": 5
}
```

<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Warning: Resource microsoft.graph.user is defined in multiple files: /api-reference/v1.0/resources/intune_shared_user.md, /api-reference/v1.0/resources/user.md",
  ]
}-->
