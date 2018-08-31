---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharingLink
ms.openlocfilehash: 7639dab9f63a948b3e9a849d8d320de60f5a0954
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/21/2018
ms.locfileid: "23270490"
---
# <a name="sharinglink-resource-type"></a>SharingLink リソース型

**SharingLink** リソースは、リンク関連のデータ項目を 1 つの構造にグループ化します。

[**Permission**](permission.md) リソースが非 null の **sharingLink** ファセットを持つ場合、アクセス許可は (ユーザーやグループに与えられているアクセス許可ではなく) 共有リンクを表します。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "application", "scope" ],
  "@odata.type": "microsoft.graph.sharingLink"
}-->

```json
{
  "application": { "@odata.type": "microsoft.graph.identity" },
  "type": "view | edit | embed",
  "scope": "anonymous | organization",
  "webHtml": "string",
  "webUrl": "url"
}
```

## <a name="properties"></a>プロパティ

| プロパティ    | タイプ          | 説明
|:------------|:--------------|:-------------------------------------
| アプリケーション | [アイデンティティ][]  | リンクが関連付けられているアプリケーションです。
| 型        | 文字列        | 作成されたリンクの種類。
| スコープ       | 文字列        | このアクセス許可によって表されるリンクの範囲です。値 `anonymous` は、すべてのユーザーがリンクを使用できることを示し、`organization` は同じテナントにサインインしたユーザーのみがリンクを使用できることを示します。
| webHtml     | 文字列        | リンクの場合、このプロパティには、Web ページに項目を埋め込む `<iframe>` 要素の HTML コードが格納されます。`embed`
| webUrl      | 文字列        | OneDrive の web サイト上で、項目をブラウザーに開く URL です。

[ID]: identity.md

## <a name="type-options"></a>タイプ オプション

この表は、**type** プロパティの可能な値を定義します。

| 値   | ロール    | 説明
|:--------|:--------|:---------------------------------------------------------
| `view`  | `read`  | 読み取り専用のアクセスを許可する、閲覧専用の共有リンクです。
| `edit`  | `write` | 読み取り/書き込みのアクセスを許可する、編集共有リンクです。
| `embed` | `read`  | ホスト Web ページにコンテンツを埋め込むために使用できる、表示専用共有リンクです。 埋め込みリンクは、OneDrive for Business または SharePoint では使用できません。

## <a name="scope-options"></a>スコープ オプション

| 値          | 説明
|:---------------|:------------------------------------------------------------
| `anonymous`    | ユーザーはリンクがあればアクセスでき、サインインする必要はありません。 これには、組織外部のユーザーが含まれる場合があります。
| `organization` | 組織 (テナント) に所属しているすべてのユーザーが、リンクを使ってアクセスできます。 OneDrive for Business と SharePoint のみで使用できます。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The sharing link facet provides information about how a file is shared.",
  "keywords": "sharing,sharing link, sharing url, webUrl",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/sharinglink.md:
      Found potential enums in resource example that weren't defined in a table:(view,edit,embed) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/sharinglink.md:
      Found potential enums in resource example that weren't defined in a table:(anonymous,organization) are in resource, but () are in table"
  ],
  "tocPath": "Facets/SharingLink"
} -->
