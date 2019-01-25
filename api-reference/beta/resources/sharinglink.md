---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharingLink
localization_priority: Normal
ms.openlocfilehash: c21c891981106faa4b631bb2713913bfa8ed0713
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521454"
---
# <a name="sharinglink-resource-type"></a>SharingLink リソース型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
  "preventsDownload": false,
  "type": "view | edit | embed",
  "scope": "anonymous | organization",
  "webHtml": "string",
  "webUrl": "url"
}
```

## <a name="properties"></a>プロパティ

| プロパティ       | 型          | 説明
|:---------------|:--------------|:-------------------------------------
| application    | [identity][]  | リンクが関連付けられているアプリケーションです。
| type           | String        | 作成されたリンクの種類。
| scope          | String        | このアクセス許可によって表されるリンクの範囲です。値 `anonymous` は、すべてのユーザーがリンクを使用できることを示し、`organization` は同じテナントにサインインしたユーザーのみがリンクを使用できることを示します。
| preventsDownload | ブール値       | True の場合、ユーザーは、web 上のアイテムを表示するのにはのみ、このリンクを使用できますし、項目の内容をダウンロードするのには使用できません。 ビジネスと SharePoint の OneDrive です。
| webHtml        | String        | `embed` リンクの場合、このプロパティには、Web ページに項目を埋め込む `<iframe>` 要素の HTML コードが格納されます。
| webUrl         | 文字列        | OneDrive の web サイト上で、項目をブラウザーに開く URL です。

[Identity]: identity.md

### <a name="type-options"></a>タイプ オプション

次の表は、 **type**プロパティの値を定義します。

| 値    | ロール     | 説明
|:---------|:---------|:---------------------------------------------------------
| `view`   | `read`   | 読み取り専用のアクセスを許可する、閲覧専用の共有リンクです。
| `edit`   | `write`  | 読み取り/書き込みのアクセスを許可する、編集共有リンクです。
| `embed`  | `read`   | ホスト Web ページにコンテンツを埋め込むために使用できる、表示専用共有リンクです。 埋め込みリンクは、OneDrive for Business または SharePoint では使用できません。

### <a name="scope-options"></a>スコープ オプション

次の表は、**スコープ**のプロパティの値を定義します。

| 値            | 説明
|:-----------------|:------------------------------------------------------------
| `anonymous`      | リンクを持つユーザーは、サインインすることがなく、アクセスを持ちます。 これには、組織の外部ユーザーが含まれます。
| `organization`   | アクセス権を取得するのには、組織 (テナント) に署名されたすべてのユーザーのリンクを使用できます。 ビジネスと SharePoint の OneDrive でのみ使用できます。
| `existingAccess` | 他の手段を使用して、アイテムへのアクセス権が既に付与されたユーザーだけは、このリンクを使用してアイテムにアクセスできます。 ビジネスと SharePoint の OneDrive でのみ使用できます。
| `users`          | リンクでは、特定のユーザーの一覧にのみアクセスが許可されます。 ビジネスと SharePoint の OneDrive でのみ使用できます。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "The sharing link facet provides information about how a file is shared.",
  "keywords": "sharing,sharing link, sharing url, webUrl",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/sharinglink.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
