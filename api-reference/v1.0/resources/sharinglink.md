---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharingLink
localization_priority: Normal
ms.openlocfilehash: 02a4c0251a5484edc7ba5e07095f44043c269ae5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863554"
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

| プロパティ    | 型          | 説明
|:------------|:--------------|:-------------------------------------
| application | [identity][]  | リンクが関連付けられているアプリケーションです。
| type        | String        | 作成されたリンクの種類。
| scope       | String        | このアクセス許可によって表されるリンクの範囲です。値 `anonymous` は、すべてのユーザーがリンクを使用できることを示し、`organization` は同じテナントにサインインしたユーザーのみがリンクを使用できることを示します。
| webHtml     | String        | `embed` リンクの場合、このプロパティには、Web ページに項目を埋め込む `<iframe>` 要素の HTML コードが格納されます。
| webUrl      | String        | OneDrive の web サイト上で、項目をブラウザーに開く URL です。

[Identity]: identity.md

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
| `anonymous`    | リンクを持つユーザーは、サインインすることがなく、アクセスを持ちます。 これには、組織の外部ユーザーが含まれます。
| `organization` | アクセス権を取得するのには、組織 (テナント) に署名されたすべてのユーザーのリンクを使用できます。 ビジネスと SharePoint の OneDrive でのみ使用できます。

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
