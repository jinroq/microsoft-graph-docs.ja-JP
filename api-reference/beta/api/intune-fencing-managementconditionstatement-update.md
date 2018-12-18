---
title: ManagementConditionStatement を更新します。
description: ManagementConditionStatement オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: 56de75540fa774f32fab7b6edf2795f3ac0d5351
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27333447"
---
# <a name="update-managementconditionstatement"></a>ManagementConditionStatement を更新します。

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

[ManagementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)オブジェクトのプロパティを更新します。
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
PATCH /deviceManagement/managementConditionStatements/{managementConditionStatementId}
PATCH /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}
```

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー|値|
|:---|:---|
|Authorization|ベアラー &lt;トークン&gt; が必須。|
|Accept|application/json|

## <a name="request-body"></a>要求本文
要求の本文に[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)オブジェクトの JSON の形式を指定します。

[ManagementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)を作成するときに必要なプロパティを次の表に示します。

|プロパティ|種類|説明|
|:---|:---|:---|
|ID|String|管理条件付きステートメントの一意の識別子です。 システムでは、作成時に割り当てられた値が生成されます。|
|displayName|String|管理者は、管理条件ステートメントの名前を定義します。|
|説明|String|管理者は、管理条件付きステートメントの説明を定義します。|
|createdDateTime|DateTimeOffset|管理条件付きステートメントが作成された時刻。 サービス側が生成されます。|
|変更された日時|DateTimeOffset|管理条件付きステートメントが最後に修正された時間です。 サービス側を更新します。|
|式|[managementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)|場合は、管理条件ステートメントを評価するために使用、管理条件ステートメントの式は、アクティブ/非アクティブでした。|
|eTag|String|管理条件付きステートメントの ETag。 サービス側を更新します。|
|applicablePlatforms|[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)コレクション|この管理条件ステートメントに適用可能なプラットフォームです。
管理に関連付けられている管理の条件を見てからこの計算は、ステートメントと該当するプラットフォームの交点の検出の条件です。 可能な値は、`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile` です。|



## <a name="response"></a>応答
かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)オブジェクトです。

## <a name="example"></a>例
### <a name="request"></a>要求
以下は、要求の例です。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managementConditionStatements/{managementConditionStatementId}
Content-type: application/json
Content-length: 256

{
  "displayName": "Display Name value",
  "description": "Description value",
  "expression": {
    "@odata.type": "microsoft.graph.managementConditionExpression"
  },
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ]
}
```

### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 491

{
  "@odata.type": "#microsoft.graph.managementConditionStatement",
  "id": "bedb0c00-0c00-bedb-000c-dbbe000cdbbe",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "expression": {
    "@odata.type": "microsoft.graph.managementConditionExpression"
  },
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ]
}
```





