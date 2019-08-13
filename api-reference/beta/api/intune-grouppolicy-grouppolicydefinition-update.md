---
title: GroupPolicyDefinition の更新
description: GroupPolicyDefinition オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 16fa748397dc08410f651a2179aa8737121aa1fb
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36355151"
---
# <a name="update-grouppolicydefinition"></a>GroupPolicyDefinition の更新

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

[Grouppolicydefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)オブジェクトのプロパティを更新します。

## <a name="prerequisites"></a>前提条件
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類|アクセス許可 (特権の大きいものから小さいものへ)|
|:---|:---|
|委任 (職場または学校のアカウント)|DeviceManagementServiceConfig.ReadWrite.All|
|委任 (個人用 Microsoft アカウント)|サポートされていません。|
|アプリケーション|DeviceManagementServiceConfig.ReadWrite.All|

## <a name="http-request"></a>HTTP 要求
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyDefinitions/{groupPolicyDefinitionId}
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/definition
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile/definitions/{groupPolicyDefinitionId}
```

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー|値|
|:---|:---|
|Authorization|ベアラー &lt;トークン&gt; が必要です。|
|承諾|application/json|

## <a name="request-body"></a>要求本文
要求本文で、 [Grouppolicydefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)オブジェクトの JSON 表記を指定します。

次の表に、 [Grouppolicydefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)の作成時に必要なプロパティを示します。

|プロパティ|型|説明|
|:---|:---|:---|
|classType|[groupPolicyDefinitionClassType](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|ポリシーを適用できるグループの種類を指定します。 可能な値は、`user`、`machine` です。|
|displayName|String|ローカライズされたポリシー名。|
|explainText|String|ポリシーに関連付けられたローカライズされた説明またはヘルプテキスト。 既定値は空白です。|
|categoryPath|String|ポリシーのローカライズされた完全なカテゴリのパス。|
|supportedOn|String|ポリシーによって影響を受けるオペレーティングシステムまたはアプリケーションのバージョンを指定するために使用されるローカライズされた文字列。|
|Msrtcsip-policytype|[groupPolicyType](../resources/intune-grouppolicy-grouppolicytype.md)|グループポリシーの種類を指定します。 可能な値は、`admxBacked`、`admxIngested` です。|
|id|文字列|エンティティのキー。|
|lastModifiedDateTime|DateTimeOffset|エンティティが最後に変更された日付と時刻。|



## <a name="response"></a>応答
成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[grouppolicydefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)オブジェクトを返します。

## <a name="example"></a>例

### <a name="request"></a>要求
以下は、要求の例です。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyDefinitions/{groupPolicyDefinitionId}
Content-type: application/json
Content-length: 285

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinition",
  "classType": "machine",
  "displayName": "Display Name value",
  "explainText": "Explain Text value",
  "categoryPath": "Category Path value",
  "supportedOn": "Supported On value",
  "policyType": "admxIngested"
}
```

### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 398

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinition",
  "classType": "machine",
  "displayName": "Display Name value",
  "explainText": "Explain Text value",
  "categoryPath": "Category Path value",
  "supportedOn": "Supported On value",
  "policyType": "admxIngested",
  "id": "f9607947-7947-f960-4779-60f9477960f9",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```






