---
author: JeremyKelley
description: SharingLink リソースは、リンク関連のデータ項目を単一の構造にグループ化します。
ms.date: 09/10/2017
title: SharingLink
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: f1ebff332227410bcb67d87de50a97dd2e078660
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965132"
---
# <a name="sharinglink-resource-type"></a>sharingLink リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**Sharinglink**リソースは、リンク関連のデータ項目を単一の構造にグループ化します。

[**アクセス許可**](permission.md)リソースに非 Null の**sharinglink**ファセットがある場合、アクセス許可は (ユーザーまたはグループに付与されたアクセス許可ではなく) 共有リンクを表します。

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
| preventsDownload | Boolean       | True の場合、ユーザーはこのリンクを使用して web 上のアイテムを表示することができ、アイテムのコンテンツをダウンロードするために使用することはできません。 OneDrive for business と SharePoint の場合のみ。
| webHtml        | String        | `embed` リンクの場合、このプロパティには、Web ページに項目を埋め込む `<iframe>` 要素の HTML コードが格納されます。
| webUrl         | 文字列        | OneDrive の web サイト上で、項目をブラウザーに開く URL です。

[Identity]: identity.md

### <a name="type-options"></a>種類のオプション

次の表は、 **type**プロパティに指定できる値を定義します。

| 値    | ロール     | 説明
|:---------|:---------|:---------------------------------------------------------
| `view`   | `read`   | 読み取り専用のアクセスを許可する、閲覧専用の共有リンクです。
| `edit`   | `write`  | 読み取り/書き込みのアクセスを許可する、編集共有リンクです。
| `embed`  | `read`   | ホスト Web ページにコンテンツを埋め込むために使用できる、表示専用共有リンクです。 埋め込みリンクは、OneDrive for Business または SharePoint では使用できません。

### <a name="scope-options"></a>範囲オプション

次の表では、 **scope**プロパティに指定できる値を定義します。

| 値            | 説明
|:-----------------|:------------------------------------------------------------
| `anonymous`      | リンクを持つすべてのユーザーが、サインインを必要とせずにアクセスできます。 これには、組織外のユーザーが含まれることがあります。
| `organization`   | 組織 (テナント) にサインインしているユーザーは、リンクを使用してアクセス権を取得することができます。 OneDrive for business と SharePoint でのみ使用できます。
| `existingAccess` | 他の手段でアイテムへのアクセスが既に許可されているユーザーのみが、このリンクを使用してアイテムにアクセスできます。 OneDrive for business と SharePoint でのみ使用できます。
| `users`          | このリンクは、ユーザーの特定のリストにのみアクセスを許可します。 OneDrive for business と SharePoint でのみ使用できます。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "The sharing link facet provides information about how a file is shared.",
  "keywords": "sharing,sharing link, sharing url, webUrl",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
