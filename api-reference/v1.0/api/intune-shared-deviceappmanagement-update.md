---
title: Update deviceAppManagement
description: deviceAppManagement オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f97316e06cec39cd0aeb1b22d6142925d81b77ae
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32577071"
---
# <a name="update-deviceappmanagement"></a>Update deviceAppManagement

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

[deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) オブジェクトのプロパティを更新します。

## <a name="prerequisites"></a>前提条件
この API を呼び出すには、次のいずれかのアクセス許可が必要です。 アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。  適切なアクセス許可は、ワークフローによって異なることに注意してください。

|アクセス許可の種類|アクセス許可 (特権の大きいものから小さいものへ)|
|:---|:---|
|委任 (職場または学校のアカウント)|DeviceManagementApps.ReadWrite.All|
|委任 (個人用 Microsoft アカウント)|サポートされていません。|
|アプリケーション|サポートされていません。|

## <a name="http-request"></a>HTTP 要求
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement
```

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー|値|
|:---|:---|
|Authorization|ベアラー &lt;トークン&gt; が必要です。|
|承諾|application/json|

## <a name="request-body"></a>要求本文
要求本文で、[deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) オブジェクトの JSON 表記を提供します。

次の表に、[deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) 作成時に必要なプロパティを示します。

|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。|
|**オンボーディング**|
|isEnabledForMicrosoftStoreForBusiness|Boolean|アカウントと、ビジネス向け Microsoft Store からのアプリケーションとの同期が有効にされているかどうか。|
|microsoftStoreForBusinessLanguage|String|ビジネス向け Microsoft Store からのアプリケーションの同期に使用されたロケール情報。 国/地域固有のカルチャ。 カルチャの名前は RFC 4646 に準拠します (Windows Vista 以降)。 形式は <languagecode2>-<country/regioncode2> です。<languagecode2> は ISO 639-1 に基づく小文字 2 文字で構成されるコードで、<country/regioncode2> は ISO 3166 の基づく大文字 2 文字で構成されるコードです。 たとえば、英語 (米国) 固有のカルチャは en-US です。|
|microsoftStoreForBusinessLastCompletedApplicationSyncTime|DateTimeOffset|ビジネス向け Microsoft Store からのアプリケーションの同期が最後に実行された日時。|
|microsoftStoreForBusinessLastSuccessfulSyncDateTime|DateTimeOffset|Microsoft Store for Business のアプリがアカウントに正常に同期された最終日時。|

## <a name="response"></a>応答
成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) オブジェクトを返します。

## <a name="example-request"></a>要求の例

``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement
Content-type: application/json
Content-length: 2

{}
```

## <a name="example-response"></a>応答の例

簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。 すべてのプロパティは実際の呼び出しから返されます。

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 110

{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
}
```



