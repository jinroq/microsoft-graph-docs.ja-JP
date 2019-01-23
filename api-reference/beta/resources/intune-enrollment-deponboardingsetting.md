---
title: depOnboardingSetting リソースの種類
description: DepOnboardingSetting は、Intune に onboarded をされている Apple の DEP のサービスのインスタンスを表します。 Onboarded サービスのインスタンスを管理、Apple トークンりんごと Intune の間でデータを同期するために使用します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3c0e5bcbdf0a687d4601aa92c8fe0eacdd675cd2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423770"
---
# <a name="deponboardingsetting-resource-type"></a>depOnboardingSetting リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

DepOnboardingSetting は、Intune に onboarded をされている Apple の DEP のサービスのインスタンスを表します。 Onboarded サービスのインスタンスを管理、Apple トークンりんごと Intune の間でデータを同期するために使用します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト depOnboardingSettings](../api/intune-enrollment-deponboardingsetting-list.md)|[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)コレクション|[DepOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)オブジェクトのプロパティと関係を一覧表示します。|
|[DepOnboardingSetting を取得します。](../api/intune-enrollment-deponboardingsetting-get.md)|[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)|[DepOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)オブジェクトのプロパティと関係を参照してください。|
|[DepOnboardingSetting を作成します。](../api/intune-enrollment-deponboardingsetting-create.md)|[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)|新しい[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)オブジェクトを作成します。|
|[DepOnboardingSetting を削除します。](../api/intune-enrollment-deponboardingsetting-delete.md)|なし|の[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)を削除します。|
|[DepOnboardingSetting を更新します。](../api/intune-enrollment-deponboardingsetting-update.md)|[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)|[DepOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)オブジェクトのプロパティを更新します。|
|[getEncryptionPublicKey 関数](../api/intune-enrollment-deponboardingsetting-getencryptionpublickey.md)|String|アップル デバイスの登録プログラムを暗号化するために使用する公開キーのトークンを取得します。|
|[uploadDepToken アクション](../api/intune-enrollment-deponboardingsetting-uploaddeptoken.md)|なし|新しいデバイスの登録プログラム トークンをアップロードします。|
|[syncWithAppleDeviceEnrollmentProgram アクション](../api/intune-enrollment-deponboardingsetting-syncwithappledeviceenrollmentprogram.md)|なし|アップル デバイスの登録プログラムと Intune との間の同期をとります|
|[shareForSchoolDataSyncService アクション](../api/intune-enrollment-deponboardingsetting-shareforschooldatasyncservice.md)|なし|まだ文書化されていません|
|[unshareForSchoolDataSyncService アクション](../api/intune-enrollment-deponboardingsetting-unshareforschooldatasyncservice.md)|なし|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|オブジェクトの UUID|
|appleIdentifier|String|Apple ID は、現在のトークンを取得するために使用します。|
|tokenExpirationDateTime|DateTimeOffset|トークンの期限が切れる。|
|lastModifiedDateTime|DateTimeOffset|Onboarded でした。|
|lastSuccessfulSyncDateTime|DateTimeOffset|Intune のサービスの最後の syned|
|lastSyncTriggeredDateTime|DateTimeOffset|Intune が最後に同期を要求された場合。|
|shareTokenWithSchoolDataSyncService|Boolean|かどうか Dep トークンの共有は学校のデータ同期サービスで有効になります。|
|lastSyncErrorCode|Int32|Dep の前回の同期中に、Apple によって報告されたエラー ・ コードです。|
|tokenType|[depTokenType](../resources/intune-enrollment-deptokentype.md)|Dep のトークンの種類を設定を取得または取得します。 可能な値は、`none`、`dep`、`appleSchoolManager` です。|
|tokenName|String|Dep のトークンの表示名|
|syncedDeviceCount|Int32|同期されたデバイスの数を取得|
|dataSharingConsentGranted|Boolean|アップル Dep のサービスと共有データの許可に同意するもの|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|defaultIosEnrollmentProfile|[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)|既定の I/o プロファイルの登録|
|defaultMacOsEnrollmentProfile|[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)|MacOs 登録プロファイルの既定値|
|enrollmentProfiles|[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)コレクション|登録のプロファイルです。|
|importedAppleDeviceIdentities|[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)コレクション|インポートされたアップルのデバイス id です。|

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
  "dataSharingConsentGranted": true
}
```




