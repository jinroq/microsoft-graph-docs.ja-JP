---
title: devicemanagementintentuserstate の作成
description: 新しい devicemanagementintentuserstate オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: aa3b718bbf0b4e87805a79066bfd6f898e47a0d8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507764"
---
# <a name="create-devicemanagementintentuserstate"></a>devicemanagementintentuserstate の作成

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

新しい[devicemanagementintentuserstate](../resources/intune-deviceintent-devicemanagementintentuserstate.md)オブジェクトを作成します。

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
POST /deviceManagement/intents/{deviceManagementIntentId}/userStates
```

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー|値|
|:---|:---|
|Authorization|ベアラー &lt;トークン&gt; が必要です。|
|承諾|application/json|

## <a name="request-body"></a>要求本文
要求本文で、devicemanagementintentuserstate オブジェクトの JSON 表記を指定します。

次の表に、devicemanagementintentuserstate の作成時に必要なプロパティを示します。

|プロパティ|型|説明|
|:---|:---|:---|
|id|String|ID|
|userPrincipalName|String|デバイスで報告されているユーザープリンシパル名|
|userName|String|デバイスで報告されているユーザー名|
|deviceCount|Int32|目的のためにユーザーに属しているデバイスの数|
|lastReportedDateTime|DateTimeOffset|インテントレポートの最終更新日時|
|state|[complianceStatus](../resources/intune-shared-compliancestatus.md)|目的のユーザー状態。 可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。|



## <a name="response"></a>応答
成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[devicemanagementintentuserstate](../resources/intune-deviceintent-devicemanagementintentuserstate.md)オブジェクトを返します。

## <a name="example"></a>例

### <a name="request"></a>要求
以下は、要求の例です。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/userStates
Content-type: application/json
Content-length: 275

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentUserState",
  "userPrincipalName": "User Principal Name value",
  "userName": "User Name value",
  "deviceCount": 11,
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "state": "notApplicable"
}
```

### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 324

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentUserState",
  "id": "0201286a-286a-0201-6a28-01026a280102",
  "userPrincipalName": "User Principal Name value",
  "userName": "User Name value",
  "deviceCount": 11,
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "state": "notApplicable"
}
```





