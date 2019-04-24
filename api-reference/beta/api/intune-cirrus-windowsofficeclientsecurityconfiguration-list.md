---
title: リスト windowsOfficeClientSecurityConfigurations
description: windowsOfficeClientSecurityConfiguration オブジェクトのプロパティとリレーションシップをリストします。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e97b364e7a30a85bd5b9109dd41806b7ed8589a4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32482782"
---
# <a name="list-windowsofficeclientsecurityconfigurations"></a>リスト windowsOfficeClientSecurityConfigurations

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

[windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)オブジェクトのプロパティとリレーションシップをリストします。

## <a name="prerequisites"></a>前提条件
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類|アクセス許可 (特権の大きいものから小さいものへ)|
|:---|:---|
|委任 (職場または学校のアカウント)|devicemanagementconfiguration をすべて取得します。|
|委任 (個人用 Microsoft アカウント)|サポートされていません。|
|アプリケーション|サポートされていません。|

## <a name="http-request"></a>HTTP 要求
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations
```

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー|値|
|:---|:---|
|Authorization|ベアラー &lt;トークン&gt; が必要です。|
|承諾|application/json|

## <a name="request-body"></a>要求本文
このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答
成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)オブジェクトのコレクションを返します。

## <a name="example"></a>例

### <a name="request"></a>要求
以下は、要求の例です。
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations
```

### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1222

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsOfficeClientSecurityConfiguration",
      "id": "f90ca1a5-a1a5-f90c-a5a1-0cf9a5a10cf9",
      "userPreferencePayload": "<Unknown Primitive Type Edm.Stream>",
      "policyPayload": "<Unknown Primitive Type Edm.Stream>",
      "description": "Description value",
      "displayName": "Display Name value",
      "priority": 8,
      "userCheckinSummary": {
        "@odata.type": "microsoft.graph.officeUserCheckinSummary",
        "succeededUserCount": 2,
        "failedUserCount": 15
      },
      "checkinStatuses": [
        {
          "@odata.type": "microsoft.graph.officeClientCheckinStatus",
          "userPrincipalName": "User Principal Name value",
          "deviceName": "Device Name value",
          "devicePlatform": "Device Platform value",
          "devicePlatformVersion": "Device Platform Version value",
          "wasSuccessful": true,
          "userId": "User Id value",
          "checkinDateTime": "2016-12-31T23:56:33.9571764-08:00",
          "errorMessage": "Error Message value",
          "appliedPolicies": [
            "Applied Policies value"
          ]
        }
      ]
    }
  ]
}
```



