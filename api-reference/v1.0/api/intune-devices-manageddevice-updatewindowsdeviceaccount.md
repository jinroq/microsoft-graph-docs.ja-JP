---
title: updateWindowsDeviceAccount アクション
description: まだ文書化されていません
author: tfitzmac
ms.openlocfilehash: 9d7ae04e3fdbecdef75cbf905257510b5a6a893b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27356869"
---
# <a name="updatewindowsdeviceaccount-action"></a>updateWindowsDeviceAccount アクション

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

まだ文書化されていません
## <a name="prerequisites"></a>前提条件
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類|アクセス許可 (特権の大きいものから小さいものへ)|
|:---|:---|
|委任 (職場または学校のアカウント)|DeviceManagementManagedDevices.PriviligedOperation.All|
|委任 (個人用 Microsoft アカウント)|サポートされていません。|
|アプリケーション|サポートされていません。|

## <a name="http-request"></a>HTTP 要求
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount
POST /deviceManagement/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount
```

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー|値|
|:---|:---|
|Authorization|ベアラー &lt;トークン&gt; が必須。|
|Accept|application/json|

## <a name="request-body"></a>要求本文
要求本文で、パラメーターの JSON 表記を指定します。

次の表に、このアクションで使用できるパラメーターを示します。

|プロパティ|種類|説明|
|:---|:---|:---|
|updateWindowsDeviceAccountActionParameter|[updateWindowsDeviceAccountActionParameter](../resources/intune-devices-updatewindowsdeviceaccountactionparameter.md)|まだ文書化されていません|



## <a name="response"></a>応答
成功した場合、このアクションは `204 No Content` 応答コードを返します。

## <a name="example"></a>例
### <a name="request"></a>要求
以下は、要求の例です。
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/updateWindowsDeviceAccount

Content-type: application/json
Content-length: 532

{
  "updateWindowsDeviceAccountActionParameter": {
    "@odata.type": "microsoft.graph.updateWindowsDeviceAccountActionParameter",
    "deviceAccount": {
      "@odata.type": "microsoft.graph.windowsDeviceAccount",
      "password": "Password value"
    },
    "passwordRotationEnabled": true,
    "calendarSyncEnabled": true,
    "deviceAccountEmail": "Device Account Email value",
    "exchangeServer": "Exchange Server value",
    "sessionInitiationProtocalAddress": "Session Initiation Protocal Address value"
  }
}
```

### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
``` http
HTTP/1.1 204 No Content
```



