---
title: Azure AD Graph と Microsoft Graph の機能の違い
description: アプリをすばやく簡単に移行できるように、Azure Active Directory (Azure AD) API と Microsoft Graph API の機能の違いについて説明します。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0e18bc286f4373c15da9d6a2360491e1b2f0371f
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33630245"
---
# <a name="feature-differences-between-azure-ad-graph-and-microsoft-graph"></a>Azure AD Graph と Microsoft Graph の機能の違い

この記事は、*手順 1:* [アプリを移行するプロセス](migrate-azure-ad-graph-planning-checklist.md)の API の相違点を確認します。

Microsoft Graph の多くの機能は、Azure AD Graph に対応しています。 ただし、いくつかの変更や改善が行われています。 ここでは、これらの違いを活用するようにアプリを調整する方法について説明します。  多くの場合、変更は軽微ですが、労力を費やす価値があります。

この記事では、Microsoft Graph の処理方法について説明します。

- ディレクトリ スキーマの拡張
- 差分クエリ
- バッチ処理

## <a name="directory-schema-extensions"></a>ディレクトリ スキーマの拡張

アプリで Azure AD Graph ディレクトリスキーマ拡張機能を使用している場合は、次のように、同じ基本 Api (Microsoft Graph 要求 Url を使用) を引き続き使用できます。

- GET とを使用して拡張機能の値を読み取る`$select`
- GET とを使用して拡張機能値を検索する`$filter`
- PATCH を使用して拡張機能の値を更新する
- PATCH を使用して拡張機能の値を削除する ( **null**に設定)

ただし、Microsoft Graph では、Azure AD Graph ディレクトリのスキーマ拡張機能の定義を管理したり、テナントで使用可能なすべてのスキーマ拡張機能の定義を表示したりすることはできません。

