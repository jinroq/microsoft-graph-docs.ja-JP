#  <a name="use-delta-query-to-track-changes-in-microsoft-graph-data-preview"></a>デルタ クエリを使用して、Microsoft Graph データの変更を追跡する (プレビュー)

デルタ クエリを使用すると、アプリケーションは、要求ごとにターゲット リソースをすべて読み取ることなく、新しく作成、更新、または削除されたエンティティを検出できます。Microsoft Graph アプリケーションはデルタ クエリを使用して、変更をローカル データ ストアと効率的に同期させることができます。

## <a name="use-delta-query-to-track-changes-in-a-resource-collection"></a>デルタ クエリを使用して、リソース コレクション内の変更を追跡する

標準的な呼び出しパターンは次のとおりです。

1.  アプリケーションは、まず目的のリソースでデルタ関数を使用して GET 要求を呼び出します。
2.  Microsoft Graph は、要求されたリソースと[状態トークン](#state-tokens)を含む応答を送信します。

     a.`nextLink` URL が返される場合は、セッションに取得するデータの追加ページがあります。`deltaLink` URL が応答で返されるまで、アプリケーションは `nextLink` URL を使用して要求を実行し続けます。

     b.`deltaLink` URL が返される場合、返されるリソースの既存の状態に関するデータはありません。以降の要求では、アプリケーションは `deltaLink` URL を使用して、リソースへの変更点を確認します。
     
3.  アプリケーションがリソースの変更を把握する必要がある場合、アプリケーションは手順 2 で受け取った `deltaLink` URL を使用して、新しい要求を実行します。この要求は、手順 2 が完了した直後、またはアプリケーションが変更を確認する際に実行できる*場合があります*。
4.  Microsoft Graph は、前の要求以降のリソースへの変更を説明する応答と、`nextLink` URL または `deltaLink` URL のいずれかを返します。

### <a name="state-tokens"></a>状態トークン

デルタ クエリの GET 応答には、`nextLink` または `deltaLink` の応答ヘッダーに指定された URL が常に含まれています。`nextLink` URL には _skipToken_、`deltaLink` URL には _deltaToken_ が含まれています。 

これらのトークンは、クライアントに対して不透明です。理解しておく必要のある事項の詳細を、以下に示します。

- 各トークンは状態を反映し、そのラウンドの変更追跡におけるリソースのスナップショットを表します。 
- 状態トークンは、初期デルタ クエリ要求で指定された他のクエリ パラメーター (`$select` など) もエンコードして含めます。したがって、後続のデルタ クエリ要求でそれらを繰り返す必要はありません。
- デルタ クエリを実行するときは、状態トークンなど、URL の内容を調べることなく、`nextLink` または `deltaLink` の URL を次の**デルタ**関数呼び出しにコピーして適用できます。


### <a name="optional-query-parameters"></a>オプションのクエリ パラメーター

クライアントがクエリ パラメーターを使用する場合は、最初の要求で指定する必要があります。Microsoft Graph は、応答で提供される `nextLink` または `deltaLink` に指定したパラメーターを自動的にエンコードします。呼び出し元のアプリケーションで必要な操作は、必要なクエリ パラメーターを最初に一度指定することだけです。Microsoft Graph は、すべての後続の要求に対して自動的に指定されたパラメーターを追加します。

ユーザーとグループには、いくつかのクエリ パラメーターの使用に関する制限があります。

-   `$select` クエリ パラメーターが使用されている場合、パラメーターは、`$select` ステートメントで指定したプロパティまたはリレーションシップに関する変更のみを追跡することを、クライアントが優先していることを示します。選択されていないプロパティに変更が加えられた場合、そのプロパティが変更されたリソースは、後続の要求後にデルタ応答には表示されなくなります。
-   `$expand` はサポートされていません。

## <a name="resource-representation-in-the-delta-query-response"></a>デルタ クエリ応答でのリソース表記

-   サポートされているリソースの新しく作成されたインスタンスは、標準的な表現を使用してデルタ クエリ応答で表されます。

-   更新されたインスタンスは、*少なくとも*更新されたプロパティを持つ **ID** で表されますが、追加のプロパティが含まれる可能性があります。

-   ユーザーとグループとのリレーションシップに対する変更は、標準的なリソース表記で注釈として表されます。これらの注釈は、`propertyName@delta` の形式を使用し、クライアントが `$select` パラメーターを使用して、リレーションシップへの変更を追跡することを明示的に選択した場合にのみ表示されます。

-   削除されたインスタンスは、**ID** と `@removed` ノードのみを使用して表されます。`@removed` ノードには、インスタンスが削除された理由に関する追加情報が含まれる場合があります。

> **将来の変更に関する注意**：削除されたインスタンスは、現在 `@removed` ノードを使用して次の形式で表示されます: *“@removed” : “削除の理由”*。ただし、将来的には大きく変更されます。デルタ クエリが /beta から /v1.0 に移行する前に、オブジェクトは削除されたノード内に入れ子にされ、より多くの情報を提供します。例: *@removed {reason: “削除の理由”}*。このオブジェクトは将来、削除に関する追加のメタデータを含むように拡張できます。

## <a name="supported-resources"></a>サポートされているリソース

デルタ クエリは現在、次のリソースの Microsoft Graph /beta エンドポイントのプレビューでサポートされています。

| **リソース コレクション** | **API** |
|:------ | :------ |
| 標準として設定されている予定表の予定表ビュー (期間) 内のイベント | [イベント](../api-reference/beta/resources/event.md)リソースの[デルタ](../api-reference/beta/api/event_delta.md)関数 |
| グループ | [グループ](../api-reference/beta/resources/group.md)リソースの[デルタ](../api-reference/beta/api/group_delta.md)関数 |
| メール フォルダー | [mailFolder](../api-reference/beta/resources/mailFolder.md) リソースの[デルタ](../api-reference/beta/api/mailfolder_delta.md)関数 |
| フォルダー内のメッセージ | [メッセージ](../api-reference/beta/resources/message.md)リソースの[デルタ](../api-reference/beta/api/message_delta.md)関数 | 
| 個人用連絡先フォルダー | [contactFolder](../api-reference/beta/resources/contactfolder.md) リソースの[デルタ](../api-reference/beta/api/contactfolder_delta.md)関数 |
| フォルダー内の個人用連絡先 | [連絡先](../api-reference/beta/resources/contact.md)リソースの[デルタ](../api-reference/beta/api/contact_delta.md)関数 |
| ユーザー | [ユーザー](../api-reference/beta/resources/user.md)リソースの[デルタ](../api-reference/beta/api/user_delta.md)関数 | 
| ドライブの項目\* | [driveItem](../api-reference/beta/resources/driveItem.md) リソースの[デルタ](../api-reference/beta/api/item_delta.md)関数 |


> \* v1.0 では、ドライブとその子への変更の追跡が既にサポートされています。使用パターンは、他のサポートされているリソースと似ていますが、構文には若干の違いがあります。ドライブのデルタ クエリは、他のリソースの種類との一貫性を保つために将来更新されます。現在の構文の詳細については、<https://developer.microsoft.com/ja-jp/graph/docs/api-reference/v1.0/api/item_delta> を参照してください。

## <a name="prerequisites"></a>前提条件

特定のリソースを読み取るために必要な[アクセス許可](../authorization/permission_scopes.md)と同じアクセス許可も、そのリソースでデルタ クエリを実行するために必要です。

## <a name="known-limitations"></a>既知の制限

デルタ クエリの使用に関する既知の制限については、既知の問題に関する記事の[「デルタ クエリ」セクション](../overview/release_notes.md#delta-query)を参照してください。

## <a name="delta-query-request-examples"></a>デルタ クエリ要求の例 

- [カレンダー ビューのイベントへの増分の変更を取得する (プレビュー)](../Concepts/delta_query_events.md)
- [フォルダー内のメッセージへの増分の変更を取得する (プレビュー)](./delta_query_messages.md)
- [グループへの増分の変更を取得する (プレビュー)](./delta_query_groups.md)
- [ユーザーへの増分の変更を取得する (プレビュー)](./delta_query_users.md)