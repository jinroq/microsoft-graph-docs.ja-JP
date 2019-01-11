---
title: 写真を取得する
description: 指定した profilePhoto またはそのメタデータ (**profilePhoto**プロパティ) を取得します。
localization_priority: Priority
ms.openlocfilehash: be20e243a89d258c8db2105efe0c53cbea0abebf
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851738"
---
# <a name="get-photo"></a>写真を取得する

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

指定した[profilePhoto](../resources/profilephoto.md)またはそのメタデータ (**profilePhoto**プロパティ) を取得します。

GET 写真操作最初の試みから Office 365 に指定された写真を取得します。 写真が Office 365 で利用できない場合は、API は、Azure Active Directory から写真を取得しようとします。

Office 365 上でサポートされている HD Photo のサイズは次のとおりです: '48x48'、'64x64'、'96x96'、'120x120'、'240x240'、'360x360'、'432x432'、'504x504'、'648x648'。 写真が Azure Active Directory に格納されている場合は、サイズに関する制限はありません。

使用可能な最大の写真のメタデータを取得したり、サイズを指定してその写真サイズのメタデータを取得したりできます。
要求したサイズが使用できない場合でも、アップロードされて使用可能になっている、より小さいサイズを取得できます。
たとえば、アップロードした写真が 504x504 ピクセルの場合は、648×648 を除くすべてのサイズの写真がダウンロード可能になります。
指定したサイズがユーザーのメールボックスにも Azure Active Directory にもない場合は、'1x1' のサイズがメタデータの残りの部分とともに返されます。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

> **注:** ベータ版の写真の取得操作は、ユーザーの作業時間、学校、または個人のアカウントをサポートします。 ただし、写真のメタデータの取得操作には、ユーザーの作業や学校のアカウントとアカウントのない個人のみがサポートされています。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | **user** リソースの場合:<br/>User.Read、User.ReadBasic.All、User.Read.All、User.ReadWrite、User.ReadWrite.All<br /><br />**group** リソースの場合:<br />Group.Read.All、Group.ReadWrite.All<br /><br />**contact** リソースの場合:<br />Contacts.Read、Contacts.ReadWrite |
|委任 (個人用 Microsoft アカウント)  <br /> **注**: メタデータの操作はサポートされていません。 | **user** リソースの場合:<br/>User.Read、User.ReadWrite<br /><br />**contact** リソースの場合:<br />Contacts.Read、Contacts.ReadWrite |
|アプリケーション                        | **user** リソースの場合:<br/>User.Read.All、User.ReadWrite.All<br /><br />**group** リソースの場合:<br />Group.Read.All、Group.ReadWrite.All<br /><br />**contact** リソースの場合:<br />Contacts.Read、Contacts.ReadWrite |

## <a name="http-request"></a>HTTP 要求 

### <a name="get-the-photo"></a>写真を取得します。
<!-- { "blockType": "ignored" } -->
```http
GET /me/photo/$value
GET /users/{id | userPrincipalName}/photo/$value
GET /groups/{id}/photo/$value
GET /me/contacts/{id}/photo/$value
GET /users/{id | userPrincipalName}/contacts/{id}/photo/$value
GET /me/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
GET /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo/$value
```
### <a name="get-the-metadata-of-the-photo"></a>写真のメタデータを取得します。
<!-- { "blockType": "ignored" } -->
```http
GET /me/photo
GET /users/{id | userPrincipalName}/photo
GET /groups/{id}/photo
GET /me/contacts/{id}/photo
GET /users/{id | userPrincipalName}/contacts/{id}/photo
GET /me/contactfolders/{contactFolderId}/contacts/{id}/photo
GET /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo
```

### <a name="get-the-metadata-for-a-specific-photo-size"></a>特定の写真サイズのメタデータを取得する
<!-- { "blockType": "ignored" } -->
```http
GET /me/photos/{size}
GET /users/{id | userPrincipalName}/photos/{size}
GET /groups/{id}/photos/{size}
GET /me/contacts/{id}/photos/{size}
GET /users/{id | userPrincipalName}/contacts/{id}/photos/{size}
GET /me/contactfolders/{contactFolderId}/contacts/{id}/photos/{size}
GET /users/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photos/{size}
```

## <a name="path-parameters"></a>パス パラメーター

