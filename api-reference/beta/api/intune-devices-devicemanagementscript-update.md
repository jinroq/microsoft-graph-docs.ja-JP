---
title: devicemanagementscript の更新
description: devicemanagementscript オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fafb11f61f6e98eba90de9054550e673b6d6cbdd
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30141791"
---
# <a name="update-devicemanagementscript"></a>devicemanagementscript の更新

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

[devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)オブジェクトのプロパティを更新します。

## <a name="prerequisites"></a>前提条件
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。

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
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
```

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー|値|
|:---|:---|
|Authorization|ベアラー &lt;トークン&gt; が必須。|
|承諾|application/json|

## <a name="request-body"></a>要求本文
要求本文で、 [devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)オブジェクトの JSON 表記を指定します。

次の表に、 [devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)の作成時に必要なプロパティを示します。

|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|デバイス管理スクリプトの一意識別子。|
|displayName|String|デバイス管理スクリプトの名前。|
|説明|文字列|デバイス管理スクリプトの省略可能な説明です。|
|runSchedule|[runSchedule](../resources/intune-devices-runschedule.md)|スクリプトを実行する間隔を指定します。 定義されていない場合、スクリプトは1回だけ実行されます。|
|scriptcontent|Binary|スクリプトの内容。|
|createdDateTime|DateTimeOffset|デバイス管理スクリプトが作成された日付と時刻。|
|lastModifiedDateTime|DateTimeOffset|デバイス管理スクリプトが最後に変更された日付と時刻。|
|runAsAccount|[runAsAccountType](../resources/intune-shared-runasaccounttype.md)|デバイス管理スクリプトを実行する実行コンテキストの種類を示します。 使用可能な値は、`system`、`user` です。|
|enforceSignatureCheck|ブール値|スクリプト署名をチェックする必要があるかどうかを示します。|
|fileName|String|スクリプトファイル名。|
|roleScopeTagIds|String collection|この powershellscript インスタンスの範囲タグ id のリスト。|
|runAs32Bit|ブール値|PowerShell スクリプトを32ビットとして実行する必要があるかどうかを示す値。|



## <a name="response"></a>応答
成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)オブジェクトを返します。

## <a name="example"></a>例

### <a name="request"></a>要求
以下は、要求の例です。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
Content-type: application/json
Content-length: 443

{
  "@odata.type": "#microsoft.graph.deviceManagementScript",
  "displayName": "Display Name value",
  "description": "Description value",
  "runSchedule": {
    "@odata.type": "microsoft.graph.runSchedule"
  },
  "scriptContent": "c2NyaXB0Q29udGVudA==",
  "runAsAccount": "user",
  "enforceSignatureCheck": true,
  "fileName": "File Name value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "runAs32Bit": true
}
```

### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 615

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
  "fileName": "File Name value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "runAs32Bit": true
}
```




