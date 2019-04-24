---
title: devicemanagementsettingdefinition の更新
description: devicemanagementsettingdefinition オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f11167524956ff3eddc9a5508fb30fdd81e2aa73
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32466736"
---
# <a name="update-devicemanagementsettingdefinition"></a>devicemanagementsettingdefinition の更新

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

[devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)オブジェクトのプロパティを更新します。

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
PATCH /deviceManagement/settingDefinitions/{deviceManagementSettingDefinitionId}
PATCH /deviceManagement/categories/{deviceManagementSettingCategoryId}/settingDefinitions/{deviceManagementSettingDefinitionId}
PATCH /deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}/settingDefinitions/{deviceManagementSettingDefinitionId}
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}/settingDefinitions/{deviceManagementSettingDefinitionId}
```

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー|値|
|:---|:---|
|Authorization|ベアラー &lt;トークン&gt; が必要です。|
|承諾|application/json|

## <a name="request-body"></a>要求本文
要求本文で、 [devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)オブジェクトの JSON 表記を指定します。

次の表に、 [devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)の作成時に必要なプロパティを示します。

|プロパティ|型|説明|
|:---|:---|:---|
|id|String|設定定義の ID|
|valueType|[deviceManangementIntentValueType](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|値のデータ型。 可能な値は `integer`、`boolean`、`string`、`complex`、`collection`、`abstractComplex` です。|
|displayName|String|設定の表示名|
|isTopLevel|Boolean|設定が最上位レベルの場合は、コレクションまたは複雑な設定でラップする必要がなく構成できます。|
|説明|String|設定の説明|
|documentation url|String|ドキュメントを設定するための Url|
|keywords|String collection|設定に関連付けられているキーワード|
|式|[devicemanagementconstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)コレクション|設定値の制約のコレクション|
|ヲ|[devicemanagementsettingdependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md)コレクション|他の設定に対する依存関係のコレクション|



## <a name="response"></a>応答
成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)オブジェクトを返します。

## <a name="example"></a>例

### <a name="request"></a>要求
以下は、要求の例です。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/settingDefinitions/{deviceManagementSettingDefinitionId}
Content-type: application/json
Content-length: 728

{
  "@odata.type": "#microsoft.graph.deviceManagementSettingDefinition",
  "valueType": "boolean",
  "displayName": "Display Name value",
  "isTopLevel": true,
  "description": "Description value",
  "documentationUrl": "https://example.com/documentationUrl/",
  "keywords": [
    "Keywords value"
  ],
  "constraints": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingXmlConstraint"
    }
  ],
  "dependencies": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingDependency",
      "definitionId": "Definition Id value",
      "constraints": [
        {
          "@odata.type": "microsoft.graph.deviceManagementSettingXmlConstraint"
        }
      ]
    }
  ]
}
```

### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 777

{
  "@odata.type": "#microsoft.graph.deviceManagementSettingDefinition",
  "id": "4ec3093d-093d-4ec3-3d09-c34e3d09c34e",
  "valueType": "boolean",
  "displayName": "Display Name value",
  "isTopLevel": true,
  "description": "Description value",
  "documentationUrl": "https://example.com/documentationUrl/",
  "keywords": [
    "Keywords value"
  ],
  "constraints": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingXmlConstraint"
    }
  ],
  "dependencies": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingDependency",
      "definitionId": "Definition Id value",
      "constraints": [
        {
          "@odata.type": "microsoft.graph.deviceManagementSettingXmlConstraint"
        }
      ]
    }
  ]
}
```





