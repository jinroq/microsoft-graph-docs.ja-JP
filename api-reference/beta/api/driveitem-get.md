---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: ファイルまたはフォルダーを取得する
ms.openlocfilehash: 1ad021e724c807bf15e777b5438c22b5a532a4aa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071115"
---
# <a name="get-a-driveitem-resource"></a>DriveItem リソースを取得する

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

[ドライブ](../resources/drive.md) 内の [DriveItem](../resources/driveitem.md) 用のメタデータを、ファイル システム パスまたは ID で取得します。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All    |
|委任 (個人用 Microsoft アカウント) | Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All    |
|アプリケーション | Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}
GET /drives/{drive-id}/root:/{item-path}
GET /groups/{group-id}/drive/items/{item-id}
GET /groups/{group-id}/drive/root:/{item-path}
GET /me/drive/items/{item-id}
GET /me/drive/root:/{item-path}
GET /sites/{siteId}/drive/items/{itemId}
GET /sites/{siteId}/drive/root:/{item-path}
GET /users/{userId}/drive/items/{itemId}
GET /users/{userId}/drive/root:/{item-path}
```

## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター

このメソッドは、応答をカスタマイズするための `$expand` と `$select` の [OData クエリ パラメーター](/graph/query-parameters)をサポートします。

アイテムが**子**関係にある場合、[`$expand` クエリ文字列パラメーター](/graph/query-parameters) を使って、アイテムのメタデータを取得するのと同じように、同一呼び出し内のアイテムの子を含めることができます。

## <a name="optional-request-headers"></a>オプションの要求ヘッダー

| 名前          | 値  | 説明                                                                                                                                              |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| if-none-match | String | この要求ヘッダーが含まれている場合、指定された eTag (または cTag) がファイルの現在のタグに一致すると、`HTTP 304 Not Modified` 応答が返されます。 |

## <a name="response"></a>応答

成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [DriveItem](../resources/driveitem.md) リソースを返します。

## <a name="example"></a>例

### <a name="request"></a>要求

以下は、ユーザーの OneDrive のルート フォルダーへの要求の例です。

<!-- { "blockType": "request", "name": "get-item-metadata" }-->

```http
GET /me/drive/root
```

## <a name="response"></a>応答

以下は、応答の例です。

<!-- { "blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.driveItem" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "createdBy": {
      "user": {
          "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
          "displayName": "Ryan Gregg"
      }
  },
  "createdDateTime": "2016-03-21T20:01:37Z",
  "cTag": "\"c:{86EB4C8E-D20D-46B9-AD41-23B8868DDA8A},0\"",
  "eTag": "\"{86EB4C8E-D20D-46B9-AD41-23B8868DDA8A},1\"",
  "folder": { "childCount": 120 },
  "id": "01NKDM7HMOJTVYMDOSXFDK2QJDXCDI3WUK",
  "lastModifiedBy": {
      "user": {
          "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
          "displayName": "Ryan Gregg"
      }
  },
  "lastModifiedDateTime": "2016-03-21T20:01:37Z",
  "name": "OneDrive",
  "root": { },
  "size": 157286400,
  "webUrl": "https://contoso-my.sharepoint.com/personal/rgregg_contoso_com/Documents"
}
```

## <a name="remarks"></a>備考

エラーがどのように返されるかについては、「[エラー応答][error-response]」を参照してください。

[error-response]: /graph/errors
[odata-parameters]: /graph/query-parameters
[item-resource]: ../resources/driveitem.md
[special-folder]: ../api/drive-get-specialfolder.md

<!-- {
  "type": "#page.annotation",
  "description": "Retrieve metadata about an item and its children in OneDrive",
  "keywords": "retrieve,item,metadata",
  "section": "documentation",
  "tocPath": "Items/Get item"
} -->