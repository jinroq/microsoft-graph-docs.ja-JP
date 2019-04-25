---
title: セクションを一覧表示する
description: 指定されたセクショングループから section オブジェクトのリストを取得します。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: c99c0a2e409dfe290712cf5944760846a43c3395
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32537595"
---
# <a name="list-sections"></a>セクションを一覧表示する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指定されたセクショングループから[section](../resources/section.md)オブジェクトのリストを取得します。
## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | メモ作成、メモ読み取り、メモ (すべて)、メモ書き込み、メモ (すべて)    |
|委任 (個人用 Microsoft アカウント) | Notes.Create、Notes.Read、Notes.ReadWrite    |
|アプリケーション | Notes.Read.All、Notes.ReadWrite.All |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sectionGroups/{id}/sections
GET /users/{id | userPrincipalName}/onenote/sectionGroups/{id}/sections
GET /groups/{id}/onenote/sectionGroups/{id}/sections
GET /sites/{id}/onenote/sectionGroups/{id}/sections
```
## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター
このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。

既定の並べ替え順序は `name asc`です。

既定のクエリは`parentNotebook` 、、 `id` `displayName`、および`self`プロパティを展開して選択します。 セクション`expand`の有効な値`parentNotebook`は`parentSectionGroup`、とです。


## <a name="request-headers"></a>要求ヘッダー
| 名前       | 型 | 説明|
|:-----------|:------|:----------|
| Authorization  | string  | ベアラー {トークン}。必須。 |
| 承諾 | string | `application/json` |

## <a name="request-body"></a>要求本文
このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答

成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[section](../resources/section.md)オブジェクトのコレクションを返します。
## <a name="example"></a>例
##### <a name="request"></a>要求
以下は、要求の例です。
<!-- {
  "blockType": "request",
  "name": "get_sections"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/sectionGroups/{id}/sections
```
##### <a name="response"></a>応答
以下は、応答の例です。注:ここに示す応答オブジェクトは切り詰めて簡略化されています。実際の呼び出しではすべてのプロパティが返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteSection",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 345

{
  "value": [
    {
      "isDefault": true,
      "pagesUrl": "pagesUrl-value",
      "displayName": "name-value",      
      "createdBy": {
        "user": {
          "id": "id-value",
          "displayName": "displayName-value"
        }
      },
      "lastModifiedBy": {
        "user": {
          "id": "id-value",
          "displayName": "displayName-value"
        }
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List sections",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/sectiongroup-list-sections.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
