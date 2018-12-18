---
title: RestrictedAppsViolation を作成します。
description: 新しい restrictedAppsViolation オブジェクトを作成します。
author: tfitzmac
ms.openlocfilehash: 3f20463363c37e8ab9ed47bebb3b2323ca308656
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27313329"
---
# <a name="create-restrictedappsviolation"></a>RestrictedAppsViolation を作成します。

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

新しい[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)オブジェクトを作成します。
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
POST /deviceManagement/deviceConfigurationRestrictedAppsViolations
```

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー|値|
|:---|:---|
|Authorization|ベアラー &lt;トークン&gt; が必須。|
|Accept|application/json|

## <a name="request-body"></a>要求本文
要求の本文に restrictedAppsViolation オブジェクトの JSON の形式を指定します。

次の表は、restrictedAppsViolation を作成するときに必要なプロパティを示します。

|プロパティ|種類|説明|
|:---|:---|:---|
|ID|String|オブジェクトの一意の識別子です。 "Accountid"、deviceId、policyId、およびユーザー Id から構成されます。|
|userId|String|ユーザーの一意の識別子の Guid にする必要があります。|
|userName|String|ユーザー名|
|managedDeviceId|String|管理対象デバイスの一意の識別子の Guid にする必要があります。|
|deviceName|String|デバイス名|
|deviceConfigurationId|String|デバイス構成プロファイルの一意の識別子の Guid にする必要があります。|
|deviceConfigurationName|String|デバイス構成のプロファイル名|
|platformType|[policyPlatformType](../resources/intune-deviceconfig-policyplatformtype.md)|プラットフォームの種類。 可能な値は、`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`all` です。|
|restrictedAppsState|[restrictedAppsState](../resources/intune-deviceconfig-restrictedappsstate.md)|アプリケーションの状態を制限します。 使用可能な値は、`prohibitedApps`、`notApprovedApps` です。|
|restrictedApps|[managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md)コレクション|違反した制限されたアプリケーションの一覧|



## <a name="response"></a>応答
かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)オブジェクトです。

## <a name="example"></a>例
### <a name="request"></a>要求
以下は、要求の例です。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationRestrictedAppsViolations
Content-type: application/json
Content-length: 564

{
  "@odata.type": "#microsoft.graph.restrictedAppsViolation",
  "userId": "User Id value",
  "userName": "User Name value",
  "managedDeviceId": "Managed Device Id value",
  "deviceName": "Device Name value",
  "deviceConfigurationId": "Device Configuration Id value",
  "deviceConfigurationName": "Device Configuration Name value",
  "platformType": "androidForWork",
  "restrictedAppsState": "notApprovedApps",
  "restrictedApps": [
    {
      "@odata.type": "microsoft.graph.managedDeviceReportedApp",
      "appId": "App Id value"
    }
  ]
}
```

### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 613

{
  "@odata.type": "#microsoft.graph.restrictedAppsViolation",
  "id": "53f99903-9903-53f9-0399-f9530399f953",
  "userId": "User Id value",
  "userName": "User Name value",
  "managedDeviceId": "Managed Device Id value",
  "deviceName": "Device Name value",
  "deviceConfigurationId": "Device Configuration Id value",
  "deviceConfigurationName": "Device Configuration Name value",
  "platformType": "androidForWork",
  "restrictedAppsState": "notApprovedApps",
  "restrictedApps": [
    {
      "@odata.type": "microsoft.graph.managedDeviceReportedApp",
      "appId": "App Id value"
    }
  ]
}
```





