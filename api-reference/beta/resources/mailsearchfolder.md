---
title: mailsearchfolder リソースの種類
description: mailsearchfolder は、指定した検索条件に一致するすべての電子メールアイテムを含む、ユーザーのメールボックス内の仮想フォルダーです。 mailsearchfolder は mailfolder から継承します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 15f334f2910c962c367242965bd2104c8f3edb79
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342756"
---
# <a name="mailsearchfolder-resource-type"></a>mailsearchfolder リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

mailsearchfolder は、指定した検索条件に一致するすべての電子メールアイテムを含む、ユーザーのメールボックス内の仮想フォルダーです。 mailsearchfolder は[mailfolder](mailfolder.md)から継承します。

## <a name="methods"></a>メソッド

| メソッド | 戻り値の型  | 説明 |
|:---------------|:--------|:----------|
| [検索フォルダーを作成する](../api/mailsearchfolder-post.md) | [mailsearchfolder](mailsearchfolder.md) | このユーザーのメールボックスに検索フォルダーを作成します。 |
| [検索フォルダーを一覧表示する](../api/mailfolder-list-childfolders.md) | [mailFolder](mailfolder.md) コレクション | このユーザーのメールボックス内のすべてのフォルダー (検索フォルダーを含む) を一覧表示します。 |
| [検索フォルダ―を取得する](../api/mailfolder-get.md) | [mailsearchfolder](mailsearchfolder.md) | 指定した検索フォルダーを取得します。 |
| [検索フォルダーを更新する](../api/mailsearchfolder-update.md) | [mailsearchfolder](mailsearchfolder.md) | 指定した検索フォルダーを更新します。 |
| [検索フォルダーを削除する](../api/mailfolder-delete.md) | なし | 指定した検索フォルダーを削除します。 |
| [検索フォルダー内のすべてのメッセージを一覧表示する](../api/mailfolder-list-messages.md) | [message](message.md) コレクション | 指定した検索フォルダー内のすべてのメッセージを一覧表示します。 |

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:---------------|:--------|:----------|
| issupported | Boolean | 検索フォルダーが REST api を使用して編集可能かどうかを示します。 |
| includeNestedFolders | Boolean | メールボックスフォルダー階層をスキャンする方法を示します。 `true`詳細検索を実行`false`する必要がある場合は、その代わりに浅い検索を実行する必要があることを意味します。 |
| sourceFolderIDs | String collection | マイニングするメールボックスフォルダー。 |
| filterquery | String | メッセージをフィルター処理するための OData クエリ。 |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailSearchFolder"
}-->

```json
{
  "isSupported": true,
  "includeNestedFolders": true,
  "sourceFolderIDs": ["string"],
  "filterQuery": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2018-01-23 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mailSearchFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
