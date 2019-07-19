---
title: SecurityBaselineCategoryStateSummary を作成する
description: 新しい securityBaselineCategoryStateSummary オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: edff9cdb1cf0a31fc7273c4c736195bf084a5aa1
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34959615"
---
# <a name="create-securitybaselinecategorystatesummary"></a>SecurityBaselineCategoryStateSummary を作成する

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

新しい[securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)オブジェクトを作成します。

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
POST /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/categoryDeviceStateSummaries
```

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー|値|
|:---|:---|
|Authorization|ベアラー &lt;トークン&gt; が必要です。|
|承諾|application/json|

## <a name="request-body"></a>要求本文
要求本文で、securityBaselineCategoryStateSummary オブジェクトの JSON 表記を指定します。

次の表に、securityBaselineCategoryStateSummary の作成時に必要なプロパティを示します。

|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|エンティティの一意識別子。 [SecurityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)から継承します。|
|secureCount|Int32|[SecurityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)から継承した、セキュリティで保護されたデバイスの数|
|notSecureCount|Int32|[SecurityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)から継承した、セキュリティで保護されていないデバイスの数|
|unknownCount|Int32|[SecurityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)から継承された不明なデバイスの数|
|errorCount|Int32|[SecurityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)から継承されたエラーデバイスの数|
|conflictCount|Int32|[SecurityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)から継承された競合デバイスの数|
|notApplicableCount|Int32|[SecurityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)から継承された、適用されていないデバイスの数|
|displayName|String|カテゴリ名|



## <a name="response"></a>応答
成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)オブジェクトを返します。

## <a name="example"></a>例

### <a name="request"></a>要求
以下は、要求の例です。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/categoryDeviceStateSummaries
Content-type: application/json
Content-length: 261

{
  "@odata.type": "#microsoft.graph.securityBaselineCategoryStateSummary",
  "secureCount": 11,
  "notSecureCount": 14,
  "unknownCount": 12,
  "errorCount": 10,
  "conflictCount": 13,
  "notApplicableCount": 2,
  "displayName": "Display Name value"
}
```

### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 310

{
  "@odata.type": "#microsoft.graph.securityBaselineCategoryStateSummary",
  "id": "7a650997-0997-7a65-9709-657a9709657a",
  "secureCount": 11,
  "notSecureCount": 14,
  "unknownCount": 12,
  "errorCount": 10,
  "conflictCount": 13,
  "notApplicableCount": 2,
  "displayName": "Display Name value"
}
```





