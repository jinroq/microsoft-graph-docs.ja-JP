---
title: androidDeviceOwnerEnrollmentProfile リソースの種類
description: Google のクラウド管理を使用して COSU デバイスを登録するために使われる登録プロファイルです。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dd22f0686a39dbd4531bb4228f5ed1ecca27b6bd
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30164415"
---
# <a name="androiddeviceownerenrollmentprofile-resource-type"></a>androidDeviceOwnerEnrollmentProfile リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Google のクラウド管理を使用して COSU デバイスを登録するために使われる登録プロファイルです。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト androidDeviceOwnerEnrollmentProfiles](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-list.md)|[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)コレクション|[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[androidDeviceOwnerEnrollmentProfile を取得する](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-get.md)|[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)|[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[androidDeviceOwnerEnrollmentProfile を作成する](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-create.md)|[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)|新しい[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)オブジェクトを作成します。|
|[androidDeviceOwnerEnrollmentProfile の削除](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-delete.md)|なし|[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)を削除します。|
|[androidDeviceOwnerEnrollmentProfile の更新](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-update.md)|[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)|[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)オブジェクトのプロパティを更新します。|
|[revokeToken action](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-revoketoken.md)|なし|まだ文書化されていません|
|[createToken action](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-createtoken.md)|なし|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|accountId|String|登録プロファイルが属するテナント GUID。|
|id|文字列|登録プロファイル用の一意な GUID。|
|displayName|String|登録プロファイルの表示名。|
|説明|文字列|登録プロファイルの説明。|
|createdDateTime|DateTimeOffset|登録プロファイルが作成された日時。|
|lastModifiedDateTime|DateTimeOffset|登録プロファイルが最後に変更された日時。|
|tokenValue|String|この登録プロファイル用に最後に作成されたトークンの値。|
|tokenの日付/時刻|DateTimeOffset|最後に作成されたトークンが作成された日時。|
|tokenExpirationDateTime|DateTimeOffset|最後に作成されたトークンの有効期限が切れる日時。|
|enrolledDeviceCount|Int32|この登録プロファイルを使用して登録した Android デバイスの合計数。|
|qrCodeContent|String|トークン用の QR コードを生成するために使用された文字列。|
|qrCodeImage|[mimeContent](../resources/intune-shared-mimecontent.md)|トークンの QR コードを生成するために使用する文字列。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidDeviceOwnerEnrollmentProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerEnrollmentProfile",
  "accountId": "String",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "tokenValue": "String",
  "tokenCreationDateTime": "String (timestamp)",
  "tokenExpirationDateTime": "String (timestamp)",
  "enrolledDeviceCount": 1024,
  "qrCodeContent": "String",
  "qrCodeImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  }
}
```




