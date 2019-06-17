---
title: Update deviceAppManagement
description: deviceAppManagement オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 03290cf87550427878d1b01d2ea4e3da9712fd8c
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34990086"
---
# <a name="update-deviceappmanagement"></a>Update deviceAppManagement

> **重要:** Microsoft Graph の/ベータ版の Api は変更される可能性があります。 実稼働アプリケーションでは、これらの API の使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

[deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) オブジェクトのプロパティを更新します。
## <a name="prerequisites"></a>前提条件
この API を呼び出すには、次のいずれかのアクセス許可が必要です。 アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。  適切なアクセス許可は、ワークフローによって異なることに注意してください。

|アクセス許可の種類|アクセス許可 (特権の大きいものから小さいものへ)|
|:---|:---|
| 委任 (職場または学校のアカウント) | |
| &nbsp;&nbsp; **アプリ**、**ブック**、**オンボード**、または**パートナーの統合** | DeviceManagementApps.ReadWrite.All |
| &nbsp;&nbsp; **デバイスの管理** | DeviceManagementManagedDevices.ReadWrite.All |
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
|Authorization|ベアラー &lt;トークン&gt; が必要です。|
|承諾|application/json|

## <a name="request-body"></a>要求本文
要求本文で、[deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) オブジェクトの JSON 表記を提供します。

次の表に、[deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) 作成時に必要なプロパティを示します。

|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。|
|**オンボード**|
|isEnabledForMicrosoftStoreForBusiness|Boolean|アカウントと、ビジネス向け Microsoft Store からのアプリケーションとの同期が有効にされているかどうか。|
|microsoftStoreForBusinessLanguage|String|ビジネス向け Microsoft Store からのアプリケーションの同期に使用されたロケール情報。 国/地域固有のカルチャ。 カルチャの名前は RFC 4646 に準拠します (Windows Vista 以降)。 形式は <languagecode2>-<country/regioncode2> です。<languagecode2> は ISO 639-1 に基づく小文字 2 文字で構成されるコードで、<country/regioncode2> は ISO 3166 の基づく大文字 2 文字で構成されるコードです。 たとえば、英語 (米国) 固有のカルチャは en-US です。|
|microsoftStoreForBusinessLastCompletedApplicationSyncTime|DateTimeOffset|ビジネス向け Microsoft Store からのアプリケーションの同期が最後に実行された日時。|
|microsoftStoreForBusinessLastSuccessfulSyncDateTime|DateTimeOffset|Microsoft Store for Business のアプリがアカウントに正常に同期された最終日時。|
|microsoftStoreForBusinessPortalSelection|[microsoftStoreForBusinessPortalSelectionOptions](../resources/intune-onboarding-microsoftstoreforbusinessportalselectionoptions.md)|エンドユーザーポータルの情報は、Microsoft Store for Business から Intune ポータルサイトにアプリケーションを同期するために使用されます。 [会社ポータルのみ]、[ \[ポータルサイトとプライベートストア]、[プライベートストアのみ] から選択するには、3\]つのオプションがあります。 可能な値は、`none`、`companyPortal`、`privateStore` です。|

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



