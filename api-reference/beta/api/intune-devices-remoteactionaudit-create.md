---
title: RemoteActionAudit を作成します。
description: 新しい remoteActionAudit オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d159565616664b1c795072336046c25585c42fa6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27881796"
---
# <a name="create-remoteactionaudit"></a>RemoteActionAudit を作成します。

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

新しい[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)オブジェクトを作成します。
## <a name="prerequisites"></a>前提条件
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類|アクセス許可 (特権の大きいものから小さいものへ)|
|:---|:---|
|委任 (職場または学校のアカウント)|DeviceManagementManagedDevices.ReadWrite.All|
|委任 (個人用 Microsoft アカウント)|サポートされていません。|
|アプリケーション|サポートされていません。|

## <a name="http-request"></a>HTTP 要求
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/remoteActionAudits
```

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー|値|
|:---|:---|
|Authorization|ベアラー &lt;トークン&gt; が必須。|
|Accept|application/json|

## <a name="request-body"></a>要求本文
要求の本文に remoteActionAudit オブジェクトの JSON の形式を指定します。

次の表は、remoteActionAudit を作成するときに必要なプロパティを示します。

|プロパティ|種類|説明|
|:---|:---|:---|
|ID|String|レポートの id。|
|deviceDisplayName|String|Intune デバイスの名前です。|
|userName|String|\[推奨\]InitiatedByUserPrincipalName を代わりに使用してください。|
|initiatedByUserPrincipalName|String|デバイスのアクションを開始したユーザーは、UPN 形式です。|
|action|[remoteAction](../resources/intune-devices-remoteaction.md)|アクション名。 使用可能な値: `unknown`、 `factoryReset`、 `removeCompanyData`、 `resetPasscode`、 `remoteLock`、 `enableLostMode`、 `disableLostMode`、 `locateDevice`、 `rebootNow`、 `recoverPasscode`、 `cleanWindowsDevice`、 `logoutSharedAppleDeviceActiveUser`、 `quickScan`、 `fullScan`、 `windowsDefenderUpdateSignatures`、 `factoryResetKeepEnrollmentData`、 `updateDeviceAccount`、 `automaticRedeployment`、 `shutDown`.|
|requestDateTime|DateTimeOffset|UTC で指定されたアクションを発行した時の時間です。|
|deviceOwnerUserPrincipalName|String|デバイス所有者の Upn。|
|deviceIMEI|String|デバイスの IMEI。|
|actionState|[actionState](../resources/intune-shared-actionstate.md)|動作状態です。 可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。|



## <a name="response"></a>応答
かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)オブジェクトです。

## <a name="example"></a>例
### <a name="request"></a>要求
以下は、要求の例です。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/remoteActionAudits
Content-type: application/json
Content-length: 455

{
  "@odata.type": "#microsoft.graph.remoteActionAudit",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "initiatedByUserPrincipalName": "Initiated By User Principal Name value",
  "action": "factoryReset",
  "requestDateTime": "2017-01-01T00:03:07.1589002-08:00",
  "deviceOwnerUserPrincipalName": "Device Owner User Principal Name value",
  "deviceIMEI": "Device IMEI value",
  "actionState": "pending"
}
```

### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 504

{
  "@odata.type": "#microsoft.graph.remoteActionAudit",
  "id": "477f8d24-8d24-477f-248d-7f47248d7f47",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "initiatedByUserPrincipalName": "Initiated By User Principal Name value",
  "action": "factoryReset",
  "requestDateTime": "2017-01-01T00:03:07.1589002-08:00",
  "deviceOwnerUserPrincipalName": "Device Owner User Principal Name value",
  "deviceIMEI": "Device IMEI value",
  "actionState": "pending"
}
```





