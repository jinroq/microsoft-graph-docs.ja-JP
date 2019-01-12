---
title: Outlook リソースの不変 ID の取得
description: Outlook アイテム (メッセージ、イベント、連絡先、タスク) には、ユーザーは気づいていないか、大きな不満を感じている可能性のある、興味深い動作があります。それは、ID の変更です。 これは頻繁に発生するものではなく、アイテムが移動された場合のみ発生します。ただし、後で使用するために ID をオフラインで格納するアプリの場合、これは深刻な問題になることがあります。 不変 ID を使用すると、お使いのアプリケーションで、アイテムの有効期間中は変更のない ID を取得できます。
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: e88f4d457f76990dc3e6145ebf2730087ad2a74e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27961716"
---
# <a name="get-immutable-identifiers-for-outlook-resources"></a>Outlook リソースの不変 ID の取得

Outlook アイテム (メッセージ、イベント、連絡先、タスク) には、ユーザーは気づいていないか、大きな不満を感じている可能性のある、興味深い動作があります。それは、ID の変更です。 これは頻繁に発生するものではなく、アイテムが移動された場合のみ発生します。ただし、後で使用するために ID をオフラインで格納するアプリの場合、これは深刻な問題になることがあります。 不変 ID を使用すると、お使いのアプリケーションで、アイテムの有効期間中は変更のない ID を取得できます。

> **重要:** 不変 ID は、Microsoft Graph のベータ版のみで使用できます。

## <a name="how-it-works"></a>しくみ

不変 ID は、Microsoft Graph のオプション機能です。 オプト インするには、アプリケーションから、API 要求に追加の HTTP ヘッダーを含めて送信する必要があります。

```http
Prefer: IdType="ImmutableId"
```

このヘッダーは、それが含まれる要求にのみ適用されます。 常に不変 ID を使用したい場合は、このヘッダーをすべての API 要求に含める必要があります。

## <a name="lifetime-of-immutable-ids"></a>不変 ID の有効期間

アイテムの不変 ID は、アイテムが同じメールボックス内にある限り、変更されません。 つまり、アイテムがメールボックス内の別のフォルダーに移動しても、不変 ID は変更されません。 ただし、次の場合、不変 ID は変更されます。

- ユーザーがアイテムをアーカイブ メールボックスに移動した
- ユーザーがアイテムをエクスポートし (PST へのエクスポート、MSG ファイルとしてのエクスポートなど)、それをメールボックスに再度インポートした

## <a name="items-that-support-immutable-id"></a>不変 ID をサポートするアイテム

不変 ID をサポートするアイテムは次のとおりです。

- [message リソース型](/graph/api/resources/message?view=graph-rest-beta)
- [attachment リソース型](/graph/api/resources/attachment?view=graph-rest-beta)
- [event リソース型](/graph/api/resources/event?view=graph-rest-beta)
- [eventMessage リソース型](/graph/api/resources/eventmessage?view=graph-rest-beta)
- [contact リソース型](/graph/api/resources/contact?view=graph-rest-beta)
- [outlookTask リソース型](/graph/api/resources/outlooktask?view=graph-rest-beta)

コンテナー型 (mailFolder、calendar など) は不変 ID をサポートしませんが、コンテナー型の標準 ID は既に不変です。

## <a name="immutable-id-with-change-notifications"></a>変更通知を使用する不変 ID

[サブスクリプションの作成](/graph/api/subscription-post-subscriptions?view=graph-rest-beta)時に `Prefer: IdType="ImmutableId"`ヘッダーを含めることで、Microsoft Graph が変更通知で不変 ID を送信するように要求することができます。 このヘッダーなしで作成された既存のサブスクリプションは、既定の ID 形式を使用し続けます。 既存のサブスクリプションを、不変 ID を使用するように切り替えるには、そのサブスクリプションを削除し、このヘッダーを使用して作成し直す必要があります。

## <a name="immutable-id-with-delta-query"></a>デルタ クエリを使用する不変 ID

`Prefer: IdType="ImmutableId"` ヘッダーを含めることで、Microsoft Graph が不変 ID を、サポートされるリソース型に関する[デルタ クエリ応答](delta-query-overview.md)で返すように要求することができます。 デルタ クエリによって返される `nextLink` と `deltaLink` の各値は、両方の ID 形式に対応しているので、アプリケーションは、不変 ID を利用するために再同期する必要はありません。 今後は、このヘッダーを使用して不変 ID を取得でき、[アプリの記憶域を個別に更新する](#updating-existing-data)ことができます。

## <a name="updating-existing-data"></a>既存のデータの更新

データベースが既に何千個もの標準 ID でいっぱいになっている場合、[translateExchangeIds](/graph/api/user-translateexchangeids?view=graph-rest-beta) 関数を使用して、それらの ID を不変形式に移行することができます。 最大 1000 個もの ID をターゲット形式に変換できます。

> **注:** `translateExchangeIds` を使用して、Exchange Web サービス アプリケーションを Microsoft Graph に移行することもできます。

### <a name="example"></a>例

次の例では、標準の Graph ID を不変の Graph ID に変換します。

#### <a name="request"></a>要求

```http
POST https://graph.microsoft.com/beta/me/translateExchangeIds

{
  "inputIds" :
  [
    "AQMkAGM2…"
  ],
  "targetIdType" : "restImmutableEntryId",
  "sourceIdType" : "restId"
}
```

#### <a name="response"></a>応答

```http
HTTP 200 OK

{
  "value": [
    {
      "targetId": "AAkALgAA...",
      "sourceId": "AQMkAGM2..."
    }
  ]
}
```
