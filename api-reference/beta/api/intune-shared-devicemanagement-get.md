---
title: deviceManagement の取得
description: deviceManagement オブジェクトのプロパティとリレーションシップを読み取ります。
ms.openlocfilehash: adc45ed789e3e636282fee851997c3fbcc8d8318
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069764"
---
# <a name="get-devicemanagement"></a>deviceManagement の取得

> **重要: **Microsoft Graph のベータ版 (/beta) の API はプレビュー中で、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

[deviceManagement](../resources/intune-shared-devicemanagement.md) オブジェクトのプロパティとリレーションシップを読み取ります。

## <a name="prerequisites"></a>前提条件

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

| アクセス権&nbsp;型&nbsp;(によって&nbsp;ワークフロー) | アクセス許可 (特権の大きいものから小さいものへ) |
|:---|:---|
| 委任 (職場または学校のアカウント) | |
| &nbsp;&nbsp; **Android の作業** | DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All |
| &nbsp; &nbsp; **監査** | DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All |
| &nbsp;&nbsp; **会社の用語** | DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All |
| &nbsp; &nbsp; **デバイス構成** | DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All |
| &nbsp; &nbsp; **デバイスの管理** | DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All |
| &nbsp;&nbsp; **電子 SIM** | DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All |
| &nbsp; &nbsp; **登録** | DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All |
| &nbsp;&nbsp; **フェンス** | DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All |
| &nbsp;&nbsp; **の通知** | DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All |
| &nbsp;&nbsp; **契約時** | DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All |
| &nbsp;&nbsp; **RBAC** | DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All |
| &nbsp;&nbsp; **リモート アクセス** | DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All |
| &nbsp;&nbsp; **リモート アシスタンス** | DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All |
| &nbsp;&nbsp; **通信経費の管理** | DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All |
| &nbsp; &nbsp; **トラブルシューティング** | DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All |
| &nbsp;&nbsp; **Windows 情報の保護** | DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All |
| 委任 (個人用 Microsoft アカウント) | サポートされていません。|
| アプリケーション | サポートされていません。 |



## <a name="http-request"></a>HTTP 要求
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement
```

## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター

このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー|値|
|:---|:---|
|Authorization|ベアラー &lt;トークン&gt; が必須。|
|Accept|application/json|

## <a name="request-body"></a>要求本文

このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答

成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceManagement](../resources/intune-shared-devicemanagement.md) オブジェクトを返します。

## <a name="example"></a>例

### <a name="request"></a>要求

以下は、要求の例です。
``` http
GET https://graph.microsoft.com/beta/deviceManagement
```

### <a name="response"></a>応答

応答の例を次に示します。 

注: ここに示す応答オブジェクトが簡潔にするために切り捨てられます。

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 130

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagement",
    "id": "0b283420-3420-0b28-2034-280b2034280b"
  }
}
```

ワークフローの適切なプロパティが返されます。

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 918

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagement",
    "id": "0b283420-3420-0b28-2034-280b2034280b",
    "subscriptionState": "active",
    "subscriptions": "intune",
    "adminConsent": {
      "@odata.type": "microsoft.graph.adminConsent",
      "shareAPNSData": "granted"
    },
    "deviceProtectionOverview": {
      "@odata.type": "microsoft.graph.deviceProtectionOverview",
      "totalReportedDeviceCount": 8,
      "inactiveThreatAgentDeviceCount": 14,
      "unknownStateThreatAgentDeviceCount": 2,
      "pendingSignatureUpdateDeviceCount": 1,
      "cleanDeviceCount": 0,
      "pendingFullScanDeviceCount": 10,
      "pendingRestartDeviceCount": 9,
      "pendingManualStepsDeviceCount": 13,
      "pendingOfflineScanDeviceCount": 13,
      "criticalFailuresDeviceCount": 11
    },
    "accountMoveCompletionDateTime": "2017-01-01T00:01:17.9006709-08:00"
  }
}
```



