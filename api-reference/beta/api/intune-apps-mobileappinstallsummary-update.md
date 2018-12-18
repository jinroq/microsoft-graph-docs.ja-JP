---
title: MobileAppInstallSummary を更新します。
description: MobileAppInstallSummary オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: 94dc7fa5023d26de91b4d64efda27332dd51de63
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27315639"
---
# <a name="update-mobileappinstallsummary"></a>MobileAppInstallSummary を更新します。

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

[MobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)オブジェクトのプロパティを更新します。
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
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/installSummary
```

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー|値|
|:---|:---|
|Authorization|ベアラー &lt;トークン&gt; が必須。|
|Accept|application/json|

## <a name="request-body"></a>要求本文
要求の本文に[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)オブジェクトの JSON の形式を指定します。

[MobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)を作成するときに必要なプロパティを次の表に示します。

|プロパティ|種類|説明|
|:---|:---|:---|
|ID|String|エンティティのキー。|
|installedDeviceCount|Int32|このアプリケーションを正常にインストールするデバイスの数です。|
|failedDeviceCount|Int32|このアプリケーションのインストールに失敗したデバイスの数。|
|notApplicableDeviceCount|Int32|このアプリケーションには適用されていないデバイスの数です。|
|notInstalledDeviceCount|Int32|このアプリケーションをインストールしていないデバイスの数。|
|pendingInstallDeviceCount|Int32|このアプリケーションをインストールするのには通知しているデバイスの数です。|
|installedUserCount|Int32|このアプリケーションをインストールするのにはデバイスがすべて成功しているユーザーの数です。|
|failedUserCount|Int32|1 を持っているユーザー、またはこのアプリケーションのインストールに失敗した複数のデバイスの数です。|
|notApplicableUserCount|Int32|デバイスがなかったすべてこのアプリケーションに適用可能なユーザーの数です。|
|notInstalledUserCount|Int32|このアプリケーションがインストールされていない 1 つ以上のデバイスを持っているユーザーの数です。|
|pendingInstallUserCount|Int32|1 を持っているユーザー、またはこのアプリケーションをインストールし、0 のデバイス障害を通知している複数のデバイスの数です。|



## <a name="response"></a>応答
かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)オブジェクトです。

## <a name="example"></a>例
### <a name="request"></a>要求
以下は、要求の例です。
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/installSummary
Content-type: application/json
Content-length: 312

{
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notApplicableDeviceCount": 8,
  "notInstalledDeviceCount": 7,
  "pendingInstallDeviceCount": 9,
  "installedUserCount": 2,
  "failedUserCount": 15,
  "notApplicableUserCount": 6,
  "notInstalledUserCount": 5,
  "pendingInstallUserCount": 7
}
```

### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 423

{
  "@odata.type": "#microsoft.graph.mobileAppInstallSummary",
  "id": "06a792e9-92e9-06a7-e992-a706e992a706",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notApplicableDeviceCount": 8,
  "notInstalledDeviceCount": 7,
  "pendingInstallDeviceCount": 9,
  "installedUserCount": 2,
  "failedUserCount": 15,
  "notApplicableUserCount": 6,
  "notInstalledUserCount": 5,
  "pendingInstallUserCount": 7
}
```





