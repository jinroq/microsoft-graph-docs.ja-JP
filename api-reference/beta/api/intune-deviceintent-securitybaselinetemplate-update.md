---
title: securityBaselineTemplate の更新
description: securityBaselineTemplate オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9f2cb66df449dc8586ef3fb3f822fadf62891902
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32466169"
---
# <a name="update-securitybaselinetemplate"></a>securityBaselineTemplate の更新

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)オブジェクトのプロパティを更新します。

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
PATCH /deviceManagement/templates/{deviceManagementTemplateId}
```

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー|値|
|:---|:---|
|Authorization|ベアラー &lt;トークン&gt; が必要です。|
|承諾|application/json|

## <a name="request-body"></a>要求本文
要求本文で、 [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)オブジェクトの JSON 表記を指定します。

次の表に、 [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)の作成時に必要なプロパティを示します。

|プロパティ|型|説明|
|:---|:---|:---|
|id|String|[devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)から継承されたテンプレート ID|
|displayName|String|[devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)から継承されたテンプレートの表示名|
|説明|String|[devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)から継承されるテンプレートの説明|



## <a name="response"></a>応答
成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)オブジェクトを返します。

## <a name="example"></a>例

### <a name="request"></a>要求
以下は、要求の例です。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}
Content-type: application/json
Content-length: 145

{
  "@odata.type": "#microsoft.graph.securityBaselineTemplate",
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 194

{
  "@odata.type": "#microsoft.graph.securityBaselineTemplate",
  "id": "3f61d4c2-d4c2-3f61-c2d4-613fc2d4613f",
  "displayName": "Display Name value",
  "description": "Description value"
}
```





