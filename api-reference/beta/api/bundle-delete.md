---
author: JeremyKelley
ms.author: jeremyke
title: バンドルの削除
description: ドライブ項目のバンドルを削除する
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 5bd1fd3f5d9befb538aa797481346a406ff0b53f
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932859"
---
# <a name="delete-bundle"></a>バンドルの削除

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**Id**を使用して、ドライブ項目の[バンドル][]を削除します。この方法を使用してバンドルを削除すると、そのバンドルが完全に削除され、ごみ箱に移動されないことに注意してください。
ただし、バンドルによって参照されていたアイテムは削除されません。
それらは親フォルダーに残ります。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | サポートされていません。                             |
|委任 (個人用 Microsoft アカウント) | Files.ReadWrite、Files.ReadWrite.All   |
|アプリケーション          | サポートされていません。                                           |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
DELETE /drive/items/{bundle-id}
```

## <a name="request-headers"></a>要求ヘッダー

| 名前          | 説明  |
|:------------- |:------------ |
| Authorization | ベアラー \{トークン\}。 必須。 |
| if-match      | eTag. 省略可能。 この要求ヘッダーが含まれていて、指定された eTag (または cTag) がバンドルの現在の`412 Precondition Failed`タグと一致しない場合は、応答が返され、バンドルは削除されません。

## <a name="request-body"></a>要求本文

このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答

成功した場合、この呼び出しはリソースが削除され返すものがなかったことを示す `204 No Content` 応答を返します。

エラーがどのように返されるかに関する詳細については、「[エラー応答][error-response]」のトピックを参照してください。

## <a name="example"></a>例

### <a name="request"></a>要求


# <a name="httptabhttp"></a>[プロトコル](#tab/http)
<!-- { "blockType": "request", "name": "delete-bundle" } -->

```http
DELETE https://graph.microsoft.com/beta/drive/items/{bundle-id}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-bundle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-bundle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目的-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-bundle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-bundle-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>応答

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```


[バンドル]: ../resources/bundle.md
[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Delete a bundle from OneDrive",
  "keywords": "delete,existing bundle,onedrive",
  "section": "documentation",
  "tocPath": "Bundles/Delete"
} -->
