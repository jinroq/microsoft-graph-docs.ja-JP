---
title: deviceManagement の更新
description: deviceManagement オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4d8465ee45a2a6c23dedc4fe049ef1f73bb25218
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924693"
---
# <a name="update-devicemanagement"></a>deviceManagement の更新

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

[deviceManagement](../resources/intune-shared-devicemanagement.md) オブジェクトのプロパティを更新します。

## <a name="prerequisites"></a>前提条件

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

ワークフローに応じて、[アクセス許可が異なることに注意してください。

| アクセス権&nbsp;型&nbsp;(によって&nbsp;ワークフロー) | アクセス許可 (特権の大きいものから小さいものへ) |
|:---|:---|
| 委任 (職場または学校のアカウント) ||
| &nbsp;&nbsp; **Android の作業** | DeviceManagementConfiguration.ReadWrite.All  |
| &nbsp; &nbsp; **監査** | DeviceManagementApps.ReadWrite.All |
| &nbsp;&nbsp; **会社の用語** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp; &nbsp; **デバイス構成** | DeviceManagementConfiguration.ReadWrite.All |
| &nbsp; &nbsp; **デバイスの管理** | DeviceManagementManagedDevices.ReadWrite.All |
| &nbsp;&nbsp; **電子 SIM** | DeviceManagementConfiguration.ReadWrite.All |
| &nbsp; &nbsp; **登録** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp; **フェンス** | DeviceManagementConfiguration.ReadWrite.All |
| &nbsp;&nbsp; **の通知** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp; **契約時** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp; **ロール ベースのアクセス制御 (RBAC)** | DeviceManagementRBAC.ReadWrite.All |
| &nbsp;&nbsp; **リモート アクセス** | DeviceManagementConfiguration.Read.All |
| &nbsp;&nbsp; **リモート アシスタンス** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp; **通信経費の管理** | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp; **Troublehooting** | DeviceManagementManagedDevices.ReadWrite.All |
| &nbsp;&nbsp; **Windows 情報の保護** | DeviceManagementApps.ReadWrite.All |
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
|Accept|application/json|

## <a name="request-body"></a>要求本文

要求本文で、[deviceManagement](../resources/intune-shared-devicemanagement.md) オブジェクトの JSON 表記を指定します。

次の表に、[deviceManagement](../resources/intune-shared-devicemanagement.md) の作成時に必要なプロパティを示します。

|プロパティ|種類|説明|
|:---|:---|:---|
|ID|String|デバイスの一意の識別子です。|
|**デバイス構成**|
|intuneAccountId|GUID|Intune アカウント ID にはテナントが指定されました。|
|legacyPcManangementEnabled|ブール型|非 MDM を有効にするプロパティは、このアカウントの従来の PC の管理を管理します。 このプロパティは読み取りのみ可能です。|
|maximumDepTokens|Int32|DEP のトークンの最大数では、テナントごとに許可されます。|
|settings|[deviceManagementSettings](../resources/intune-deviceconfig-devicemanagementsettings.md)|アカウント レベルの設定。|
|**デバイスの管理**|
|accountMoveCompletionDateTime|DateTimeOffset|日付と時刻 scaleunits のテナントのデータを移動するときです。|
|adminConsent|[adminConsent](../resources/intune-devices-adminconsent.md)|同意の情報を管理します。|
|deviceProtectionOverview|[deviceProtectionOverview](../resources/intune-devices-deviceprotectionoverview.md)|デバイス保護の概要です。|
|managedDeviceCleanupSettings|[managedDeviceCleanupSettings](../resources/intune-devices-manageddevicecleanupsettings.md)|デバイスのクリーンアップ ・ ルール|
|subscriptionState|[deviceManagementSubscriptionState](../resources/intune-devices-devicemanagementsubscriptionstate.md)|テナントのモバイル デバイス管理のサブスクリプション状態。 可能な値は、`pending`、`active`、`warning`、`disabled`、`deleted`、`blocked`、`lockedOut` です。|
|サブスクリプション|[deviceManagementSubscriptions](../resources/intune-devices-devicemanagementsubscriptions.md)|テナントのサブスクリプション。 使用可能な値: `none`、`intune`、`office365`、`intunePremium`、`intune_EDU`、`intune_SMB`。|
|windowsMalwareOverview|[windowsMalwareOverview](../resources/intune-devices-windowsmalwareoverview.md)|Windows デバイスのマルウェアの概要です。|
|**契約時**|
|intuneBrand|[intuneBrand](../resources/intune-onboarding-intunebrand.md)|intuneBrand には、会社のポータル アプリケーションとエンド ユーザーの Web ポータルの外観のカスタマイズに使用するデータが含まれています。|

要求本文のプロパティのサポートは、ワークフローによって異なります。

## <a name="response"></a>応答
成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceManagement](../resources/intune-shared-devicemanagement.md) オブジェクトを返します。

## <a name="example"></a>例

### <a name="request"></a>要求

デバイス管理のワークフローを次の要求の例を以下に示します。

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



