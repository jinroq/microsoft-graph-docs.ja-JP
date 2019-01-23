---
title: WindowsAutopilotDeviceIdentity を作成します。
description: 新しい windowsAutopilotDeviceIdentity オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9d9287738b33b1afe55a3f22c441b888ae7d77b4
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406396"
---
# <a name="create-windowsautopilotdeviceidentity"></a>WindowsAutopilotDeviceIdentity を作成します。

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

新しい[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)オブジェクトを作成します。

## <a name="prerequisites"></a>前提条件
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。

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
POST /deviceManagement/windowsAutopilotDeviceIdentities
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices
```

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー|値|
|:---|:---|
|Authorization|ベアラー &lt;トークン&gt; が必須。|
|Accept|application/json|

## <a name="request-body"></a>要求本文
要求の本文に windowsAutopilotDeviceIdentity オブジェクトの JSON の形式を指定します。

次の表は、windowsAutopilotDeviceIdentity を作成するときに必要なプロパティを示します。

|プロパティ|型|説明|
|:---|:---|:---|
|id|String|オブジェクトの GUID|
|deploymentProfileAssignmentStatus|[windowsAutopilotProfileAssignmentStatus](../resources/intune-enrollment-windowsautopilotprofileassignmentstatus.md)|Windows の自動操縦装置のデバイスの割り当ての状態をプロファイルします。 可能な値は、`unknown`、`assignedInSync`、`assignedOutOfSync`、`assignedUnkownSyncState`、`notAssigned`、`pending`、`failed` です。|
|deploymentProfileAssignmentDetailedStatus|[windowsAutopilotProfileAssignmentDetailedStatus](../resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)|プロファイルの割り当ては、Windows の自動操縦装置のデバイスの状態を詳しく説明します。 使用可能な値は、`none`、`hardwareRequirementsNotMet` です。|
|deploymentProfileAssignedDateTime|DateTimeOffset|プロファイルは、Windows の自動操縦装置のデバイスの時刻を設定します。|
|orderIdentifier|String|Windows の自動操縦装置のデバイスの順序の識別子です。|
|purchaseOrderIdentifier|String|Windows の自動操縦装置のデバイスの購買注文の識別子です。|
|シリアル番号|String|Windows オートパイロット デバイスのシリアル番号。|
|productKey|String|Windows オートパイロット デバイスのプロダクト キー。|
|manufacturer|String|Windows の自動操縦装置のデバイスの Oem メーカーです。|
|model|String|Windows の自動操縦装置のデバイスのモデル名です。|
|enrollmentState|[enrollmentState](../resources/intune-enrollment-enrollmentstate.md)|Intune Windows の自動操縦装置のデバイスの状態を登録します。 使用可能な値: `unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。|
|lastContactedDateTime|DateTimeOffset|Intune 最終接続日時 Windows の自動操縦装置のデバイスのです。|
|addressableUserName|String|アドレス指定可能なユーザー名です。|
|userPrincipalName|String|ユーザー プリンシパル名です。|



## <a name="response"></a>応答
かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)オブジェクトです。

## <a name="example"></a>例

### <a name="request"></a>要求
以下は、要求の例です。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities
Content-type: application/json
Content-length: 755

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeviceIdentity",
  "deploymentProfileAssignmentStatus": "assignedInSync",
  "deploymentProfileAssignmentDetailedStatus": "hardwareRequirementsNotMet",
  "deploymentProfileAssignedDateTime": "2016-12-31T23:58:26.2447023-08:00",
  "orderIdentifier": "Order Identifier value",
  "purchaseOrderIdentifier": "Purchase Order Identifier value",
  "serialNumber": "Serial Number value",
  "productKey": "Product Key value",
  "manufacturer": "Manufacturer value",
  "model": "Model value",
  "enrollmentState": "enrolled",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "addressableUserName": "Addressable User Name value",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 804

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeviceIdentity",
  "id": "fac6f0b1-f0b1-fac6-b1f0-c6fab1f0c6fa",
  "deploymentProfileAssignmentStatus": "assignedInSync",
  "deploymentProfileAssignmentDetailedStatus": "hardwareRequirementsNotMet",
  "deploymentProfileAssignedDateTime": "2016-12-31T23:58:26.2447023-08:00",
  "orderIdentifier": "Order Identifier value",
  "purchaseOrderIdentifier": "Purchase Order Identifier value",
  "serialNumber": "Serial Number value",
  "productKey": "Product Key value",
  "manufacturer": "Manufacturer value",
  "model": "Model value",
  "enrollmentState": "enrolled",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "addressableUserName": "Addressable User Name value",
  "userPrincipalName": "User Principal Name value"
}
```




