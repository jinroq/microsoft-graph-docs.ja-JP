---
title: DeviceManagementScript を作成します。
description: 新しい deviceManagementScript オブジェクトを作成します。
ms.openlocfilehash: feb3463e679e77a1702a38f8cc7fd0edb28170d5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074010"
---
# <a name="create-devicemanagementscript"></a>DeviceManagementScript を作成します。

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

新しい[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)オブジェクトを作成します。
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
POST /deviceManagement/deviceManagementScripts
```

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー|値|
|:---|:---|
|Authorization|ベアラー &lt;トークン&gt; が必須。|
|Accept|application/json|

## <a name="request-body"></a>要求本文
要求の本文に deviceManagementScript オブジェクトの JSON の形式を指定します。

次の表は、deviceManagementScript を作成するときに必要なプロパティを示します。

|プロパティ|型|説明|
|:---|:---|:---|
|id|String|デバイス管理スクリプト用の一意の識別子。|
|displayName|String|デバイスの管理スクリプトの名前です。|
|説明|String|デバイスの管理スクリプトのオプションの説明です。|
|runSchedule|[runSchedule](../resources/intune-devices-runschedule.md)|スクリプトを実行する間隔です。 定義されていないスクリプトは実行 1 回|
|scriptContent|バイナリ|スクリプトの内容。|
|createdDateTime|DateTimeOffset|デバイス管理スクリプトが作成された日時です。|
|lastModifiedDateTime|DateTimeOffset|日付と時刻、デバイス管理のスクリプトが最後に修正されました。|
|runAsAccount|[runAsAccountType](../resources/intune-shared-runasaccounttype.md)|デバイス管理のスクリプトで実行される実行コンテキストの種類を示します。 使用可能な値は、`system`、`user` です。|
|enforceSignatureCheck|ブール値|スクリプト署名をチェックする必要があるかどうかを指定します。|
|fileName|String|スクリプト ファイルの名前です。|



## <a name="response"></a>応答
かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)オブジェクトです。

## <a name="example"></a>例
### <a name="request"></a>要求
以下は、要求の例です。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts
Content-type: application/json
Content-length: 422

{
  "@odata.type": "#microsoft.graph.deviceManagementScript",
  "displayName": "Display Name value",
  "description": "Description value",
  "runSchedule": {
    "@odata.type": "microsoft.graph.runSchedule"
  },
  "scriptContent": "c2NyaXB0Q29udGVudA==",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "runAsAccount": "user",
  "enforceSignatureCheck": true,
  "fileName": "File Name value"
}
```

### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 530

{
  "@odata.type": "#microsoft.graph.deviceManagementScript",
  "id": "59ea4525-4525-59ea-2545-ea592545ea59",
  "displayName": "Display Name value",
  "description": "Description value",
  "runSchedule": {
    "@odata.type": "microsoft.graph.runSchedule"
  },
  "scriptContent": "c2NyaXB0Q29udGVudA==",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "runAsAccount": "user",
  "enforceSignatureCheck": true,
  "fileName": "File Name value"
}
```





