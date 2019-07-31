---
title: EmbeddedSIMDeviceState の更新
description: EmbeddedSIMDeviceState オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2986858bd3ee2fa3cc54148f0c0354de360992cb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35990513"
---
# <a name="update-embeddedsimdevicestate"></a>EmbeddedSIMDeviceState の更新

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

[EmbeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)オブジェクトのプロパティを更新します。

## <a name="prerequisites"></a>前提条件
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類|アクセス許可 (特権の大きいものから小さいものへ)|
|:---|:---|
|委任 (職場または学校のアカウント)|DeviceManagementConfiguration.ReadWrite.All|
|委任 (個人用 Microsoft アカウント)|サポートされていません。|
|アプリケーション|サポートされていません。|

## <a name="http-request"></a>HTTP 要求
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates/{embeddedSIMDeviceStateId}
```

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー|値|
|:---|:---|
|Authorization|ベアラー &lt;トークン&gt; が必要です。|
|承諾|application/json|

## <a name="request-body"></a>要求本文
要求本文で、 [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)オブジェクトの JSON 表記を指定します。

次の表に、 [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)の作成時に必要なプロパティを示します。

|プロパティ|型|説明|
|:---|:---|:---|
|id|String|埋め込まれている SIM デバイスの状態を表す一意の識別子です。 作成時に割り当てられたシステム生成値。|
|createdDateTime|DateTimeOffset|埋め込み SIM デバイスの状態が作成された時刻。 サービス側を生成しました。|
|modifiedDateTime|DateTimeOffset|埋め込み SIM デバイスの状態が最後に変更された時刻。 サービス側を更新しました。|
|lastSyncDateTime|DateTimeOffset|埋め込まれた SIM デバイスが最後にチェックインされた時刻。 サービス側を更新しました。|
|universalIntegratedCircuitCardIdentifier|String|プロファイルが展開されるハードウェアを識別するユニバーサル統合回路カード識別子 (UICCID)。|
|deviceName|String|サブスクリプションが準備されたデバイス名 (デスクトップの例: JOE)|
|userName|String|サブスクリプションが準備されたユーザー名 (joe@contoso.com など)|
|state|[embeddedSIMDeviceStateValue](../resources/intune-esim-embeddedsimdevicestatevalue.md)|デバイスに適用されるプロファイル操作の状態。 可能な値は、`notEvaluated`、`failed`、`installing`、`installed`、`deleting`、`error`、`deleted`、`removedByUser` です。|
|stateDetails|String|プロビジョニング状態の文字列の説明。|



## <a name="response"></a>応答
成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)オブジェクトを返します。

## <a name="example"></a>例

### <a name="request"></a>要求
以下は、要求の例です。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates/{embeddedSIMDeviceStateId}
Content-type: application/json
Content-length: 361

{
  "@odata.type": "#microsoft.graph.embeddedSIMDeviceState",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "universalIntegratedCircuitCardIdentifier": "Universal Integrated Circuit Card Identifier value",
  "deviceName": "Device Name value",
  "userName": "User Name value",
  "state": "failed",
  "stateDetails": "State Details value"
}
```

### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 529

{
  "@odata.type": "#microsoft.graph.embeddedSIMDeviceState",
  "id": "908884a3-84a3-9088-a384-8890a3848890",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "universalIntegratedCircuitCardIdentifier": "Universal Integrated Circuit Card Identifier value",
  "deviceName": "Device Name value",
  "userName": "User Name value",
  "state": "failed",
  "stateDetails": "State Details value"
}
```





