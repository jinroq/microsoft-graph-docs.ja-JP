---
title: importedWindowsAutopilotDeviceIdentity の更新
description: importedWindowsAutopilotDeviceIdentity オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5360b08417e8867f3dcb7cc31c00690bc9b224be
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27880424"
---
# <a name="update-importedwindowsautopilotdeviceidentity"></a>importedWindowsAutopilotDeviceIdentity の更新

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) オブジェクトのプロパティを更新します。
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
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
```

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー|値|
|:---|:---|
|Authorization|ベアラー &lt;トークン&gt; が必須。|
|Accept|application/json|

## <a name="request-body"></a>要求本文
要求本文で、[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) オブジェクトの JSON 表記を指定します。

次の表に、[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) の作成時に必要なプロパティを示します。

|プロパティ|種類|説明|
|:---|:---|:---|
|ID|String|オブジェクトの GUID|
|orderIdentifier|String|Windows オートパイロット デバイスの受注 ID。|
|シリアル番号|String|Windows オートパイロット デバイスのシリアル番号。|
|productKey|String|Windows オートパイロット デバイスのプロダクト キー。|
|hardwareIdentifier|Binary|Windows オートパイロット デバイスのハードウェア BLOB。|
|state|[importedWindowsAutopilotDeviceIdentityState](../resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)|インポートしたデバイスの現在の状態。|



## <a name="response"></a>応答
成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) オブジェクトを返します。

## <a name="example"></a>例
### <a name="request"></a>要求
以下は、要求の例です。
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentities/{importedWindowsAutopilotDeviceIdentityId}
Content-type: application/json
Content-length: 541

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
  "orderIdentifier": "Order Identifier value",
  "serialNumber": "Serial Number value",
  "productKey": "Product Key value",
  "hardwareIdentifier": "aGFyZHdhcmVJZGVudGlmaWVy",
  "state": {
    "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityState",
    "deviceImportStatus": "pending",
    "deviceRegistrationId": "Device Registration Id value",
    "deviceErrorCode": 15,
    "deviceErrorName": "Device Error Name value"
  }
}
```

### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 590

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
  "id": "985b4f49-4f49-985b-494f-5b98494f5b98",
  "orderIdentifier": "Order Identifier value",
  "serialNumber": "Serial Number value",
  "productKey": "Product Key value",
  "hardwareIdentifier": "aGFyZHdhcmVJZGVudGlmaWVy",
  "state": {
    "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityState",
    "deviceImportStatus": "pending",
    "deviceRegistrationId": "Device Registration Id value",
    "deviceErrorCode": 15,
    "deviceErrorName": "Device Error Name value"
  }
}
```



