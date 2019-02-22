---
title: androidmanagedstoreaccountenterprisesettings リソースの種類
description: Android 管理ストアアカウントのエンタープライズ設定。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fd6f278963bd37276b808f221d1902fd82e23a48
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159137"
---
# <a name="androidmanagedstoreaccountenterprisesettings-resource-type"></a>androidmanagedstoreaccountenterprisesettings リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Android 管理ストアアカウントのエンタープライズ設定。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[androidmanagedstoreaccountenterprisesettings の取得](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-get.md)|[androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md)|[androidmanagedstoreaccountenterprisesettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[androidmanagedstoreaccountenterprisesettings の更新](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-update.md)|[androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md)|[androidmanagedstoreaccountenterprisesettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md)オブジェクトのプロパティを更新します。|
|[requestSignupUrl action](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-requestsignupurl.md)|String|まだ文書化されていません|
|[completeSignup action](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-completesignup.md)|なし|まだ文書化されていません|
|[syncApps action](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-syncapps.md)|なし|まだ文書化されていません|
|[unbind action](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-unbind.md)|なし|まだ文書化されていません|
|[createGooglePlayWebToken アクション](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-creategoogleplaywebtoken.md)|String|埋め込みコンポーネントで使用される web トークンを生成します。|
|[setAndroidDeviceOwnerFullyManagedEnrollmentState アクション](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-setandroiddeviceownerfullymanagedenrollmentstate.md)|なし|androidmanagedstoreaccountenterprisesettings AndroidDeviceOwnerFullyManagedEnrollmentEnabled を指定された値に設定します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|Android ストアアカウントのエンタープライズ設定識別子|
|bindStatus|[androidmanagedstoreaccountbindstatus](../resources/intune-androidforwork-androidmanagedstoreaccountbindstatus.md)|Google EMM API を使用して、テナントの状態をバインドします。 使用可能な値は、`notBound`、`bound`、`boundAndValidated`、`unbinding` です。|
|lastAppSyncDateTime|DateTimeOffset|アプリ同期の最終完了時刻|
|lastAppSyncStatus|[androidmanagedstoreaccountappsyncstatus](../resources/intune-androidforwork-androidmanagedstoreaccountappsyncstatus.md)|最後のアプリケーションの同期結果。 使用可能な値: `success`、`credentialsNotValid`、`androidForWorkApiError`、`managementServiceError`、`unknownError`、`none`。|
|ownerUserPrincipalName|String|エンタープライズを作成した所有者 UPN|
|ownerOrganizationName|String|Android Enterprise のオンボード時に使用される組織名|
|lastModifiedDateTime|DateTimeOffset|Android エンタープライズ設定の最終変更時刻|
|enrollmentTarget|[androidManagedStoreAccountEnrollmentTarget](../resources/intune-androidforwork-androidmanagedstoreaccountenrollmenttarget.md)|Android エンタープライズデバイス管理にデバイスを登録できるユーザーを示します。 使用可能な値は、`none`、`all`、`targeted`、`targetedAsEnrollmentRestrictions` です。|
|targetGroupIds|String コレクション|enrollmentTarget が 'Targeted' に設定されている場合、どの AAD グループが Android for Work デバイス管理にデバイスを登録できるかを指定します。|
|deviceownermanagementenabled|ブール値|CloudDPC を使用した Android デバイス所有者の管理に、このアカウントが flighting になるかどうかを示します。|
|会社コード|[androidEnrollmentCompanyCode](../resources/intune-androidforwork-androidenrollmentcompanycode.md)コレクション|androidmanagedstoreaccountenterprisesettings の会社コード|
|androidDeviceOwnerFullyManagedEnrollmentEnabled|ブール値|androidmanagedstoreaccountenterprisesettings の会社コード|

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




