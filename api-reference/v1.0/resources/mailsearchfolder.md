---
title: mailSearchFolder リソースの種類
description: MailSearchFolder は、指定した検索条件に一致するすべての電子メールアイテムを含む、ユーザーのメールボックス内の仮想フォルダーです。 mailSearchFolder は mailFolder から継承します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 0980a99567a93b48c4bd75ef3510c51347d8d794
ms.sourcegitcommit: b742da101a3a232356bf748c42da3ba08a7539d3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/10/2019
ms.locfileid: "34818683"
---
# <a name="mailsearchfolder-resource-type"></a>mailSearchFolder リソースの種類

**Mailsearchfolder**は、指定した検索条件に一致するすべての電子メールアイテムを含む、ユーザーのメールボックス内の仮想フォルダーです。 **Mailsearchfolder**は[mailfolder](mailfolder.md)から継承します。 検索フォルダーは、ユーザーの Exchange Online メールボックス内の任意のフォルダーに作成できます。 ただし、検索フォルダーが Outlook、web 用の Outlook、または Outlook Live に表示されるようにするには、 **WellKnownFolderName**フォルダー内にフォルダーを作成する必要があります。 

## <a name="search-folder-lifecycle"></a>検索フォルダーのライフサイクル

アプリケーションによって作成された検索フォルダーは、次のいずれかの理由により、Exchange Online で削除できます。

1.  検索フォルダーは利用できなくなってから45日後に有効期限が切れます。 
2.  ソースフォルダーごとに作成できる検索フォルダーの数には制限があります。 この制限が侵害された場合は、古い検索フォルダーが削除され、新しいフォルダーを使用できるようになります。 

検索フォルダーが削除されると、アプリは新しい検索フォルダーリソースを作成して同じものを使用する必要があります。


## <a name="methods"></a>メソッド

| メソッド | 戻り値の型  | 説明 |
|:---------------|:--------|:----------|
| [検索フォルダーを作成する](../api/mailsearchfolder-post.md) | [mailSearchFolder](mailsearchfolder.md) | このユーザーのメールボックスに検索フォルダーを作成します。 |
| [検索フォルダーを一覧表示する](../api/mailfolder-list-childfolders.md) | [mailFolder](mailfolder.md) コレクション | このユーザーのメールボックス内のすべてのフォルダー (検索フォルダーを含む) を一覧表示します。 |
| [検索フォルダ―を取得する](../api/mailfolder-get.md) | [mailSearchFolder](mailsearchfolder.md) | 指定した検索フォルダーを取得します。 |
| [検索フォルダーを更新する](../api/mailsearchfolder-update.md) | [mailSearchFolder](mailsearchfolder.md) | 指定した検索フォルダーを更新します。 |
| [検索フォルダーを削除する](../api/mailfolder-delete.md) | None | 指定した検索フォルダーを削除します。 |
| [検索フォルダー内のすべてのメッセージを一覧表示する](../api/mailfolder-list-messages.md) | [message](message.md) コレクション | 指定した検索フォルダー内のすべてのメッセージを一覧表示します。 |

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:---------------|:--------|:----------|
| isSupported | Boolean | 検索フォルダーが REST Api を使用して編集可能かどうかを示します。 |
| includeNestedFolders | Boolean | 検索でメールボックスフォルダー階層をスキャンする方法を示します。 `true`**sourceFolderIds**で明示的に指定された各フォルダーの階層内に子フォルダーを含めるには、詳細検索を実行する必要があることを意味します。 `false`は、 **sourceFolderIds**で明示的に指定された各フォルダーの浅い検索を意味します。 |
| sourceFolderIds | 文字列コレクション | マイニングするメールボックスフォルダー。 |
| filterQuery | String | メッセージをフィルター処理するための OData クエリ。 |

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
  "sourceFolderIds": ["string"],
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