|**パラメーター**|**型**|**説明**|
|:-----|:-----|:-----|
|size  |String  | 写真のサイズ。 Office 365 上でサポートされている HD Photo のサイズは次のとおりです: '48x48'、'64x64'、'96x96'、'120x120'、'240x240'、'360x360'、'432x432'、'504x504'、'648x648'。 写真が Azure Active Directory に格納されている場合は、サイズに関する制限はありません。 |

## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター
このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。

## <a name="request-headers"></a>要求ヘッダー
| 名前       | 種類 | 説明|
|:-----------|:------|:----------|
| Authorization  | string  | ベアラー {トークン}。必須。 |

## <a name="request-body"></a>要求本文
このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答
### <a name="response-for-getting-the-photo"></a>写真の取得に対する応答
成功した場合、このメソッドは `200 OK` 応答コードと、要求した写真のバイナリ データを応答本文で返します。写真が存在しない場合、この操作により `404 Not Found` が返されます。
### <a name="response-for-getting-the-metadata-of-the-photo"></a>写真のメタデータの取得に対する応答
成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [profilePhoto](../resources/profilephoto.md) オブジェクトを返します。

## <a name="example"></a>例
##### <a name="request-1"></a>要求 1
この要求では、サインインしているユーザーの写真を利用可能な最大のサイズで取得します。

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/beta/me/photo/$value
Content-Type: image/jpg
```

##### <a name="response-1"></a>応答 1
要求した写真のバイナリ データが含まれています。HTTP 応答コードは 200 です。

##### <a name="request-2"></a>要求 2
この要求は、サインインしているユーザーの 48x48 の写真を取得します。

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/beta/me/photos/48x48/$value
Content-Type: image/jpg
```

##### <a name="response-2"></a>応答 2
要求した 48x48 の写真のバイナリ データが含まれています。HTTP 応答コードは 200 です。

##### <a name="request-3"></a>要求 3
この要求は、サインインしているユーザーのユーザー写真のメタデータを取得します。

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/beta/me/photo
```

##### <a name="response-3"></a>応答 3
次の応答データは、写真のメタデータを示しています。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。

<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/photo/$entity",
    "@odata.id": "https://graph.microsoft.com/beta/users('ddfcd489-628b-7d04-b48b-20075df800e5@1717622f-1d94-c0d4-9d74-f907ad6677b4')/photo",
    "@odata.mediaContentType": "image/jpeg",
    "@odata.mediaEtag": "\"BA09D118\"",
    "id": "240X240",
    "width": 240,
    "height": 240
}
```

次の応答データは、そのユーザーの写真がまだアップロードされていないときの応答の内容を示しています。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。

<!-- {
  "blockType": "ignored"
}-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/photo/$entity",
    "@odata.id": "https://graph.microsoft.com/beta/users('ddfcd489-628b-7d04-b48b-20075df800e5@1717622f-1d94-c0d4-9d74-f907ad6677b4')/photo",
    "@odata.mediaContentType": "image/gif",
    "@odata.mediaEtag": "",
    "id": "1X1",
    "width": 1,
    "height": 1
}
```
## <a name="using-the-binary-data-of-the-requested-photo"></a>要求した写真のバイナリ データを使用する

`/photo/$value` エンドポイントを使用してプロフィール写真のバイナリ データを取得するときに、そのデータを電子メールの添付ファイルとして追加するには、ベース 64 の文字列に変換する必要があります。 JavaScript で [Outlook メッセージ](user-post-messages.md)の `Attachments` パラメーターの値として渡すことができる配列を作成する方法の例を次に示します。

      const attachments = [{
        '@odata.type': '#microsoft.graph.fileAttachment',
        ContentBytes: file.toString('base64'),
        Name: 'mypic.jpg'
      }];

この例の実装については、「[Node.js 用の Microsoft Graph Connect サンプル](https://github.com/microsoftgraph/nodejs-connect-rest-sample)」を参照してください。

Web ページにイメージを表示する場合は、イメージからメモリ内オブジェクトを作成し、そのオブジェクトをイメージ要素のソースにします。 この操作の JavaScript の例を次に示します。

    const url = window.URL || window.webkitURL;
    const blobUrl = url.createObjectURL(image.data);
    document.getElementById(imageElement).setAttribute("src", blobUrl);

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
