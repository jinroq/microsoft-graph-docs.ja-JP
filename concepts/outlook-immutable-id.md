---
title: Outlook リソースの不変の識別子を取得します。
description: 'または大きなストレスが発生した可能性があることに気付きませんでしたか、注目に値する動作を outlook のアイテム (メッセージ、イベント、連絡先、タスクなど) がある: その Id を変更します。 しない場合に発生する多くの場合、だけアイテムを移動するが、後で使用できるオフラインの Id を格納するアプリケーションで実際に問題が発生することができます。 不変の識別子は、アイテムの有効期間は変更されませんが、ID を取得するようにアプリケーションを有効にします。'
ms.openlocfilehash: a7b188c968ad6e0bf93f92ec99cb473075f29a4d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092514"
---
# <a name="get-immutable-identifiers-for-outlook-resources"></a>Outlook リソースの不変の識別子を取得します。

または大きなストレスが発生した可能性があることに気付きませんでしたか、注目に値する動作を outlook のアイテム (メッセージ、イベント、連絡先、タスクなど) がある: その Id を変更します。 しない場合に発生する多くの場合、だけアイテムを移動するが、後で使用できるオフラインの Id を格納するアプリケーションで実際に問題が発生することができます。 不変の識別子は、アイテムの有効期間は変更されませんが、ID を取得するようにアプリケーションを有効にします。

> **重要な:** 不変の識別子は、Microsoft Graph で/beta のバージョンでの使用のみです。

## <a name="how-it-works"></a>しくみ

不変の ID は、Microsoft のグラフのオプション機能です。 オプトインすると、アプリケーションは、API 要求に追加の HTTP ヘッダーを送信する必要があります。

```http
Prefer: IdType="ImmutableId"
```

このヘッダーに付属しています要求にのみ適用されます。 常に不変の Id を使用する場合は、API のすべての要求でこのヘッダーを含める必要があります。

## <a name="lifetime-of-immutable-ids"></a>不変の Id の有効期間

アイテムが同じメールボックスに保持している限り、アイテムの変更不可の ID は変更されません。 メールボックス内の別のフォルダーにアイテムを移動する場合に、不変の ID が変更されないことを意味します。 ただし場合は、不変の ID は変更されます。

- ユーザーがアーカイブ メールボックスにアイテムを移動します。
- ユーザーが (PST ファイルのメッセージなど) にアイテムをエクスポートし、各自のメールボックスに再インポートすることです。

## <a name="items-that-support-immutable-id"></a>不変の ID をサポートしている項目

次の項目では、不変の Id をサポートします。

- [メッセージ リソースの種類](/graph/api/resources/message?view=graph-rest-beta)
- [添付ファイル リソースの種類](/graph/api/resources/attachment?view=graph-rest-beta)
- [イベント リソースの種類](/graph/api/resources/event?view=graph-rest-beta)
- [eventMessage リソースの種類](/graph/api/resources/eventmessage?view=graph-rest-beta)
- [contact リソース型](/graph/api/resources/contact?view=graph-rest-beta)
- [outlookTask リソースの種類](/graph/api/resources/outlooktask?view=graph-rest-beta)

コンテナーの種類 (mailFolder、予定表など) は、不変の ID をサポートしていませんが、正規の Id の定数が存在しました。

## <a name="immutable-id-with-change-notifications"></a>変更通知の ID を変更できません。

含めることによって不変の Id での変更通知を送信する Microsoft Graph を要求することができます、`Prefer: IdType="ImmutableId"`ヘッダーと[サブスクリプションを作成](/graph/api/subscription-post-subscriptions?view=graph-rest-beta)します。 ヘッダーなしで作成された既存のサブスクリプションは、ID の既定の形式を使用する続行されます。 不変の Id を使用する既存のサブスクリプションを切り替えるには、削除し、ヘッダーを使用してそれらを再作成する必要があります。

## <a name="immutable-id-with-delta-query"></a>デルタのクエリを使用して ID を変更できません。

Microsoft Graph などによってサポートされているリソースの種類の[クエリ応答のデルタ](delta-query-overview.md)に不変の Id を返すことを要求することができます、`Prefer: IdType="ImmutableId"`ヘッダー。 `nextLink`と`deltaLink`アプリケーションは、不変の ID の利用を再同期化する必要はありませんので、デルタのクエリによって返される値は両方の ID の形式と互換性のあります。 今後、不変の Id を取得するヘッダーを使用することができ、[更新](#updating-existing-data)することできます、アプリケーションのストレージとは別にします。

## <a name="updating-existing-data"></a>既存データの更新

既に何千もの正規の Id を格納するデータベースがあれば、 [translateExchangeIds](/graph/api/user-translateexchangeids?view=graph-rest-beta)関数を使用して、変更不可能な形式にこれらの Id を移行できます。 ターゲット形式に変換するのには Id を 1000 までの配列を提供することができます。

> **注:** 使用することができます`translateExchangeIds`Exchange Web サービス アプリケーションは、Microsoft Graph を移行します。

### <a name="example"></a>例

不変グラフ ID への通常のグラフ ID を変換する次の使用例

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