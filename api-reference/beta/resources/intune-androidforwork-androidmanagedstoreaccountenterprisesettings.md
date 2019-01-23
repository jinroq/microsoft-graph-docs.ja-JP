---
title: androidManagedStoreAccountEnterpriseSettings リソースの種類
description: Android のエンタープライズの設定は、ストア アカウントを管理します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0deee2d3bbf816371a6331c000383398390e6610
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406382"
---
# <a name="androidmanagedstoreaccountenterprisesettings-resource-type"></a>androidManagedStoreAccountEnterpriseSettings リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Android のエンタープライズの設定は、ストア アカウントを管理します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[AndroidManagedStoreAccountEnterpriseSettings を取得します。](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-get.md)|[androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md)|[AndroidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md)オブジェクトのプロパティと関係を参照してください。|
|[AndroidManagedStoreAccountEnterpriseSettings を更新します。](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-update.md)|[androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md)|[AndroidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md)オブジェクトのプロパティを更新します。|
|[requestSignupUrl action](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-requestsignupurl.md)|String|まだ文書化されていません|
|[completeSignup action](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-completesignup.md)|なし|まだ文書化されていません|
|[syncApps action](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-syncapps.md)|なし|まだ文書化されていません|
|[unbind action](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-unbind.md)|なし|まだ文書化されていません|
|[createGooglePlayWebToken アクション](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-creategoogleplaywebtoken.md)|String|組み込み可能なコンポーネントで使用される web トークンを生成します。|
|[setAndroidDeviceOwnerFullyManagedEnrollmentState アクション](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-setandroiddeviceownerfullymanagedenrollmentstate.md)|なし|AndroidManagedStoreAccountEnterpriseSettings AndroidDeviceOwnerFullyManagedEnrollmentEnabled を指定した値に設定します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|アカウントのエンタープライズ設定の識別子を格納する、アプリ|
|bindStatus|[androidManagedStoreAccountBindStatus](../resources/intune-androidforwork-androidmanagedstoreaccountbindstatus.md)|Google の EMM の API を使用してテナントの状態をバインドします。 可能な値は、`notBound`、`bound`、`boundAndValidated`、`unbinding` です。|
|lastAppSyncDateTime|DateTimeOffset|アプリ同期の最終完了時刻|
|lastAppSyncStatus|[androidManagedStoreAccountAppSyncStatus](../resources/intune-androidforwork-androidmanagedstoreaccountappsyncstatus.md)|アプリケーション同期の最終結果です。 使用可能な値: `success`、`credentialsNotValid`、`androidForWorkApiError`、`managementServiceError`、`unknownError`、`none`。|
|ownerUserPrincipalName|String|エンタープライズを作成した所有者 UPN|
|ownerOrganizationName|String|組織名を使用する場合 Android のエンタープライズ契約時|
|lastModifiedDateTime|DateTimeOffset|Android エンタープライズ設定の最終変更時刻|
|enrollmentTarget|[androidManagedStoreAccountEnrollmentTarget](../resources/intune-androidforwork-androidmanagedstoreaccountenrollmenttarget.md)|Android エンタープライズ デバイスの管理デバイスを登録できるユーザーを示します。 可能な値は、`none`、`all`、`targeted`、`targetedAsEnrollmentRestrictions` です。|
|targetGroupIds|String コレクション|enrollmentTarget が 'Targeted' に設定されている場合、どの AAD グループが Android for Work デバイス管理にデバイスを登録できるかを指定します。|
|deviceOwnerManagementEnabled|Boolean|このアカウントを CloudDPC に Android のデバイスの所有者の管理の flighting かどうかを示します。|
|companyCodes|[androidEnrollmentCompanyCode](../resources/intune-androidforwork-androidenrollmentcompanycode.md)コレクション|AndroidManagedStoreAccountEnterpriseSettings の会社コード|
|androidDeviceOwnerFullyManagedEnrollmentEnabled|Boolean|AndroidManagedStoreAccountEnterpriseSettings の会社コード|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidManagedStoreAccountEnterpriseSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidManagedStoreAccountEnterpriseSettings",
  "id": "String (identifier)",
  "bindStatus": "String",
  "lastAppSyncDateTime": "String (timestamp)",
  "lastAppSyncStatus": "String",
  "ownerUserPrincipalName": "String",
  "ownerOrganizationName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "enrollmentTarget": "String",
  "targetGroupIds": [
    "String"
  ],
  "deviceOwnerManagementEnabled": true,
  "companyCodes": [
    {
      "@odata.type": "microsoft.graph.androidEnrollmentCompanyCode",
      "enrollmentToken": "String",
      "qrCodeContent": "String",
      "qrCodeImage": {
        "@odata.type": "microsoft.graph.mimeContent",
        "type": "String",
        "value": "binary"
      }
    }
  ],
  "androidDeviceOwnerFullyManagedEnrollmentEnabled": true
}
```




