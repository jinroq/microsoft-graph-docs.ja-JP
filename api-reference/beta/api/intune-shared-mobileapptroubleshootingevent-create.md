---
title: MobileAppTroubleshootingEvent を作成します。
description: Intune は、複数のワークフローをサポートするための Microsoft グラフ API を作成する mobileAppTroubleshootingEvent メソッドを説明します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e409aa663ff2471222a7e36a9e381505792f37eb
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431636"
---
# <a name="create-mobileapptroubleshootingevent"></a>MobileAppTroubleshootingEvent を作成します。

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

新しい[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)オブジェクトを作成します。

## <a name="prerequisites"></a>前提条件
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。

|アクセス許可の種類|アクセス許可 (特権の大きいものから小さいものへ)|
|:---|:---|
|委任 (職場または学校のアカウント)||
|&nbsp; &nbsp; **デバイスの管理**|DeviceManagementManagedDevices.ReadWrite.All|
|&nbsp; &nbsp; **トラブルシューティング**|DeviceManagementManagedDevices.ReadWrite.All|
|委任 (個人用 Microsoft アカウント)|サポートされていません。|
|アプリケーション|サポートされていません。|

## <a name="http-request"></a>HTTP 要求
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileAppTroubleshootingEvents
POST /users/{usersId}/mobileAppTroubleshootingEvents
```

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー|値|
|:---|:---|
|Authorization|ベアラー &lt;トークン&gt; が必須。|
|Accept|application/json|

## <a name="request-body"></a>要求本文
要求の本文に mobileAppTroubleshootingEvent オブジェクトの JSON の形式を指定します。

次の表は、mobileAppTroubleshootingEvent を作成するときに必要なプロパティを示します。

|プロパティ|型|説明|
|:---|:---|:---|
|id|String|オブジェクトの GUID|
|**トラブルシューティング**|
|について|[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション|トラブルシューティング イベントに関する追加情報を提供する文字列キーと文字列値のペアのセットです。|
|applicationId|文字列型 (String)|Intune アプリケーション識別子です。|
|correlationId|String|サービスでエラーのトレースに使用される ID です。 |
|eventDateTime|DateTimeOffset|インシデントが発生した時間。 |
|eventName|String|トラブルシューティング イベントに対応するイベントの名前です。 省略可能。|
|履歴|[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)コレクション|Intune モバイル アプリケーションの履歴項目のトラブルシューティング|
|managedDeviceIdentifier|String|Intune によって作成または収集されるデバイス識別子。|
|troubleshootingErrorDetails|[deviceManagementTroubleshootingErrorDetails](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|エラーとその修復に関する詳細情報を含むオブジェクトです。 |
|userId|String|デバイスを登録しようとするユーザーの識別子。|

## <a name="response"></a>応答
かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)オブジェクトです。

## <a name="example"></a>例

### <a name="request"></a>要求
以下は、要求の例です。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents
Content-type: application/json
Content-length: 71

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent"
}
```

### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 120

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
  "id": "77943c10-3c10-7794-103c-9477103c9477"
}
```




