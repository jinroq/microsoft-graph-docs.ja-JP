---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharingLink
ms.openlocfilehash: 7b7729899d134fa1d5de7debb1f209ec5aadd70d
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/28/2017
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

| プロパティ    | 型          | 説明
|:------------|:--------------|:-------------------------------------
| application | [identity][]  | リンクが関連付けられているアプリケーションです。
| type        | String        | 作成されたリンクの種類。
| scope       | String        | このアクセス許可によって表されるリンクの範囲です。値 `anonymous` は、すべてのユーザーがリンクを使用できることを示し、`organization` は同じテナントにサインインしたユーザーのみがリンクを使用できることを示します。
| webHtml     | String        | `embed` リンクの場合、このプロパティには、Web ページに項目を埋め込む `<iframe>` 要素の HTML コードが含まれています。
| webUrl      | String        | 項目をブラウザーで OneDrive の Web サイト上で開くための URL です。

[Identity]: identity.md

## <a name="type-enumeration"></a>Type 列挙型

この表は、**type** プロパティの可能な値を定義します。

| 値   | ロール    | 説明
|:--------|:--------|:---------------------------------------------------------
| `view`  | `read`  | 読み取り専用のアクセスを許可する、閲覧専用の共有リンクです。
| `edit`  | `write` | 読み取り/書き込みのアクセスを許可する、編集共有リンクです。
| `embed` | `read`  | ホスト Web ページにコンテンツを埋め込むために使用できる、表示専用共有リンクです。 埋め込みリンクは、OneDrive for Business または SharePoint では使用できません。

## <a name="scope-enumeration"></a>スコープ列挙

| 値          | 説明                                                                                                                 |
|:---------------|:----------------------------------------------------------------------------------------------------------------------------|
| `anonymous`    | 共有リンクは誰でも使用可能です。                                                                            |
| `organization` | 共有リンクは、同じ組織 (テナント) 内のすべてのユーザーが使用可能です。OneDrive Personal では使用できません。 |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The sharing link facet provides information about how a file is shared.",
  "keywords": "sharing,sharing link, sharing url, webUrl",
  "section": "documentation",
  "tocPath": "Facets/SharingLink"
} -->
