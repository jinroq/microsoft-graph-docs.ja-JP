---
title: targetedManagedAppConfiguration の作成
description: 新しい targetedManagedAppConfiguration オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ff469f57819db74f62ad0f300ecd13443be346ea
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35996561"
---
# <a name="create-targetedmanagedappconfiguration"></a>targetedManagedAppConfiguration の作成

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

新しい [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) オブジェクトを作成します。

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
POST /deviceAppManagement/targetedManagedAppConfigurations
```

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー|値|
|:---|:---|
|Authorization|ベアラー &lt;トークン&gt; が必要です。|
|承諾|application/json|

## <a name="request-body"></a>要求本文
要求本文で、targetedManagedAppConfiguration オブジェクトの JSON 表記を指定します。

次の表に、targetedManagedAppConfiguration の作成時に必要なプロパティを示します。

|プロパティ|型|説明|
|:---|:---|:---|
|displayName|String|ポリシーの表示名。 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します|
|description|String|ポリシーの説明。 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します|
|createdDateTime|DateTimeOffset|ポリシーが作成された日時。 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|ポリシーが変更された最終日時。 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します|
|id|文字列|エンティティのキー。 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します|
|version|String|エンティティのバージョン。 [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します|
|customSettings|[keyValuePair](../resources/intune-mam-keyvaluepair.md) コレクション|構成の対象であるユーザーに対して、このサービスで変更せずにアプリに送信される文字列キーと文字列値の一連のペア。[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) から継承します|
|deployedAppCount|Int32|現在のポリシーが配置されたアプリの数。|
|isAssigned|Boolean|包含グループにポリシーを配置するかどうかを示します。|



## <a name="response"></a>応答
成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) オブジェクトを返します。

## <a name="example"></a>例

### <a name="request"></a>要求
以下は、要求の例です。
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/targetedManagedAppConfigurations
Content-type: application/json
Content-length: 388

{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "version": "Version value",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "deployedAppCount": 0,
  "isAssigned": true
}
```

### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 560

{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "id": "2444e029-e029-2444-29e0-442429e04424",
  "version": "Version value",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "deployedAppCount": 0,
  "isAssigned": true
}
```



