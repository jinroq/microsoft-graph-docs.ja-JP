---
title: Microsoft グラフ API を使用して、アプリケーションでは、ソーシャル ・ インテリジェンスを統合するために
description: Graph では、コンテキストでは、ユーザーのソーシャル、ソーシャルのジェスチャをサポートしているし、便利な人や社会のデータにアクセスを提供します。
localization_priority: Priority
ms.openlocfilehash: b3b71cf1bad0d860978c75c88f0b77a32eab1a0c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862490"
---
# <a name="use-the-microsoft-graph-api-to-integrate-social-intelligence-in-an-app"></a>Microsoft グラフ API を使用して、アプリケーションでは、ソーシャル ・ インテリジェンスを統合するために

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

Graph では、コンテキストでは、ユーザーのソーシャル、ソーシャルのジェスチャをサポートしているし、便利な人や社会のデータにアクセスを提供します。

## <a name="aggregate-and-extract-specific-information-about-people"></a>集約し、他のユーザーに関する特定の情報を抽出

メール、連絡先、およびソーシャル ネットワークの間で[ユーザー](../resources/person.md)リソースとユーザー API から、ある人物に関する情報を集約を使用します。 結果は、複数の通信、コラボレーション、および取引関係に基づく妥当性で並べ替えられます。 API は、参照、並べ替え、選択、フィルター、またはの条件に基づいてユーザーを検索することができます。

- [ユーザーを一覧表示する](../api/user-list-people.md)

## <a name="manage--mentions"></a>@-参照投稿を管理します。

受信者に通知し、メッセージ内の受信者の注意を引くために呼び出すことは、一般的なソーシャル ジェスチャです。
[説明](../resources/mention.md)リソースに関する API[メッセージ](../resources/message.md)の受信者を @ の説明を使用してユーザーに通知するすべてのメッセージを取得するには、軽量のメカニズムを提供やメッセージに記載されている各を取得します。

<!--
Include the next sentence when supporting events.

**Mention** is also supported by [Event](../resources/event.md).

-->

- 新しいメッセージ内にメンションを作成する

  - [新しいメッセージの一部としてメンションを作成および送信する](../api/user-sendmail.md#request-2)
  - [下書きの一部としてメンションを作成する](../api/user-post-messages.md#request-2)

- メッセージのメンションに関する情報を取得する

  - [ユーザーに言及する、サインイン中のユーザーのメールボックス内のすべてのメッセージを取得します。](../api/user-list-messages.md#request-2)
  - [メッセージ内の各メンションの詳細の取得](../api/message-get.md#request-2)

- メッセージで[参照を削除](../api/message-delete.md#request-2)

## <a name="access-social-data-around-and-about-a-user"></a>周りと、ユーザーのソーシャル データにアクセス

Office のグラフは、Office 365 内の別のエンティティ間の関係をカプセル化します。 Office 365 の間で個々 のユーザーのソーシャル洞察を取得するのにには、Office のグラフを使用します。

- アイテム[の周囲にトレンド ・](../api/insights-list-trending.md)ユーザーの一覧を表示します。
- [使用](../api/user-list-people.md)されているユーザーのユーザーを一覧表示します。
