# <a name="alert-resource-type"></a>通知リソースの種類

マイクロソフトまたはパートナーのセキュリティ ・ ソリューションを特定の顧客のテナント内の潜在的なセキュリティ問題を表します。 統一し、すべての統合されたソリューションのセキュリティ問題の管理を合理化するには、アラートを使用します。 詳細については、[グラフのエクスプ ローラー](https://developer.microsoft.com/graph/graph-explorer)内のサンプル クエリを参照してください。

警告は、 [Microsoft のグラフのセキュリティの概要」](security-api-overview.md)に記載されている別のセキュリティ プロバイダーから取得できます。

## <a name="methods"></a>メソッド

| メソッド   | 戻り値の型|説明|
|:---------------|:--------|:----------|
|[警告の取得](../api/alert_get.md) | [アラート](alert.md) |Alert オブジェクトのプロパティと関係を参照してください。|
|[警告の更新](../api/alert_update.md) | [アラート](alert.md) |Alert オブジェクトを更新します。 |
|[警告の一覧表示](../api/alert_list.md) | [アラート](alert.md)のコレクション |Alert オブジェクトのコレクションを取得します。|

## <a name="properties"></a>プロパティ

| プロパティ   | 型|説明|
|:---------------|:--------|:----------|
|activityGroupName|文字列|アクティビティ グループ (攻撃者) の名前またはエイリアスにこのアラートが属する。|
|担当者|文字列|アナリスト、警告の名前は、選別、調査、または ([更新](../api/alert_update.md)がサポートされています) の改善のために割り当てられます。|
|azureSubscriptionId|文字列|Azure サブスクリプション ID、このアラートは、Azure のリソースに関連している場合に存在します。|
|azureTenantId |文字列|Azure Active Directory のテナント id。 必須。|
|category|文字列|(たとえば、credentialTheft、ransomware など) の警告のカテゴリです。|
|closedDateTime|DateTimeOffset|時間のアラートが閉じられました。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 2014 年 1 月 1 日に UTC 午前 0 時、これのようになります: `'2014-01-01T00:00:00Z'` ([更新](../api/alert_update.md)がサポートされています)。|
|cloudAppStates|[cloudAppSecurityState](cloudappsecuritystate.md)コレクション|セキュリティに関連するステートフルな情報については、このアラートに関連するクラウド アプリケーション/秒のプロバイダーによって生成されます。|
|comments|String コレクション|アラート (アラート管理の顧客) のお客様提供のコメント ([更新](../api/alert_update.md)がサポートされています)。|
|confidence|Int32|検出ロジック (1 ~ 100%) を信頼します。|
|createdDateTime |DateTimeOffset|アラートが通知プロバイダーによって作成された時点の時間です。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'` 必須。|
|説明|文字列|アラートの説明です。|
|detectionIds|String コレクション|(各アラートは、個別のレコードとして SIEM にプッシュされます) この警告のエンティティに関連するアラートのセットです。|
|eventDateTime |DateTimeOffset|アラートを生成するトリガーとして処理されるイベントが発生した時刻です。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'` 必須。|
|feedback|alertFeedback|アナリストのフィードバック通知をします。 可能な値は、`unknown`、`truePositive`、`falsePositive`、`benignPositive` です。 ([更新](../api/alert_update.md)がサポートされています)|
|fileStates|[fileSecurityState](filesecuritystate.md)コレクション|セキュリティに関連するステートフルな情報については、このアラートに関連するファイルのプロバイダーによって生成されます。|
|hostStates|[hostSecurityState](hostsecuritystate.md)コレクション|セキュリティに関連するステートフルな情報については、このアラートに関連するホスト プロバイダーによって生成されます。|
|id |文字列|プロバイダーによって生成された GUID または一意の識別子。 読み取り専用です。 必須。|
|lastModifiedDateTime|DateTimeOffset|アラートのエンティティが最後に修正された時間です。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|malwareStates|[malwareState](malwarestate.md)コレクション|このアラートに関連するマルウェアに関連する脅威インテリジェンスです。|
|networkConnections|[ネットワーク接続](networkconnection.md)のコレクション|セキュリティに関連するステートフルな情報については、このアラートに関連するネットワーク接続のプロバイダーによって生成されます。|
|プロセス|[プロセス](process.md)のコレクション|セキュリティに関連するステートフルな情報については、このアラートに関連するプロセスのプロバイダーによって生成されます。|
|recommendedActions|String コレクション|仕入先/プロバイダーは、(たとえば、特定のコンピューター、enforce2FA、ホストのイメージを再作成) は、アラートの結果として実行するアクションをお勧めします。|
|registryKeyStates|[registryKeyState](registrykeystate.md)コレクション|レジストリ キーのプロバイダーによって生成されるセキュリティ関連のステートフルな情報は、このアラートに関連しています。|
|重大度レベル |alertSeverity|アラートの重大度のベンダーまたはプロバイダーが設定します。 可能な値は、`unknown`、`informational`、`low`、`medium`、`high` です。 必須。|
|sourceMaterials|String コレクション|ソース マテリアルへのハイパーリンク (Uri) に関連する警告などの通知またはログの検索などのユーザー インターフェイスをプロバイダーの。|
|status |alertStatus|アラートのライフ サイクルのステータス (ステージ)。 可能な値は、`unknown`、`newAlert`、`inProgress`、`resolved` です。 ([更新](../api/alert_update.md)をサポートしています)。 必須。|
|タグの前に追加されるマークアップ|String コレクション|アラートに適用することができますし、(たとえば"HVA"、"SAW"など) のフィルター条件として使用できるユーザー定義のラベル([更新](../api/alert_update.md)をサポートしています)。|
|タイトル |文字列|通知のタイトル。 必須。|
|トリガー|[alertTrigger](alerttrigger.md)コレクション|セキュリティに関連するアラート (アラートに表示されるプロパティ) をトリガーする特定のプロパティについての情報です。 アラートには、複数のユーザー、ホスト、ファイル、ip アドレスに関する情報が含まれます。 このフィールドは、プロパティ、アラートの生成をトリガーすることを示します。|
|userStates|[userSecurityState](usersecuritystate.md)コレクション|ユーザー アカウントのプロバイダーによって生成されるセキュリティ関連のステートフルな情報は、このアラートに関連しています。|
|vendorInformation |[securityVendorInformation](securityvendorinformation.md)|セキュリティ製品やサービスの仕入先、プロバイダー、および subprovider の詳細を含む複合型 (仕入先など = Microsoft; プロバイダー = Windows Defender の ATP は subProvider AppLocker を =)。 必須。|
|vulnerabilityStates|[vulnerabilityState](vulnerabilitystate.md)コレクション|このアラートに関連する 1 つまたは複数の脆弱性に関連する脅威インテリジェンスです。|

## <a name="relationships"></a>リレーションシップ

なし。

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.alert"
}-->