代わりに、Microsoft Graph は、拡張可能なスキーマ拡張機能を提供します。ここでは、Azure AD Graph ディレクトリスキーマの extentions との下位互換性がありません。 詳細については、「 [add custom data」の「スキーマ拡張機能](/graph/extensibility-overview#schema-extensions)」を参照してください。

### <a name="recommended-migration-approach"></a>推奨される移行方法

Azure AD Graph アプリがディレクトリスキーマ拡張機能を使用している場合は、アプリを Microsoft Graph に移行するための段階的なアプローチを取ります。

最初に、アプリを Microsoft Graph API 呼び出しを使用するように切り替えますが、アプリは Azure AD Graph ディレクトリスキーマ拡張機能を引き続き利用できます。

その後、Microsoft Graph スキーマ拡張機能の使用に切り替えることができます。 場合によっては、切り替えは適切ではありません。 次の場合に切り替えません。

- アプリは AD Connect によって作成されたディレクトリスキーマ拡張機能を使用します。
- アプリは、トークンクレームのディレクトリスキーマ拡張値に依存します。

>**注**: Microsoft Graph スキーマ拡張プロパティを、オプションのクレームを使用してトークン内のクレームとして使用することもまだサポートされていません。

新しい Microsoft Graph スキーマ拡張モデルに切り替えるには、次の操作を行う必要があります。

- Microsoft Graph を使用して、新しいスキーマ拡張機能の定義を定義します。
- 新しいスキーマ拡張機能の定義をサポートするようにアプリを更新します。
- Azure AD スキーマ拡張機能のプロパティから新しい Microsoft Graph スキーマ拡張プロパティにデータを移行します。  データの自動移行はサポートされていません。

## <a name="differential-queries"></a>差分クエリ

Azure AD Graph と Microsoft Graph では、クエリを使用して変更を追跡できます。  高レベルの方法は、2つの Api 間で似ていますが、構文が異なります。  

Azure AD Graph は、これらの差分クエリを呼び出します。  Microsoft Graph では、これらは[デルタクエリ](/graph/delta-query-overview)です。

次の表では、主な類似点と相違点について取り上げます。

||Azure AD Graph | Microsoft Graph |
|----|----|----|
| _最初のデータ要求_ | クエリパラメーターを使用します。<br>`GET /groups?deltaLink=` | 関数を使用します。 <br> `GET /groups/delta` |
| _新しい変更を取得する_ | `GET /groups?deltaLink={deltaToken}` | `GET /groups/delta?$deltaToken={deltaToken}` |
| _今すぐ同期_ |カスタム HTTP ヘッダーを使用します。<br> `ocp-aad-dq-include-only-delta-token: true` | クエリパラメーターを使用します。 <br> `GET /groups/delta?$deltaToken=latest` |
| _DirectoryObjects の変更を追跡する_ | 同じ操作で複数のリソース (ユーザーとグループ) の変更を取得します。&nbsp;&nbsp;<br> `GET /directoryObject?$filter=isof('User') or isof('Group')&deltaLink=` | は、Microsoft Graph で個別のクエリを使用し、1つはリソースごとに使用します。 |
| _リソースおよびリレーションシップの変更を取得する_ | リソースがリレーションシップを持っている場合、すべての要求はリソースおよびリレーションシップの変更を返します。 | `GET /groups/delta?$expand=members` |
| _新規および変更されたアイテムを示す応答_ | <ul><li><p>標準表現を使用して、新しく作成されたインスタンスを表します。</p></li><li><p>更新されたインスタンスは、*少なく*とも更新されたプロパティを持つ id で表されます。 その他のプロパティが含まれている場合があります。</p></li><li><p>リレーションシップは、 `directoryLinkChange`型として表されます。</p></li></ul>|<ul><li><p>標準表現を使用して、新しく作成されたインスタンスを表します。</p></li><li><p>更新されたインスタンスは、*少なく*とも更新されたプロパティを持つ id で表されます。 その他のプロパティが含まれている場合があります。</p></li><li><p>リレーションシップは、標準のリソース表現における注釈として表されます。 これらの注釈は、 `propertyName@delta`グループのメンバーシップ`members@delta`の変更などの形式を使用します。</p></li></ul> |
| _削除済みアイテムを示す応答_| *Aad*が true に設定された追加のプロパティを持つ削除済みアイテムがあることを示します。 | 削除された注釈が\@含まれる削除済みアイテムを示します。 また、アイテムが削除された場合でも、復元できるかどうか、または完全に削除されているかどうかを示す理由コードが含まれている場合があります。 |

アプリに既に状態データが格納されている場合は、前に示した「今すぐ同期」を使用して、デルタクエリへの移行を管理することを検討してください。

## <a name="batching"></a>バッチ処理

Azure AD Graph は、マルチパート MIME メッセージと呼ばれるシステムを使用して、バッチ処理を管理しています。  Microsoft Graph では、1回のバッチ操作で最大20個の要求を許可するために、 [JSON バッチ](json-batching.md)処理を使用します。 JSON のバッチ処理機構は、特に JSON 解析ライブラリと組み合わせて使用する方がはるかに簡単です。  また、バッチ処理を順序付けることもできます。  ただし、Azure AD Graph のバッチ処理方法との下位互換性はありません。

## <a name="next-steps"></a>次のステップ

- Azure AD Graph と Microsoft Graph の[リソースの相違点](migrate-azure-ad-graph-resource-differences.md)について説明します。
- [開く] [[カスタムデータの追加](/graph/extensibility-overview)] を参照して、オープンおよびスキーマの拡張機能に関する情報を確認します
- [デルタクエリ](/graph/delta-query-overview)を調査して、Microsoft Graph の差分クエリのバージョンについて説明します。
- Microsoft Graph でのバッチ処理の動作を理解するために、 [JSON バッチ](json-batching.md)を調査します。
- [Graph エクスプローラー](https://aka.ms/ge)を使用して、Microsoft graph を試してみてください。

<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Warning: /concepts/migrate-azure-ad-graph-feature-changes.md:
      Failed to parse any rows out of table with headers: |Task|Azure AD Graph|Microsoft Graph|"
  ],
}
-->
