---
title: デルタ クエリを使用して、Microsoft Graph データの変更を追跡する
description: デルタ クエリを使用すると、アプリケーションは、要求ごとにターゲット リソースをすべて読み取ることなく、新しく作成、更新、または削除されたエンティティを検出できます。Microsoft Graph アプリケーションはデルタ クエリを使用して、変更をローカル データ ストアと効率的に同期させることができます。
author: piotrci
localization_priority: Priority
ms.openlocfilehash: e0affa6f4e3edf1289d31422dcd5833a4d5b17ff
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32526196"
---
# <a name="use-delta-query-to-track-changes-in-microsoft-graph-data"></a>デルタ クエリを使用して、Microsoft Graph データの変更を追跡する

デルタ クエリを使用すると、アプリケーションは、要求ごとにターゲット リソースをすべて読み取ることなく、新しく作成、更新、または削除されたエンティティを検出できます。Microsoft Graph アプリケーションはデルタ クエリを使用して、変更をローカル データ ストアと効率的に同期させることができます。

## <a name="use-delta-query-to-track-changes-in-a-resource-collection"></a>デルタ クエリを使用して、リソース コレクション内の変更を追跡する

標準的な呼び出しパターンは次のとおりです。

1. アプリケーションは、まず目的のリソースでデルタ関数を使用して GET 要求を呼び出します。
2. Microsoft Graph は、要求されたリソースと[状態トークン](#state-tokens)を含む応答を送信します。

     a. `nextLink` URL が返される場合は、セッションに取得するデータの追加ページがあります。`deltaLink` URL が応答で返されるまで、アプリケーションは `nextLink` URL を使用してデータのすべてのページを取得する要求を実行し続けます。

     b.`deltaLink` URL が返される場合、返されるリソースの既存の状態に関するデータはありません。以降の要求では、アプリケーションは `deltaLink` URL を使用して、リソースへの変更点を確認します。

3. アプリケーションがリソースの変更を把握する必要がある場合、アプリケーションは手順 2 で受け取った `deltaLink` URL を使用して、新しい要求を実行します。この要求は、手順 2 が完了した直後、またはアプリケーションが変更を確認する際に実行できる*場合があります*。
4. Microsoft Graph は、前の要求以降のリソースへの変更を説明する応答と、`nextLink` URL または `deltaLink` URL のいずれかを返します。

>**注:** Azure Active Directory (ユーザーやグループなど) に保管されているリソースは、"今から同期を開始する" という状況をサポートしています。 このため、上記の手順 1 と 2 をスキップし (リソースの完全な状態を取得する必要がない場合)、代わりに最新の `deltaLink` を要求することができます。 `$deltaToken=latest` を `delta` 関数に追加すると、応答には `deltaLink` が含まれ、リソー スデータは一切含まれません。

### <a name="state-tokens"></a>状態トークン

デルタ クエリの GET 応答には、`nextLink` または `deltaLink` の応答ヘッダーに指定された URL が常に含まれています。`nextLink` URL には _skipToken_、`deltaLink` URL には _deltaToken_ が含まれています。

これらのトークンは、クライアントに対して不透明です。理解しておく必要のある事項の詳細を、以下に示します。

- 各トークンは状態を反映し、そのラウンドの変更追跡におけるリソースのスナップショットを表します。

- 状態トークンは、初期デルタ クエリ要求で指定された他のクエリ パラメーター (`$select` など) もエンコードして含めます。したがって、後続のデルタ クエリ要求でそれらを繰り返す必要はありません。

- デルタ クエリを実行するときは、状態トークンなど、URL の内容を調べることなく、`nextLink` または `deltaLink` の URL を次の**デルタ**関数呼び出しにコピーして適用できます。

### <a name="optional-query-parameters"></a>オプションのクエリ パラメーター

クライアントがクエリ パラメーターを使用する場合は、最初の要求で指定する必要があります。Microsoft Graph は、応答で提供される `nextLink` または `deltaLink` に指定したパラメーターを自動的にエンコードします。呼び出し元のアプリケーションで必要な操作は、必要なクエリ パラメーターを最初に一度指定することだけです。Microsoft Graph は、すべての後続の要求に対して自動的に指定されたパラメーターを追加します。

ユーザーとグループには、いくつかのクエリ パラメーターの使用に関する制限があります。

- `$select` クエリ パラメーターが使用されている場合、パラメーターは、`$select` ステートメントで指定したプロパティまたはリレーションシップに関する変更のみを追跡することを、クライアントが優先していることを示します。選択されていないプロパティに変更が加えられた場合、そのプロパティが変更されたリソースは、後続の要求後のデルタ応答には表示されなくなります。
- `$expand` は、それぞれのユーザーとグループのナビゲーション プロパティである `manager` および `members` についてのみサポートされます。

- スコープ フィルターで、objectID を使って 1 つまたは複数の特定のユーザーまたはグループに加えられた変更を追跡できます。 たとえば、https://graph.microsoft.com/beta/groups/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ae5f' or id eq '004d6a07-fe70-4b92-add5-e6e37b8acd8e' の要求では、クエリ フィルターで指定された ID に一致するグループに加えられた変更が返されます。

## <a name="resource-representation-in-the-delta-query-response"></a>デルタ クエリ応答でのリソース表記

- サポートされているリソースの新しく作成されたインスタンスは、標準的な表現を使用してデルタ クエリ応答で表されます。

- 更新されたインスタンスは、*少なくとも*更新されたプロパティを持つ **ID** で表されますが、追加のプロパティが含まれる可能性があります。

- ユーザーとグループのリレーションシップは、標準的なリソース表記で注釈として表されます。これらの注釈は `propertyName@delta` の形式で表示されます。注釈は最初のデルタ クエリ要求の応答に含まれます。

削除されたインスタンスは、**ID** と `@removed` オブジェクトを使用して表されます。`@removed` オブジェクトには、インスタンスが削除された理由に関する追加情報が含まれる場合があります。たとえば、"@removed": {"reason": “changed”} です。

"@removed" で考えられる理由は、*changed* または *deleted* です。

- *Changed* は、項目は削除されたものの、[deletedItems](/graph/api/resources/directory?view=graph-rest-beta) から復元できることを表します。

- *Deleted* は、項目は削除され、復元できないことを表します。

`@removed` オブジェクトは最初のデルタ クエリ応答と追跡された (deltaLink) 応答で返されます。デルタ クエリ要求を使用するクライアントは、応答に含まれるこれらのオブジェクトを処理できるよう設計する必要があります。

## <a name="supported-resources"></a>サポートされているリソース

デルタ クエリは現在、次のリソースでサポートされています。

| **リソース コレクション** | **API** |
|:------ | :------ |
| アプリケーション (プレビュー) | [アプリケーション](/graph/api/resources/application?view=graph-rest-beta) リソース (プレビュー) の[デルタ](/graph/api/application-delta?view=graph-rest-beta)関数 |
| ディレクトリ オブジェクト | [ディレクトリ オブジェクト](/graph/api/resources/directoryobject?view=graph-rest-beta) リソース (プレビュー) の[デルタ](/graph/api/directoryobject-delta?view=graph-rest-beta)関数 |
| ディレクトリ ロール | [ディレクトリ ロール](/graph/api/resources/directoryrole?view=graph-rest-1.0) リソースの[デルタ](/graph/api/directoryrole-delta?view=graph-rest-1.0)関数 |
| 標準として設定されている予定表の予定表ビュー (期間) 内のイベント | [イベント](/graph/api/resources/event?view=graph-rest-1.0)リソースの[デルタ](/graph/api/event-delta?view=graph-rest-1.0)関数 |
| グループ | [グループ](/graph/api/resources/group?view=graph-rest-1.0)リソースの[デルタ](/graph/api/group-delta?view=graph-rest-1.0)関数 |
| メール フォルダー | [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-1.0) リソースの[デルタ](/graph/api/mailfolder-delta?view=graph-rest-1.0)関数 |
| フォルダー内のメッセージ | [メッセージ](/graph/api/resources/message?view=graph-rest-1.0)リソースの[デルタ](/graph/api/message-delta?view=graph-rest-1.0)関数 |
| 個人用連絡先フォルダー | [contactFolder](/graph/api/resources/contactfolder?view=graph-rest-1.0) リソースの[デルタ](/graph/api/contactfolder-delta?view=graph-rest-1.0)関数 |
| フォルダー内の個人用連絡先 | [連絡先](/graph/api/resources/contact?view=graph-rest-1.0)リソースの[デルタ](/graph/api/contact-delta?view=graph-rest-1.0)関数 |
| サービス プリンシパル (プレビュー) | [サービス プリンシパル](/graph/api/resources/serviceprincipal?view=graph-rest-beta) リソース (プレビュー) の[デルタ](/graph/api/serviceprincipal-delta?view=graph-rest-beta)関数 |
| ユーザー | [ユーザー](/graph/api/resources/user?view=graph-rest-1.0)リソースの[デルタ](/graph/api/user-delta?view=graph-rest-1.0)関数 |
| ドライブの項目\* | [driveItem](/graph/api/resources/driveitem?view=graph-rest-1.0) リソースの[デルタ](/graph/api/driveitem-delta?view=graph-rest-1.0)関数 |
| Planner の項目\*\* | [plannerUser](/graph/api/resources/planneruser?view=graph-rest-beta) リソースのすべてのセグメントの[デルタ](/graph/api/planneruser-list-delta?view=graph-rest-beta)関数 (プレビュー) |

> \* OneDrive リソースの使用パターンは、他のサポートされているリソースと似ていますが、構文には若干の違いがあります。 ドライブのデルタ クエリは、他のリソースの種類との一貫性を保つために将来更新されます。 現在の構文の詳細については、 「[ドライブの変更履歴を記録する](/graph/api/driveitem-delta?view=graph-rest-1.0)」を参照してください。

> \*\* Planner リソースの使用パターンは、他のサポートされているリソースと似ていますが、若干の違いがあります。  詳細については、「[Planner の変更履歴を記録する](/graph/api/planneruser-list-delta?view=graph-rest-beta)」を参照してください。

## <a name="prerequisites"></a>前提条件

特定のリソースを読み取るために必要な[アクセス許可](./permissions-reference.md)と同じアクセス許可も、そのリソースでデルタ クエリを実行するために必要です。

## <a name="delta-query-request-examples"></a>デルタ クエリ要求の例

- [カレンダー ビューのイベントへの増分の変更を取得する](delta-query-events.md)
- [フォルダー内のメッセージへの増分の変更を取得する](./delta-query-messages.md)
- [グループへの増分の変更を取得する](./delta-query-groups.md)
- [ユーザーへの増分の変更を取得する](./delta-query-users.md)
