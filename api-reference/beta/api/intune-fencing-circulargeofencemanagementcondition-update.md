---
title: CircularGeofenceManagementCondition の更新
description: CircularGeofenceManagementCondition オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 75e653dd1152de9bbb57beea00af65572bc8dda4
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36355655"
---
# <a name="update-circulargeofencemanagementcondition"></a>CircularGeofenceManagementCondition の更新

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

[CircularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)オブジェクトのプロパティを更新します。

## <a name="prerequisites"></a>前提条件
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類|アクセス許可 (特権の大きいものから小さいものへ)|
|:---|:---|
|委任 (職場または学校のアカウント)|DeviceManagementConfiguration.ReadWrite.All|
|委任 (個人用 Microsoft アカウント)|サポートされていません。|
|アプリケーション|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP 要求
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managementConditions/{managementConditionId}
PATCH /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー|値|
|:---|:---|
|Authorization|ベアラー &lt;トークン&gt; が必要です。|
|承諾|application/json|

## <a name="request-body"></a>要求本文
要求本文で、 [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)オブジェクトの JSON 表記を指定します。

次の表に、 [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)の作成時に必要なプロパティを示します。

|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|管理条件の一意識別子。 作成時に割り当てられたシステム生成値。 [Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します|
|uniqueName|String|管理条件の一意の名前。 管理条件式で使用されます。 [Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します|
|displayName|String|管理条件の管理者定義の名前。 [Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します|
|description|String|管理条件の管理者定義の説明。 [Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します|
|createdDateTime|DateTimeOffset|管理条件が作成された時刻。 サービス側を生成しました。 [Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します|
|modifiedDateTime|DateTimeOffset|管理条件が最後に変更された時刻。 サービス側を更新しました。 [Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します|
|eTag|String|管理条件の ETag。 サービス側を更新しました。 [Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します|
|アプリケーションのプラットフォーム|[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)コレクション|この管理条件の適用可能なプラットフォーム。 [Managementcondition](../resources/intune-fencing-managementcondition.md)から継承されます。 可能な値は、`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`unknown` です。|
|latitude|2 行分|緯度 (度は-90 と + 90 を含む)。|
|longitude|Double|角度 (単位は-180 と + 180 を含む)。|
|radiusInMeters|1 行|半径 (メートル単位)。|



## <a name="response"></a>応答
成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)オブジェクトを返します。

## <a name="example"></a>例

### <a name="request"></a>要求
以下は、要求の例です。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managementConditions/{managementConditionId}
Content-type: application/json
Content-length: 444

{
  "@odata.type": "#microsoft.graph.circularGeofenceManagementCondition",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "latitude": "<Unknown Primitive Type Edm.Double>",
  "longitude": "<Unknown Primitive Type Edm.Double>",
  "radiusInMeters": "<Unknown Primitive Type Edm.Single>"
}
```

### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 612

{
  "@odata.type": "#microsoft.graph.circularGeofenceManagementCondition",
  "id": "30ee27b6-27b6-30ee-b627-ee30b627ee30",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "latitude": "<Unknown Primitive Type Edm.Double>",
  "longitude": "<Unknown Primitive Type Edm.Double>",
  "radiusInMeters": "<Unknown Primitive Type Edm.Single>"
}
```






