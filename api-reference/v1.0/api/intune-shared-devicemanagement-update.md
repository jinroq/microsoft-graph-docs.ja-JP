---
title: deviceManagement の更新
description: deviceManagement オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c96877d25476ede3cee6ce407c1df84f08448a9a
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253058"
---
# <a name="update-devicemanagement"></a>deviceManagement の更新

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

[deviceManagement](../resources/intune-shared-devicemanagement.md) オブジェクトのプロパティを更新します。

## <a name="prerequisites"></a>前提条件
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

| アクセス&nbsp;許可&nbsp;の種類&nbsp;(ワークフロー別) | アクセス許可 (特権の大きいものから小さいものへ) |
|:---|:---|
| 委任 (職場または学校のアカウント) |
| &nbsp;&nbsp;監査 | DeviceManagementApps.ReadWrite.All |
| &nbsp;&nbsp;会社の使用条件 | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp;企業の登録 | DeviceManagementServiceConfig.ReadWrite.All|
| &nbsp;&nbsp;デバイス構成 | DeviceManagementConfiguration.ReadWrite.All |
| &nbsp;&nbsp;デバイスの管理 | DeviceManagementManagedDevices.ReadWrite.All |
| &nbsp;&nbsp;エンドポイント保護 | DeviceManagementManagedDevices.ReadWrite.All |
| &nbsp;&nbsp;通知 | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp;オンボード | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp;役割ベースのアクセス制御 | DeviceManagementRBAC.ReadWrite.All |
| &nbsp;&nbsp;リモートアシスタンス | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp;通信経費管理 | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp;トラブルシューティング | DeviceManagementManagedDevices.ReadWrite.All |
| &nbsp;&nbsp; Windows 情報保護 | DeviceManagementApps.ReadWrite.All |
| 委任 (個人用 Microsoft アカウント) | サポートされていません。|
| アプリケーション | サポートされていません。 |

## <a name="http-request"></a>HTTP 要求
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー|値|
|:---|:---|
|Authorization|ベアラー &lt;トークン&gt; が必須。|
|承諾|application/json|

## <a name="request-body"></a>要求本文
要求本文で、[deviceManagement](../resources/intune-shared-devicemanagement.md) オブジェクトの JSON 表記を指定します。

次の表に、[deviceManagement](../resources/intune-shared-devicemanagement.md) の作成時に必要なプロパティを示します。

|プロパティ|型|説明|
|:---|:---|:---|
|id|String|デバイスの一意識別子|
|**デバイス構成**|
|settings|[deviceManagementSettings](../resources/intune-deviceconfig-devicemanagementsettings.md)|アカウント レベルの設定。|
|**デバイスの管理**|
|subscriptionState|[devicemanagementsubscriptionstate](../resources/intune-devices-devicemanagementsubscriptionstate.md)|テナントのモバイル デバイス管理のサブスクリプション状態。 使用可能な値: `pending`、`active`、`warning`、`disabled`、`deleted`、`blocked`、`lockedOut`。|
|**オンボーディング**|
|intuneBrand|[intuneBrand](../resources/intune-onboarding-intunebrand.md)|intuneBrand には、会社のポータル アプリケーションとエンド ユーザーの Web ポータルの外観のカスタマイズに使用するデータが含まれています。|

要求本文のプロパティのサポートは、ワークフローによって異なります。

## <a name="response"></a>応答
成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceManagement](../resources/intune-shared-devicemanagement.md) オブジェクトを返します。

## <a name="example"></a>例

### <a name="request"></a>要求
以下は、要求の例です。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement
Content-type: application/json
Content-length: 751

{
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
```

### <a name="response"></a>応答

以下は、応答の例です。 注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。 返されるプロパティは、ワークフローおよびコンテキストによって異なります。

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 855

{
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
```



