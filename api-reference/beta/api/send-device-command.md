---
title: デバイス コマンドを送信する
description: 'この API を使用すると、Project ローマ機能を使用して、Microsoft アカウントに関連付けられているデバイスにコマンドを実行できます。 GET 呼び出しを実行した`me/devices`後、デバイスにコマンドを発行するデバイスの ID を渡します。 launchuri と appservices という2種類のコマンドがサポートされています。 launchuri を使用している場合は、 *type*パラメーターと*payload*パラメーターを指定します。 AppService の呼び出しの場合は、 '
localization_priority: Normal
ms.openlocfilehash: d0c25200933a4a87a66349e457c500c496272b08
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32537530"
---
# <a name="send-device-command"></a>デバイス コマンドを送信する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

この API を使用すると、Project ローマ機能を使用して、Microsoft アカウントに関連付けられているデバイスにコマンドを実行できます。 GET 呼び出しを実行した`me/devices`後、デバイスにコマンドを発行するデバイスの ID を渡します。 launchuri と appservices という2種類のコマンドがサポートされています。 launchuri を使用している場合は、 *type*パラメーターと*payload*パラメーターを指定します。 AppService の呼び出しの場合は、 *type*、 *payload*、 *efamilyname*、 *appservicename*の各パラメーターを指定します。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。


|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | サポートされていません。    |
|委任 (個人用 Microsoft アカウント) | Device.Command    |
|アプリケーション | サポートされていません。 |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
POST me/devices/{id}/commands
```

## <a name="request-headers"></a>要求ヘッダー


| ヘッダー |値
|:----|:------|
|Authorization| ベアラー {トークン}。必須。 |
|承諾 | application/json |

## <a name="request-body"></a>要求本文

要求本文で、コマンドプロパティの JSON 表記を指定します。

```json
{
  "type": "appService",
  "payload": "payload-JSON",
  "packageFamilyName": "packageFamilyName",
  "appServiceName": "appServiceName",
  "postbackURI": "postbackURI"
}
```

## <a name="response"></a>応答

```http
HTTP/1.1 201 OK
```

```json
{
  "id": "0",
  "status": "requesting",
  "type": "appService",
  "appServiceName": "appServiceName",
  "packageFamilyName": "packageFamilyName",
  "error": "null",
  "responsePayload": "null",
  "payload": "payload-JSON",
  "permissionTicket": "null",
  "postBackUri": "postbackURI"
}
```
## <a name="command-properties"></a>コマンドのプロパティ 

|**名前**|**Type**|**説明**|
|:----|:------|:------|
|payload | microsoft graph| アプリサービスに送信するペイロード、またはデバイスで URI を起動するためのペイロード。 |
|responsepayload | microsoft graph| ターゲットデバイスから返されたペイロード。 |
|postBackURI | String | 今後の更新通知を送信するための URI をポストバックします。 |
|パッケージ efamilyname | String | Windows パッケージファミリアプリケーションの名前。 |
|appservicename | String | ターゲットアプリケーションによって定義された app service の名前です。 app service を開始する場合に必要です。 |
|type| String | launchuri または AppService。 |
|id| String | デバイスに送信されたコマンドの ID。 |
|actionstatus | String | コマンドの[状態](get-device-command-status.md)を示します。 |
|error| String| ターゲットアプリケーションからの要求に関連付けられているエラー。 |

## <a name="launch-uri-example"></a>開始 URI の例

ここでは、launchuri 要求の例を示します。ターゲットデバイス上の URI またはアプリケーションを起動します。 URI またはアプリを起動するには、デバイスの ID を使用して POST を発行します (GET 呼び出し`me/devices`の実行によって取得されます)。 *型*パラメーターを*launchuri*に設定し、などの URI 値をhttps://bing.com指定します。

#### <a name="request"></a>要求

要求の例を次に示します。

<!-- {
  "blockType": "ignored",
  "name": "post_command"
} -->

```http

POST me/devices/{id}/commands
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8

{ "type" : "LaunchUri", "payload" : {"uri":"https://bing.com"}}

```

#### <a name="response"></a>応答 

応答の例を次に示します。

<!-- {
  "blockType": "ignored",
  "truncated": false,
  "@odata.type": "microsoft.graph.commandobject",
  "isCollection": true
} -->

```http
HTTP/1.1 201 OK

{
  "id": "0158355AD4D680CC4E2994CC009EFFD7337D1B...",
  "status": "requesting",
  "type": null,
  "appServiceName": null,
  "packageFamilyName": null,
  "error": null,
  "permissionTicket": null,
  "postBackUri": null,
  "payload": {
    "uri": "https://bing.com"
  }
}

```


## <a name="app-service-example"></a>App service の例

ここでは、デバイス上の app service に対してクエリを実行する例を示します。 アプリサービスを使用するには、デバイスの id を使用して POST 呼び出しを行う必要があります (GET `me/devices`呼び出しの実行によって取得)。 次の例を使用するには、ターゲットデバイスに[ローマアプリ](https://aka.ms/romanapp)をインストールする必要があります。

呼び出しでは、いくつかの追加プロパティを設定する必要があります。 *Type*を*AppService*に設定する必要があります。 *appservicename*は、アプリケーションで定義されている app service ** の名前に設定する必要があります。また、アプリマニフェストで定義されているパッケージファミリー名と*ペイロード*に設定する必要があります。ターゲットアプリケーション内で呼び出すサービスのキーと値を保持します。

#### <a name="request"></a>要求

<!-- {
  "blockType": "ignored",
  "name": "post_command_2"
} -->

```http

POST me/devices/{id}/commands
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8

{
  "type" : "AppService",
  "appServiceName" : "com.microsoft.test.cdppingpongservice",
  "packageFamilyName" : "5085ShawnHenry.RomanTestApp_jsjw7knzsgcce",
  "payload" : {
    "Type":"Toast","Title":"Hello","Subtitle":"World!"}
  }
```

#### <a name="response"></a>応答

応答の例を次に示します。

<!-- {
  "blockType": "ignored",
  "truncated": false,
  "@odata.type": "microsoft.graph.commandobject",
  "isCollection": true
} -->

```http
HTTP/1.1 201 OK

{
  "id": "0158355AD4D680CC4E2994CC009EFFD7EADA8307E96FF1C8D19B..",
  "status": "requesting",
  "type": null,
  "appServiceName": "com.microsoft.randomnumbergenerator",
  "packageFamilyName": "Microsoft.SDKSamples.AppServicesProvider.CS_8wekyb3d8bbwe",
  "error": null,
  "permissionTicket": null,
  "postBackUri": null,
  "payload": {
    "Type": "Toast",
    "Title": "Hello",
    "Subtitle": "World!"
  }
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/send-device-command.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
