---
title: devicemanagementcollectionsettingdefinition の更新
description: devicemanagementcollectionsettingdefinition オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0839e2be1a39da448c9bb9146cea3b06bc6511e1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32509843"
---
# <a name="update-devicemanagementcollectionsettingdefinition"></a>devicemanagementcollectionsettingdefinition の更新

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

[devicemanagementcollectionsettingdefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md)オブジェクトのプロパティを更新します。

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
要求本文で、 [devicemanagementcollectionsettingdefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md)オブジェクトの JSON 表記を指定します。

次の表に、 [devicemanagementcollectionsettingdefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md)の作成時に必要なプロパティを示します。

|プロパティ|型|説明|
|:---|:---|:---|
|id|String|[devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)から継承された設定定義の ID|
|valueType|[deviceManangementIntentValueType](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|[devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)から継承された値のデータ型。 可能な値は `integer`、`boolean`、`string`、`complex`、`collection`、`abstractComplex` です。|
|displayName|String|[devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)から継承された設定の表示名|
|isTopLevel|Boolean|設定が最上位レベルの場合は、 [devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)から継承されたコレクションまたは複雑な設定でラップする必要がなく、構成することができます。|
|説明|String|[devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)から継承された設定の説明|
|documentation url|String|[devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)から継承されたドキュメントを設定するための Url|
|keywords|String collection|[devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)から継承した設定に関連付けられているキーワード|
|式|[devicemanagementconstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)コレクション|[devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)から継承された設定値の制約のコレクション|
|ヲ|[devicemanagementsettingdependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md)コレクション|[devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)から継承された他の設定に対する依存関係のコレクション|
|elementDefinitionId|String|コレクションの各要素がどのようなものかを示す設定定義 ID。|



## <a name="response"></a>応答
成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[devicemanagementcollectionsettingdefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md)オブジェクトを返します。

## <a name="example"></a>例

### <a name="request"></a>要求
以下は、要求の例です。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/settingDefinitions/{deviceManagementSettingDefinitionId}
Content-type: application/json
Content-length: 795

{
  "@odata.type": "#microsoft.graph.deviceManagementCollectionSettingDefinition",
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
  ],
  "elementDefinitionId": "Element Definition Id value"
}
```

### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 844

{
  "@odata.type": "#microsoft.graph.deviceManagementCollectionSettingDefinition",
  "id": "0419c4a7-c4a7-0419-a7c4-1904a7c41904",
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
  ],
  "elementDefinitionId": "Element Definition Id value"
}
```





