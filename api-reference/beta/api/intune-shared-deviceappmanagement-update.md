---
title: Update deviceAppManagement
description: deviceAppManagement オブジェクトのプロパティを更新します。
ms.openlocfilehash: e842e81f098a42e064be1aa00616a84d7f08eb34
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071668"
---
# <a name="update-deviceappmanagement"></a>Update deviceAppManagement

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

[deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) オブジェクトのプロパティを更新します。
## <a name="prerequisites"></a>前提条件
この API を呼び出すには次のアクセス許可のいずれかが必要です。 アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。  ワークフローに従って、適切なアクセス許可が異なることに注意してください。

|アクセス許可の種類|アクセス許可 (特権の大きいものから小さいものへ)|
|:---|:---|
| 委任 (職場または学校のアカウント) | |
| &nbsp;&nbsp; **アプリケーション**、**ブック**、または**契約時** | DeviceManagementApps.ReadWrite.All |
| &nbsp; &nbsp; **デバイスの管理** | DeviceManagementManagedDevices.ReadWrite.All |
| 委任 (個人用 Microsoft アカウント) | サポートされていません。 |
| アプリケーション | サポートされていません。 |

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
|Authorization|ベアラー &lt;トークン&gt; が必須。|
|Accept|application/json|

## <a name="request-body"></a>要求本文
要求本文で、[deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) オブジェクトの JSON 表記を提供します。

次の表に、[deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) 作成時に必要なプロパティを示します。

|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。|
|**採用**|
|isEnabledForMicrosoftStoreForBusiness|Boolean|アカウントと、ビジネス向け Microsoft Store からのアプリケーションとの同期が有効にされているかどうか。|
|microsoftStoreForBusinessLanguage|String|ビジネス向け Microsoft Store からのアプリケーションの同期に使用されたロケール情報。 国/地域固有のカルチャ。 カルチャの名前は RFC 4646 に準拠します (Windows Vista 以降)。 形式の <languagecode2>-<country/regioncode2> は<languagecode2>  ISO 639-1 に基づく小文字 2 文字のコードで、<country/regioncode2> は ISO 3166 に基づく大文字 2 文字のコードです。 たとえば、英語 (米国) 固有のカルチャは en-US です。|
|microsoftStoreForBusinessLastCompletedApplicationSyncTime|DateTimeOffset|ビジネス向け Microsoft Store からのアプリケーション同期が最後に実行された日時。|
|microsoftStoreForBusinessLastSuccessfulSyncDateTime|DateTimeOffset|ビジネス向け Microsoft Store のアプリがアカウントに正常に同期された最終日時。|
|microsoftStoreForBusinessPortalSelection|[microsoftStoreForBusinessPortalSelectionOptions](../resources/intune-onboarding-microsoftstoreforbusinessportalselectionoptions.md)|エンド ・ ユーザーのポータルの情報は、Intune 企業ポータルにビジネス向けのマイクロソフト ストアからアプリケーションを同期する使用されます。 3 つのオプションから選択するのには\['会社のポータルのみ'、' 企業ポータルおよびプライベート ストアの'、'プライベート ストアのみ'\]。 可能な値は、`none`、`companyPortal`、`privateStore` です。|

このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。

## <a name="response"></a>応答
成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) オブジェクトを返します。

## <a name="example"></a>例

### <a name="request"></a>要求

以下は、要求の例です。

``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a>応答

以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 110

{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
}
```



