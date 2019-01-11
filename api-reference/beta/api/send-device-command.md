---
title: デバイス コマンドを送信します。
description: 'この API は、Microsoft アカウントに関連付けられているデバイスのコマンドをプロジェクトのローマの機能を使用します。 GET の呼び出しを実行した後は`me/devices`、デバイスにコマンドを実行するデバイスの ID を渡します。 コマンドの 2 つの種類がサポートされている: LaunchURI と AppServices。 LaunchURI を使用している場合は、*型*と*ペイロード*のパラメーターを指定します。 AppService 呼び出しに指定します '
localization_priority: Normal
ms.openlocfilehash: 54349e2f43a776523614b0cd2abbc209e89305fd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891988"
---
# <a name="send-device-command"></a>デバイス コマンドを送信します。

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

この API は、Microsoft アカウントに関連付けられているデバイスのコマンドをプロジェクトのローマの機能を使用します。 GET の呼び出しを実行した後は`me/devices`、デバイスにコマンドを実行するデバイスの ID を渡します。 コマンドの 2 つの種類がサポートされている: LaunchURI と AppServices。 LaunchURI を使用している場合は、*型*と*ペイロード*のパラメーターを指定します。 AppService 呼び出しには、*型*、*ペイロード*、 *packageFamilyName*、および*appServiceName*パラメーターを指定します。

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

要求の本文には、コマンドのプロパティの JSON 表現を指定します。

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

|**Name**|**型**|**説明**|
|:----|:------|:------|
|payload | microsoft.graph.json| ペイロードのアプリケーション サービスに送信するか、デバイスの URI を起動します。 |
|responsePayload | microsoft.graph.json| ペイロードは、ターゲット ・ デバイスから返されます。 |
|postBackURI | String | 投稿は、更新の後続の通知を送信する URI をバックアップします。 |
|packageFamilyName | String | Windows のアプリケーションのパッケージ ファミリ名。 |
|appServiceName | String | 対象のアプリケーションで定義されているアプリケーション サービスの名前です。 場合は、アプリケーション サービスを起動する必要があります。 |
|type| String | LaunchURI または AppService です。 |
|id| String | デバイスに送信されたコマンドの ID。 |
|actionStatus | String | コマンドの[ステータス](get-device-command-status.md)です。 |
|エラー| String| ターゲット アプリケーションからの要求に関連付けられているエラーです。 |

## <a name="launch-uri-example"></a>URI の使用例を起動します。

LaunchURI 要求の例を次のとおりです。URI またはターゲット ・ デバイス上のアプリケーションが起動されます。 URI またはアプリケーションを起動するには、デバイスの ID を使用して投稿を発行します (GET の呼び出しを行うから取得した`me/devices`)。 *型*パラメーターを*LaunchURI*に設定し、URI 値を指定して次のようにhttps://bing.com。

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


## <a name="app-service-example"></a>アプリケーション サービスの例

ここでは、デバイスで、アプリケーションのサービスのクエリの例です。 アプリケーション サービスを使用するデバイスの id を使用して POST 呼び出しを行う必要があります (GET の呼び出しを行うから取得した`me/devices`)。 次の例を使用するには、ターゲット ・ デバイスに[ローマのアプリケーション](https://aka.ms/romanapp)をインストールしてください。

呼び出しでは、いくつかの追加プロパティを設定する必要があります。 *型*は、 *AppService*に設定する必要があります。、 *AppServiceName*は、アプリケーションで定義されているアプリケーション サービスの名前に設定する必要があります。、 *PackageFamilyName*は、アプリケーション マニフェスト、および*ペイロード*で定義されているパッケージのファミリ名を設定する必要があります。キーと呼び出し先のアプリケーション サービスの値を保持します。

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
