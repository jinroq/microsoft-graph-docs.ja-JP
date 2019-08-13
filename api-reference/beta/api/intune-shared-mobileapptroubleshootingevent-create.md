---
title: MobileAppTroubleshootingEvent を作成する
description: 複数のワークフローをサポートする Microsoft Graph API for Intune の Create mobileAppTroubleshootingEvent メソッドについて説明します。
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 241f31384d0e1c346659d5ac33b51acd4e2f3a6c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36350868"
---
# <a name="create-mobileapptroubleshootingevent"></a>MobileAppTroubleshootingEvent を作成する

> **重要:** Microsoft Graph の/ベータ版の Api は変更される可能性があります。 実稼働アプリケーションでは、これらの API の使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

新しい[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)オブジェクトを作成します。

## <a name="prerequisites"></a>前提条件
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類|アクセス許可 (特権の大きいものから小さいものへ)|
|:---|:---|
|委任 (職場または学校のアカウント)||
|&nbsp;&nbsp; **デバイスの管理**|DeviceManagementManagedDevices.ReadWrite.All|
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
|Authorization|ベアラー &lt;トークン&gt; が必要です。|
|承諾|application/json|

## <a name="request-body"></a>要求本文
要求本文で、mobileAppTroubleshootingEvent オブジェクトの JSON 表記を指定します。

次の表に、mobileAppTroubleshootingEvent の作成時に必要なプロパティを示します。

|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|オブジェクトの GUID|
|**トラブルシューティング**|
|additionalInformation|[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション|トラブルシューティングイベントに関する追加情報を提供する文字列キーと文字列値のペアのセット。|
|applicationId|文字列型 (String)|Intune アプリケーション識別子。|
|correlationId|String|サービスのエラーをトレースするために使用される ID。 |
|eventDateTime|DateTimeOffset|インシデントが発生した時間。 |
|eventName|String|トラブルシューティングイベントに対応するイベント名。 省略可能。|
|履歴|[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)コレクション|Intune モバイルアプリケーションのトラブルシューティングの履歴項目|
|managedDeviceIdentifier|String|Intune によって作成または収集されるデバイス識別子。|
|トラブルシューティングのエラーの詳細|[deviceManagementTroubleshootingErrorDetails](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|エラーとその修復に関する詳細情報を含むオブジェクト。 |
|userId|String|デバイスを登録しようとするユーザーの識別子。|

## <a name="response"></a>応答
成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)オブジェクトを返します。

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







