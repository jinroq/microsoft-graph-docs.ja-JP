---
title: ユーザー デバイスを一覧表示する
description: プロジェクトローマ機能をサポートするユーザーデバイスのリストを取得します。 これには、アプリを起動したり、アプリケーションに対してデータを送信したりする機能が含まれます。 [自分/デバイスで呼び出しを実行した後、デバイスにコマンドを送信するには、デバイスの ID] を渡します。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 292124babfb71ad1c86ae373f123c2f5d57df3b4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35996253"
---
# <a name="list-user-devices"></a>ユーザー デバイスを一覧表示する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

プロジェクトローマ機能をサポートするユーザーデバイスのリストを取得します。 これには、アプリを起動したり、アプリケーションに対してデータを送信したりする機能が含まれます。 [自分/デバイスで呼び出しを実行した後、デバイスに[コマンドを送信](send-device-command.md)するには、デバイスの ID] を渡します。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。


|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | サポートされていません。    |
|委任 (個人用 Microsoft アカウント) | Device.Read    |
|アプリケーション | サポートされていません。 |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
GET me/devices
```

## <a name="request-headers"></a>要求ヘッダー

| ヘッダー |値
|:----|:------|
|Authorization| ベアラー {トークン}。必須。 |
|承諾 | application/json |

## <a name="request-body"></a>要求本文
このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答

成功した場合、このメソッドは応答本文で200応答コードとユーザーデバイスプロパティを返します。

<!-- { "blockType": "ignored" } -->

```http
HTTP/1.1 200 OK
```

<!-- { "blockType": "ignored" } -->

```json
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#devices",
  "value": [
    {
      "name": "name",
      "id": "id",
      "status": "status",
      "platform": "platform",
      "kind": "formFactor",
      "model": "model",
      "manufacturer": "manufacturer",
    }
  ]
}
```

## <a name="example"></a>例
この例では、ユーザーのデバイスの一覧を返します。 を使用して`me/devices/{id}/command`デバイスのコマンドを実行するには、返されるデバイスの ID を取得する必要があります。

#### <a name="request"></a>要求

要求の例を次に示します。

<!-- {
  "blockType": "ignored",
  "name": "list_devices"
}-->

```http
GET me/devices
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a>応答

応答の例を次に示します。 注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。 実際の呼び出しではすべてのプロパティが返されます。

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.device",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 140

{
  "value": [
    {
      "Name": "JimSurface",
      "id": "6841b3db-2b55-467b-ad84-79a41a4ef665",
      "Manufacturer": "Microsoft Corporation",
      "Model": "Surface Book",
      "Kind": "Tablet",
      "Status": "Unknown",
      "Platform": "Windows"
    }
  ]
}
```
