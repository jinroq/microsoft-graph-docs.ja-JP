---
title: ImportedDeviceIdentityResult を更新します。
description: ImportedDeviceIdentityResult オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: 4c698810bb3fe88f52d8fcba11d8c29aeb508fe6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27332439"
---
# <a name="update-importeddeviceidentityresult"></a>ImportedDeviceIdentityResult を更新します。

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

[ImportedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)オブジェクトのプロパティを更新します。
## <a name="prerequisites"></a>前提条件
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類|アクセス許可 (特権の大きいものから小さいものへ)|
|:---|:---|
|委任 (職場または学校のアカウント)|DeviceManagementServiceConfig.ReadWrite.All|
|委任 (個人用 Microsoft アカウント)|サポートされていません。|
|アプリケーション|サポートされていません。|

## <a name="http-request"></a>HTTP 要求
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedDeviceIdentities/{importedDeviceIdentityId}
```

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー|値|
|:---|:---|
|Authorization|ベアラー &lt;トークン&gt; が必須。|
|Accept|application/json|

## <a name="request-body"></a>要求本文
要求の本文に[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)オブジェクトの JSON の形式を指定します。

[ImportedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)を作成するときに必要なプロパティを次の表に示します。

|プロパティ|種類|説明|
|:---|:---|:---|
|ID|String|[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承されるインポート済みのデバイス id の id|
|importedDeviceIdentifier|String|インポートされたデバイスの識別子から継承された[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)|
|importedDeviceIdentityType|[importedDeviceIdentityType](../resources/intune-enrollment-importeddeviceidentitytype.md)|[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)からインポートされたデバイスの Id を継承の種類。 可能な値は、`unknown`、`imei`、`serialNumber` です。|
|lastModifiedDateTime|DateTimeOffset|[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承する」の説明の最後の変更日時|
|createdDateTime|DateTimeOffset|[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承される、デバイスの日時を作成|
|lastContactedDateTime|DateTimeOffset|最終接続日時[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承されるデバイスの|
|説明|String|[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承される、デバイスの説明|
|enrollmentState|[enrollmentState](../resources/intune-enrollment-enrollmentstate.md)|Intune 継承で[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)からのデバイスの状態。 使用可能な値: `unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。|
|platform|[プラットフォーム](../resources/intune-enrollment-platform.md)|デバイスのプラットフォームです。 [ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承されます。 使用可能な値: `unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。|
|status|ブール型|インポートされたデバイス id のステータス|



## <a name="response"></a>応答
かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)オブジェクトです。

## <a name="example"></a>例
### <a name="request"></a>要求
以下は、要求の例です。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities/{importedDeviceIdentityId}
Content-type: application/json
Content-length: 354

{
  "importedDeviceIdentifier": "Imported Device Identifier value",
  "importedDeviceIdentityType": "imei",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios",
  "status": true
}
```

### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 529

{
  "@odata.type": "#microsoft.graph.importedDeviceIdentityResult",
  "id": "9dfd3690-3690-9dfd-9036-fd9d9036fd9d",
  "importedDeviceIdentifier": "Imported Device Identifier value",
  "importedDeviceIdentityType": "imei",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "description": "Description value",
  "enrollmentState": "enrolled",
  "platform": "ios",
  "status": true
}
```





