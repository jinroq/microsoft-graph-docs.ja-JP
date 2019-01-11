---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: 旧バージョンの SharePoint リスト アイテムを復元する
localization_priority: Normal
ms.openlocfilehash: 0df91bfb33ba395de4724c1ac1a72dc69f8d15e1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811390"
---
# <a name="restore-a-previous-version-of-a-listitem"></a>旧バージョンのリスト アイテムを復元する

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

旧バージョンのリスト アイテムを現在のバージョンに復元します。 旧バージョンのコンテンツを持つ新しいバージョンを作成します。しかし、アイテムの既存のバージョンはすべて保持されます。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|            アクセス許可の種類             |         アクセス許可 (特権の小さいものから大きいものへ)          |
| :------------------------------------- | :----------------------------------------------------------- |
| 委任 (職場または学校のアカウント)     | Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All |
| 委任 (個人用 Microsoft アカウント) | 該当なし                                                          |
| アプリケーション                            | Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a>要求本文

要求の本文は必要ありません。

## <a name="example"></a>例

この例では、`{item-id}` と `{version-id}` で識別されるリスト アイテムのバージョンを復元します。

<!-- { "blockType": "request", "name": "restore-item-version-listItem", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

## <a name="response"></a>応答

成功すると、API 呼び出しは `204 No content` を返します。

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy"
} -->
