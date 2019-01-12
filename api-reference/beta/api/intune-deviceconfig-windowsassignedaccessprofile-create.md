---
title: WindowsAssignedAccessProfile を作成します。
description: 新しい windowsAssignedAccessProfile オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2313dff2c2f387e0a981775e0b6cc6e53a988f3f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956347"
---
# <a name="create-windowsassignedaccessprofile"></a>WindowsAssignedAccessProfile を作成します。

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

新しい[windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md)オブジェクトを作成します。
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
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/assignedAccessMultiModeProfiles
```

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー|値|
|:---|:---|
|Authorization|ベアラー &lt;トークン&gt; が必須。|
|Accept|application/json|

## <a name="request-body"></a>要求本文
要求の本文に windowsAssignedAccessProfile オブジェクトの JSON の形式を指定します。

次の表は、windowsAssignedAccessProfile を作成するときに必要なプロパティを示します。

|プロパティ|型|説明|
|:---|:---|:---|
|ID|String|エンティティのキー。|
|profilename プロパティ|String|これは、[スタート] メニューの [このプレゼンテーションの構成が割り当てられているユーザーにこれらのアプリケーションのレイアウト、アプリケーションのグループを識別するために使用するフレンドリ名です。|
|showTaskBar|Boolean|この設定では、タスク バーを表示するかどうかを指定するのには管理ができます。|
|appUserModelIds|String コレクション|これらは、[スタート] メニューから起動できる唯一の Windows ストア アプリです。|
|desktopAppPaths|String コレクション|これらは、[スタート] メニューで利用可能なデスクトップ アプリケーションのパスと、唯一のアプリケーション、ユーザーが起動できるようです。|
|ユーザー アカウント|String コレクション|この構成にキオスクがロックアウトされているユーザー アカウントです。|
|startMenuLayoutXml|Binary|開始の既定のレイアウトを変更するのには管理者は、ユーザーが変更できないようにします。レイアウトを変更するには、レイアウト変更スキーマに基づく XML ファイルを指定します。 XML は、バイナリ形式である必要があります。|



## <a name="response"></a>応答
かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md)オブジェクトです。

## <a name="example"></a>例
### <a name="request"></a>要求
以下は、要求の例です。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/assignedAccessMultiModeProfiles
Content-type: application/json
Content-length: 364

{
  "@odata.type": "#microsoft.graph.windowsAssignedAccessProfile",
  "profileName": "Profile Name value",
  "showTaskBar": true,
  "appUserModelIds": [
    "App User Model Ids value"
  ],
  "desktopAppPaths": [
    "Desktop App Paths value"
  ],
  "userAccounts": [
    "User Accounts value"
  ],
  "startMenuLayoutXml": "c3RhcnRNZW51TGF5b3V0WG1s"
}
```

### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 413

{
  "@odata.type": "#microsoft.graph.windowsAssignedAccessProfile",
  "id": "cfa70299-0299-cfa7-9902-a7cf9902a7cf",
  "profileName": "Profile Name value",
  "showTaskBar": true,
  "appUserModelIds": [
    "App User Model Ids value"
  ],
  "desktopAppPaths": [
    "Desktop App Paths value"
  ],
  "userAccounts": [
    "User Accounts value"
  ],
  "startMenuLayoutXml": "c3RhcnRNZW51TGF5b3V0WG1s"
}
```