```json
{
  "activityGroupName": "String",
  "assignedTo": "String",
  "azureSubscriptionId": "String",
  "azureTenantId": "String",
  "category": "String",
  "closedDateTime": "String (timestamp)",
  "cloudAppStates": [{"@odata.type": "microsoft.graph.cloudAppSecurityState"}],
  "comments": ["String"],
  "confidence": 1024,
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "detectionIds": ["String"],
  "eventDateTime": "String (timestamp)",
  "feedback": "@odata.type: microsoft.graph.alertFeedback",
  "fileStates": [{"@odata.type": "microsoft.graph.fileSecurityState"}],
  "hostStates": [{"@odata.type": "microsoft.graph.hostSecurityState"}],
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "malwareStates": [{"@odata.type": "microsoft.graph.malwareState"}],
  "networkConnections": [{"@odata.type": "microsoft.graph.networkConnection"}],
  "processes": [{"@odata.type": "microsoft.graph.process"}],
  "recommendedActions": ["String"],
  "registryKeyStates": [{"@odata.type": "microsoft.graph.registryKeyState"}],
  "severity": "@odata.type: microsoft.graph.alertSeverity",
  "sourceMaterials": ["String"],
  "status": "@odata.type: microsoft.graph.alertStatus",
  "tags": ["String"],
  "title": "String",
  "triggers": [{"@odata.type": "microsoft.graph.alertTrigger"}],
  "userStates": [{"@odata.type": "microsoft.graph.userSecurityState"}],
  "vendorInformation": {"@odata.type": "microsoft.graph.securityVendorInformation"},
  "vulnerabilityStates": [{"@odata.type": "microsoft.graph.vulnerabilityState"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "alert resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->