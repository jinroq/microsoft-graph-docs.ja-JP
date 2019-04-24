---
title: remoteAssistancePartner の作成
description: 新しい remoteAssistancePartner オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f387750fcd06bc2520479b511c24b4ac7ce333dd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32585266"
---
# <a name="create-remoteassistancepartner"></a>remoteAssistancePartner の作成

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

新しい [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) オブジェクトを作成します。

## <a name="prerequisites"></a>前提条件
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

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
POST /deviceManagement/remoteAssistancePartners
```

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー|値|
|:---|:---|
|Authorization|ベアラー &lt;トークン&gt; が必要です。|
|承諾|application/json|

## <a name="request-body"></a>要求本文
要求本文で、remoteAssistancePartner オブジェクトの JSON 表記を指定します。

次の表に、remoteAssistancePartner の作成時に必要なプロパティを示します。

|プロパティ|型|説明|
|:---|:---|:---|
|id|String|パートナーの一意識別子。|
|displayName|String|パートナーの表示名。|
|onboardingUrl|String|パートナーのオンボーディング ポータルの URL。このポータルでは、管理者がパートナーのリモート アシスタンス サービスを構成できます。|
|onboardingStatus|[remoteAssistanceOnboardingStatus](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|TBD. 使用可能な値は、`notOnboarded`、`onboarding`、`onboarded` です。|
|lastConnectionDateTime|DateTimeOffset|TEM パートナーによって Intune に最後に送信された要求のタイムスタンプ。|



## <a name="response"></a>応答
成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) オブジェクトを返します。

## <a name="example"></a>例

### <a name="request"></a>要求
以下は、要求の例です。
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/remoteAssistancePartners
Content-type: application/json
Content-length: 266

{
  "@odata.type": "#microsoft.graph.remoteAssistancePartner",
  "displayName": "Display Name value",
  "onboardingUrl": "https://example.com/onboardingUrl/",
  "onboardingStatus": "onboarding",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```

### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 315

{
  "@odata.type": "#microsoft.graph.remoteAssistancePartner",
  "id": "7443c8b9-c8b9-7443-b9c8-4374b9c84374",
  "displayName": "Display Name value",
  "onboardingUrl": "https://example.com/onboardingUrl/",
  "onboardingStatus": "onboarding",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```



