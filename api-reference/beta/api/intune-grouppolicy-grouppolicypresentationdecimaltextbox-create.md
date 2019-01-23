---
title: GroupPolicyPresentationDecimalTextBox を作成します。
description: 新しい groupPolicyPresentationDecimalTextBox オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1cc6e5cb8104cc4d9ff4cffcf2157fe954f991cf
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430437"
---
# <a name="create-grouppolicypresentationdecimaltextbox"></a>GroupPolicyPresentationDecimalTextBox を作成します。

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

新しい[groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)オブジェクトを作成します。

## <a name="prerequisites"></a>前提条件
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。

|アクセス許可の種類|アクセス許可 (特権の大きいものから小さいものへ)|
|:---|:---|
|委任 (職場または学校のアカウント)|DeviceManagementServiceConfig.ReadWrite.All|
|委任 (個人用 Microsoft アカウント)|サポートされていません。|
|アプリケーション|サポートされていません。|

## <a name="http-request"></a>HTTP 要求
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー|値|
|:---|:---|
|Authorization|ベアラー &lt;トークン&gt; が必須。|
|Accept|application/json|

## <a name="request-body"></a>要求本文
要求の本文に groupPolicyPresentationDecimalTextBox オブジェクトの JSON の形式を指定します。

次の表は、groupPolicyPresentationDecimalTextBox を作成するときに必要なプロパティを示します。

|プロパティ|型|説明|
|:---|:---|:---|
|label|String|プレゼンテーションの任意のエンティティのローカライズされたテキスト ラベルです。 既定値は空です。 [GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承されました。|
|id|String|エンティティのキー。 [GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承されました。|
|lastModifiedDateTime|DateTimeOffset|日付と時刻、エンティティが最後に修正されました。 [GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承されました。|
|defaultValue|Int64|符号なし整数を 10 進数のテキスト ボックスの初期値を指定します。 既定値は 1 です。|
|スピン|Boolean|True の場合、スピン コントロールを作成します。それ以外の場合、数値入力用のテキスト ボックスを作成します。 既定値は、true を指定します。|
|spinStep|Int64|スピン コントロールの変更の増分値を指定する符号なし整数。 既定値は 1 です。|
|必須|Boolean|パラメーター] ボックスに値を入力するための要件です。 既定値は、false を指定します。|
|minValue|Int64|指定できる最小の値を指定する符号なし整数。 既定値は 0 です。|
|maxValue|Int64|最大許容値を指定する符号なし整数。 既定値は、9999 です。|



## <a name="response"></a>応答
かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)オブジェクトです。

## <a name="example"></a>例

### <a name="request"></a>要求
以下は、要求の例です。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
Content-type: application/json
Content-length: 221

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationDecimalTextBox",
  "label": "Label value",
  "defaultValue": 12,
  "spin": true,
  "spinStep": 8,
  "required": true,
  "minValue": 8,
  "maxValue": 8
}
```

### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 334

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationDecimalTextBox",
  "label": "Label value",
  "id": "988daea7-aea7-988d-a7ae-8d98a7ae8d98",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "defaultValue": 12,
  "spin": true,
  "spinStep": 8,
  "required": true,
  "minValue": 8,
  "maxValue": 8
}
```




