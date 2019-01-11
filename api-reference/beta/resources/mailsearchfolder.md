---
title: mailSearchFolder リソースの種類
description: MailSearchFolder は、指定した検索条件に一致するすべてのメール アイテムが含まれているユーザーのメールボックス内の仮想フォルダーです。 mailSearchFolder は、mailFolder から継承します。
localization_priority: Normal
ms.openlocfilehash: 62d4d8569977c99690e317a39a43bbc9d9dca3f1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870393"
---
# <a name="mailsearchfolder-resource-type"></a>mailSearchFolder リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

MailSearchFolder は、指定した検索条件に一致するすべてのメール アイテムが含まれているユーザーのメールボックス内の仮想フォルダーです。 mailSearchFolder は、 [mailFolder](mailfolder.md)から継承します。

## <a name="methods"></a>メソッド

| メソッド | 戻り値の型  | 説明 |
|:---------------|:--------|:----------|
| [検索フォルダーを作成する](../api/mailsearchfolder-post.md) | [mailSearchFolder](mailsearchfolder.md) | このユーザーのメールボックスで検索フォルダーを作成します。 |
| [検索フォルダーの一覧](../api/mailfolder-list-childfolders.md) | [mailFolder](mailfolder.md) コレクション | 検索フォルダーを含む、このユーザーのメールボックス内のすべてのフォルダーを一覧表示します。 |
| [検索フォルダ―を取得する](../api/mailfolder-get.md) | [mailSearchFolder](mailsearchfolder.md) | 指定した検索フォルダーを取得します。 |
| [検索フォルダーを更新する](../api/mailsearchfolder-update.md) | [mailSearchFolder](mailsearchfolder.md) | 指定した検索フォルダーを更新します。 |
| [検索フォルダーを削除する](../api/mailfolder-delete.md) | なし | 指定した検索フォルダーを削除します。 |
| [検索フォルダー内のすべてのメッセージを一覧表示します。](../api/mailfolder-list-messages.md) | [message](message.md) コレクション | 指定した検索フォルダー内のすべてのメッセージを一覧表示します。 |

## <a name="properties"></a>プロパティ

| プロパティ | 種類 | 説明 |
|:---------------|:--------|:----------|
| 参照して | ブール型 | 検索フォルダーは、REST Api を使用して編集可能かどうかを示します。 |
| includeNestedFolders | ブール型 | メールボックス フォルダー階層を走査する方法を示します。 `true`詳細検索をする必要があることを意味時に`false`簡易検索を代わりに行う必要があることを意味します。 |
| sourceFolderIDs | String コレクション | メールボックス フォルダーをマイニングする必要があります。 |
| filterQuery | String | メッセージをフィルタ リングする OData クエリです。 |

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
<!-- {
  "type": "#page.annotation",
  "description": "mailSearchFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
