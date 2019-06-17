---
title: Get deviceManagement
description: deviceManagement オブジェクトのプロパティとリレーションシップを読み取ります。
author: rolyon
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b1c3534583d1e5f825c734160dea3ddd8959934c
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34989687"
---
# <a name="get-devicemanagement"></a>Get deviceManagement

> **重要:** Microsoft Graph の/ベータ版の Api は変更される可能性があります。 実稼働アプリケーションでは、これらの API の使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

[deviceManagement](../resources/intune-shared-devicemanagement.md) オブジェクトのプロパティとリレーションシップを読み取ります。

## <a name="prerequisites"></a>前提条件

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

| アクセス&nbsp;許可&nbsp;の種類&nbsp;(ワークフロー別) | アクセス許可 (特権の大きいものから小さいものへ) |
|:---|:---|
| 委任 (職場または学校のアカウント) | |
| &nbsp;&nbsp; **Android for Work** | DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All |
| &nbsp; &nbsp; **監査** | DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All |
| &nbsp; &nbsp; **会社の用語** | DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All |
| &nbsp; &nbsp; **デバイス構成** | DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All |
| &nbsp;&nbsp; **デバイスの目的** | DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All|
| &nbsp;&nbsp; **デバイスの管理** | DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All |
| &nbsp;&nbsp; **電子 SIM** | DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All |
| &nbsp;&nbsp; **登録** | DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All |
| &nbsp;&nbsp; **フェンス** | DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All |
| &nbsp; &nbsp; **通知** | DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All |
| &nbsp;&nbsp; **Odj** | DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All |
| &nbsp; &nbsp; **オンボーディング** | DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All |
| &nbsp;&nbsp; **RBAC** | DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All |
| &nbsp; &nbsp; **リモート アクセス** | DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All |
| &nbsp;&nbsp; **リモートアシスタンス** | DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All |
| &nbsp;&nbsp; **通信経費管理** | DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All |
| &nbsp; &nbsp; **トラブルシューティング** | DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All |
| &nbsp; &nbsp; **Windows 情報保護** | DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All |
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
|Authorization|ベアラー &lt;トークン&gt; が必要です。|
|承諾|application/json|

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

注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。

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

ワークフローに適したプロパティが返されます。

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



