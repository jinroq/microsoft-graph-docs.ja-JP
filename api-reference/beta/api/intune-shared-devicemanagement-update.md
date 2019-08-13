---
title: deviceManagement の更新
description: deviceManagement オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b227d89df59e4b8a7bd975c96befe2c06e8af445
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36350854"
---
# <a name="update-devicemanagement"></a>deviceManagement の更新

> **重要:** Microsoft Graph の/ベータ版の Api は変更される可能性があります。 実稼働アプリケーションでは、これらの API の使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

[deviceManagement](../resources/intune-shared-devicemanagement.md) オブジェクトのプロパティを更新します。

## <a name="prerequisites"></a>前提条件

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

アクセス許可は、ワークフローによって異なることに注意してください。

| アクセス&nbsp;許可&nbsp;の種類&nbsp;(ワークフロー別) | アクセス許可 (特権の大きいものから小さいものへ) |
|:---|:---|
| 委任 (職場または学校のアカウント) ||
| &nbsp;&nbsp; **Android for Work** | DeviceManagementConfiguration.ReadWrite.All  |
| &nbsp; &nbsp; **監査** | DeviceManagementApps.ReadWrite.All |
| &nbsp; &nbsp; **会社の用語** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp; &nbsp; **デバイス構成** | DeviceManagementConfiguration.ReadWrite.All |
| &nbsp;&nbsp; **デバイスの目的** | DeviceManagementConfiguration.ReadWrite.All|
| &nbsp;&nbsp; **デバイスの管理** | DeviceManagementManagedDevices.ReadWrite.All |
| &nbsp;&nbsp; **電子 SIM** | DeviceManagementConfiguration.ReadWrite.All |
| &nbsp;&nbsp; **登録** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp; **フェンス** | DeviceManagementConfiguration.ReadWrite.All |
| &nbsp; &nbsp; **通知** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp; **Odj** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp; &nbsp; **オンボーディング** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp; &nbsp; **役割ベースのアクセス制御 (RBAC)** | DeviceManagementRBAC.ReadWrite.All |
| &nbsp; &nbsp; **リモート アクセス** | DeviceManagementConfiguration.Read.All |
| &nbsp;&nbsp; **リモートアシスタンス** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp; **通信経費管理** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp; **Troublehooting** | DeviceManagementManagedDevices.ReadWrite.All |
| &nbsp; &nbsp; **Windows 情報保護** | DeviceManagementApps.ReadWrite.All |
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
|Authorization|ベアラー &lt;トークン&gt; が必要です。|
|承諾|application/json|

## <a name="request-body"></a>要求本文

要求本文で、[deviceManagement](../resources/intune-shared-devicemanagement.md) オブジェクトの JSON 表記を指定します。

次の表に、[deviceManagement](../resources/intune-shared-devicemanagement.md) の作成時に必要なプロパティを示します。

|プロパティ|型|説明|
|:---|:---|:---|
|id|String|デバイスの一意識別子。|
|**デバイス構成**|
|Int未指定 Eaccountid|GUID|指定したテナントの Intune アカウント ID|
|legacyPcManangementEnabled|Boolean|このアカウントの非 MDM で管理されているレガシー PC 管理を有効にするプロパティ。 このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。|
|maximumDepTokens|Int32|テナントごとに許容される DEP トークンの最大数。|
|settings|[deviceManagementSettings](../resources/intune-deviceconfig-devicemanagementsettings.md)|アカウント レベルの設定。|
|**デバイスの管理**|
|accountMoveCompletionDateTime|DateTimeOffset|Scaleunits 間でテナントデータを移動したときの日付 & 時刻。|
|adminConsent|[adminConsent](../resources/intune-devices-adminconsent.md)|管理者の同意情報。|
|deviceProtectionOverview|[deviceProtectionOverview](../resources/intune-devices-deviceprotectionoverview.md)|デバイス保護の概要。|
|managedDeviceCleanupSettings|[managedDeviceCleanupSettings](../resources/intune-devices-manageddevicecleanupsettings.md)|デバイスクリーンアップルール|
|subscriptionState|[deviceManagementSubscriptionState](../resources/intune-devices-devicemanagementsubscriptionstate.md)|テナントのモバイル デバイス管理のサブスクリプション状態。 可能な値は、`pending`、`active`、`warning`、`disabled`、`deleted`、`blocked`、`lockedOut` です。|
|subscriptions|[deviceManagementSubscriptions](../resources/intune-devices-devicemanagementsubscriptions.md)|テナントのサブスクリプション。 使用可能な値: `none`、`intune`、`office365`、`intunePremium`、`intune_EDU`、`intune_SMB`。|
|windowsMalwareOverview|[windowsMalwareOverview](../resources/intune-devices-windowsmalwareoverview.md)|Windows デバイスのマルウェアの概要。|
|**オンボーディング**|
|intuneBrand|[intuneBrand](../resources/intune-onboarding-intunebrand.md)|intuneBrand には、会社のポータル アプリケーションとエンド ユーザーの Web ポータルの外観のカスタマイズに使用するデータが含まれています。|

要求本文のプロパティのサポートは、ワークフローによって異なります。

## <a name="response"></a>応答
成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceManagement](../resources/intune-shared-devicemanagement.md) オブジェクトを返します。

## <a name="example"></a>例

### <a name="request"></a>要求

以下は、デバイス管理ワークフローの後の要求の例です。

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

以下は、応答の例です。 

注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。 返されるプロパティは、ワークフローおよびコンテキストによって異なります。

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






