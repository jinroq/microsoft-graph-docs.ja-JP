---
title: DeviceHealthScript を作成する
description: 新しい deviceHealthScript オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0084852f4c0cb236931ee532f12e54a08c1e2fc2
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36311717"
---
# <a name="create-devicehealthscript"></a>DeviceHealthScript を作成する

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

新しい[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)オブジェクトを作成します。

## <a name="prerequisites"></a>前提条件
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類|アクセス許可 (特権の大きいものから小さいものへ)|
|:---|:---|
|委任 (職場または学校のアカウント)|DeviceManagementManagedDevices.ReadWrite.All|
|委任 (個人用 Microsoft アカウント)|サポートされていません。|
|アプリケーション|DeviceManagementManagedDevices.ReadWrite.All|

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
|Authorization|ベアラー &lt;トークン&gt; が必要です。|
|承諾|application/json|

## <a name="request-body"></a>要求本文
要求本文で、deviceHealthScript オブジェクトの JSON 表記を指定します。

次の表に、deviceHealthScript の作成時に必要なプロパティを示します。

|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|デバイス管理スクリプトの一意識別子。 [Devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)から継承します|
|displayName|String|デバイス管理スクリプトの名前。 [Devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)から継承します|
|description|String|デバイス管理スクリプトの省略可能な説明です。 [Devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)から継承します|
|runSchedule|[runSchedule](../resources/intune-devices-runschedule.md)|スクリプトを実行する間隔を指定します。 定義されていない場合、スクリプトは[Devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)から継承された後に実行されます|
|scriptContent|Binary|スクリプトの内容。 [Devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)から継承します|
|createdDateTime|DateTimeOffset|デバイス管理スクリプトが作成された日付と時刻。 [Devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)から継承します|
|lastModifiedDateTime|DateTimeOffset|デバイス管理スクリプトが最後に変更された日付と時刻。 [Devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)から継承します|
|runAsAccount|[runAsAccountType](../resources/intune-shared-runasaccounttype.md)|実行コンテキストの種類を示します。 [Devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)から継承されます。 可能な値は、`system`、`user` です。|
|enforceSignatureCheck|Boolean|スクリプト署名をチェックする必要があるかどうかを示します。 [Devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)から継承します|
|fileName|String|スクリプトファイル名。 [Devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)から継承します|
|roleScopeTagIds|文字列コレクション|この PowerShellScript インスタンスの範囲タグ Id のリスト。 [Devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)から継承します|
|runAs32Bit|Boolean|PowerShell スクリプトを[Devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)から継承した32ビットとして実行する必要があるかどうかを示す値。|
|complianceRule|[deviceHealthScriptComplianceRule](../resources/intune-devices-devicehealthscriptcompliancerule.md)|まだ文書化されていません|
|remediationScriptContent|Binary|まだ文書化されていません|
|runRemediationScript|ブール型 (Boolean)|まだ文書化されていません|



## <a name="response"></a>応答
成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)オブジェクトを返します。

## <a name="example"></a>例

### <a name="request"></a>要求
以下は、要求の例です。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts
Content-type: application/json
Content-length: 745

{
  "@odata.type": "#microsoft.graph.deviceHealthScript",
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
  "runAs32Bit": true,
  "complianceRule": {
    "@odata.type": "microsoft.graph.deviceHealthScriptComplianceRule",
    "detectionType": "string",
    "operator": "equal",
    "detectionValue": "Detection Value value"
  },
  "remediationScriptContent": "cmVtZWRpYXRpb25TY3JpcHRDb250ZW50",
  "runRemediationScript": true
}
```

### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 917

{
  "@odata.type": "#microsoft.graph.deviceHealthScript",
  "id": "bcb60502-0502-bcb6-0205-b6bc0205b6bc",
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
  "runAs32Bit": true,
  "complianceRule": {
    "@odata.type": "microsoft.graph.deviceHealthScriptComplianceRule",
    "detectionType": "string",
    "operator": "equal",
    "detectionValue": "Detection Value value"
  },
  "remediationScriptContent": "cmVtZWRpYXRpb25TY3JpcHRDb250ZW50",
  "runRemediationScript": true
}
```






