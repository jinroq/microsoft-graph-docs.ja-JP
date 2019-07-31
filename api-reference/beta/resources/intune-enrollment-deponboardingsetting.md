---
title: depOnboardingSetting リソースの種類
description: DepOnboardingSetting は、Intune に利用されている Apple DEP サービスのインスタンスを表します。 利用サービスインスタンスは、Apple と Intune 間でデータを同期するために使用される Apple トークンを管理します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4209421a952ddfbcfa762cd7d5b6c7eb68cba8b2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35999228"
---
# <a name="deponboardingsetting-resource-type"></a>depOnboardingSetting リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

DepOnboardingSetting は、Intune に利用されている Apple DEP サービスのインスタンスを表します。 利用サービスインスタンスは、Apple と Intune 間でデータを同期するために使用される Apple トークンを管理します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[Depon掲示板の設定を一覧表示する](../api/intune-enrollment-deponboardingsetting-list.md)|[Deponboardingsetting](../resources/intune-enrollment-deponboardingsetting.md)コレクション|[Deponboardingsetting](../resources/intune-enrollment-deponboardingsetting.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[Depon掲示の設定を取得する](../api/intune-enrollment-deponboardingsetting-get.md)|[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)|[Deponboardingsetting](../resources/intune-enrollment-deponboardingsetting.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Depon掲示の設定を作成する](../api/intune-enrollment-deponboardingsetting-create.md)|[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)|新しい[Depon掲示設定](../resources/intune-enrollment-deponboardingsetting.md)オブジェクトを作成します。|
|[Depon掲示板の設定を削除する](../api/intune-enrollment-deponboardingsetting-delete.md)|None|[Depon掲示設定](../resources/intune-enrollment-deponboardingsetting.md)を削除します。|
|[DepOnboardingSetting の更新](../api/intune-enrollment-deponboardingsetting-update.md)|[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)|[Deponboardingsetting](../resources/intune-enrollment-deponboardingsetting.md)オブジェクトのプロパティを更新します。|
|[getEncryptionPublicKey 関数](../api/intune-enrollment-deponboardingsetting-getencryptionpublickey.md)|String|Apple device enrollment program トークンを暗号化するために使用する公開キーを取得する|
|[uploadDepToken アクション](../api/intune-enrollment-deponboardingsetting-uploaddeptoken.md)|None|新しいデバイス登録プログラムトークンをアップロードする|
|[syncWithAppleDeviceEnrollmentProgram アクション](../api/intune-enrollment-deponboardingsetting-syncwithappledeviceenrollmentprogram.md)|None|Apple Device Enrollment Program と Intune 間の同期|
|[shareForSchoolDataSyncService アクション](../api/intune-enrollment-deponboardingsetting-shareforschooldatasyncservice.md)|なし|まだ文書化されていません|
|[unshareForSchoolDataSyncService アクション](../api/intune-enrollment-deponboardingsetting-unshareforschooldatasyncservice.md)|なし|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|オブジェクトの UUID|
|appleIdentifier|String|現在のトークンを取得するために使用される Apple ID。|
|tokenExpirationDateTime|DateTimeOffset|トークンの有効期限が切れるとき。|
|lastModifiedDateTime|DateTimeOffset|サービスが利用されたとき。|
|lastSuccessfulSyncDateTime|DateTimeOffset|Intune でサービスが最後に使用されたとき|
|lastSyncTriggeredDateTime|DateTimeOffset|Intune が最後に同期を要求したとき。|
|shareTokenWithSchoolDataSyncService|Boolean|School Data Sync サービスで Dep トークンの共有が有効になっているかどうか。|
|lastSyncErrorCode|Int32|前回の dep 同期中に Apple によって報告されたエラーコード。|
|tokenType|[depTokenType](../resources/intune-enrollment-deptokentype.md)|Dep トークンの種類を取得または設定します。 可能な値は、`none`、`dep`、`appleSchoolManager` です。|
|tokenName|String|Dep トークンのフレンドリ名|
|syncedDeviceCount|Int32|同期されたデバイスの数を取得する|
|dataSharingConsentGranted|Boolean|Apple Dep サービスでのデータ共有に対して付与される同意|
|roleScopeTagIds|文字列コレクション|このエンティティインスタンスの範囲タグのリスト。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|defaultIosEnrollmentProfile|[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)|既定の iOS 登録プロファイル|
|defaultMacOsEnrollmentProfile|[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)|既定の MacOs 登録プロファイル|
|enrollmentProfiles|[しました](../resources/intune-enrollment-enrollmentprofile.md)コレクション|登録プロファイル。|
|importedAppleDeviceIdentities|[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)コレクション|インポートされた Apple デバイスの id です。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.depOnboardingSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.depOnboardingSetting",
  "id": "String (identifier)",
  "appleIdentifier": "String",
  "tokenExpirationDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "lastSuccessfulSyncDateTime": "String (timestamp)",
  "lastSyncTriggeredDateTime": "String (timestamp)",
  "shareTokenWithSchoolDataSyncService": true,
  "lastSyncErrorCode": 1024,
  "tokenType": "String",
  "tokenName": "String",
  "syncedDeviceCount": 1024,
  "dataSharingConsentGranted": true,
  "roleScopeTagIds": [
    "String"
  ]
}
```





