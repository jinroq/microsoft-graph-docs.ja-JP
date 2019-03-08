---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SharingLink
localization_priority: Normal
ms.openlocfilehash: f16f8240800be4b9c1780a4057583381b736f079
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481427"
---
# <a name="sharinglink-resource-type"></a>SharingLink リソースの種類

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

| プロパティ    | 種類          | 説明
|:------------|:--------------|:-------------------------------------
| application | [identity][]  | リンクが関連付けられているアプリケーションです。
| type        | String        | 作成されたリンクの種類。
| scope       | String
        | このアクセス許可によって表されるリンクの範囲です。値 `anonymous` は、すべてのユーザーがリンクを使用できることを示し、`organization` は同じテナントにサインインしたユーザーのみがリンクを使用できることを示します。
| webHtml     | String        | `embed` リンクの場合、このプロパティには、Web ページに項目を埋め込む `<iframe>` 要素の HTML コードが格納されます。
| webUrl      | 文字列        | OneDrive の web サイト上で、項目をブラウザーに開く URL です。

[Identity]: identity.md

## <a name="type-options"></a>種類のオプション

この表は、**type** プロパティの可能な値を定義します。

| 値   | ロール    | 説明
|:--------|:--------|:---------------------------------------------------------
| `view`  | `read`  | 読み取り専用のアクセスを許可する、閲覧専用の共有リンクです。
| `edit`  | `write` | 読み取り/書き込みのアクセスを許可する、編集共有リンクです。
| `embed` | `read`  | ホスト Web ページにコンテンツを埋め込むために使用できる、表示専用共有リンクです。 埋め込みリンクは、OneDrive for Business または SharePoint では使用できません。

## <a name="scope-options"></a>範囲オプション

| 値          | 説明
|:---------------|:------------------------------------------------------------
| `anonymous`    | リンクを持つすべてのユーザーが、サインインを必要とせずにアクセスできます。 これには、組織外のユーザーが含まれることがあります。
| `organization` | 組織 (テナント) にサインインしているユーザーは、リンクを使用してアクセス権を取得することができます。 OneDrive for business と SharePoint でのみ使用できます。

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
