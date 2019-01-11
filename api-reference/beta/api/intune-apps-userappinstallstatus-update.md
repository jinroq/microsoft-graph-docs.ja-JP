---
title: UserAppInstallStatus を更新します。
description: UserAppInstallStatus オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c9357d213c7a5acd9836fb3301b57d8d91979f55
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892471"
---
# <a name="update-userappinstallstatus"></a>UserAppInstallStatus を更新します。

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

[UserAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)オブジェクトのプロパティを更新します。
## <a name="prerequisites"></a>前提条件
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類|アクセス許可 (特権の大きいものから小さいものへ)|
|:---|:---|
|委任 (職場または学校のアカウント)|DeviceManagementApps.ReadWrite.All|
|委任 (個人用 Microsoft アカウント)|サポートされていません。|
|アプリケーション|サポートされていません。|

## <a name="http-request"></a>HTTP 要求
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}
```

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー|値|
|:---|:---|
|Authorization|ベアラー &lt;トークン&gt; が必須。|
|Accept|application/json|

## <a name="request-body"></a>要求本文
要求の本文に[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)オブジェクトの JSON の形式を指定します。

[UserAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)を作成するときに必要なプロパティを次の表に示します。

|プロパティ|種類|説明|
|:---|:---|:---|
|ID|String|エンティティのキー。|
|userName|String|ユーザー名です。|
|userPrincipalName|String|ユーザー プリンシパル名です。|
|installedDeviceCount|Int32|インストールされたデバイスの数です。|
|failedDeviceCount|Int32|失敗したデバイスの数です。|
|notInstalledDeviceCount|Int32|インストールされていないデバイスの数です。|



## <a name="response"></a>応答
かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)オブジェクトです。

## <a name="example"></a>例
### <a name="request"></a>要求
以下は、要求の例です。
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}
Content-type: application/json
Content-length: 180

{
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7
}
```

### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 288

{
  "@odata.type": "#microsoft.graph.userAppInstallStatus",
  "id": "14959a2a-9a2a-1495-2a9a-95142a9a9514",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7
}
```





