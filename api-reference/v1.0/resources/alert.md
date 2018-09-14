# <a name="alert-resource-type"></a>警告リソースの種類

マイクロソフトまたはパートナーのセキュリティ ソリューションが特定されるを顧客のテナント内の潜在的なセキュリティ問題を表します。 すべての統合されたソリューションのセキュリティ問題の管理を統一し、合理化するには、警告を使用します。 詳細については、 [グラフのエクスプ ローラー](https://developer.microsoft.com/en-us/graph/graph-explorer)内のサンプル クエリを参照してください。

警告は、次のプロバイダーから取得できます: Azure のセキュリティ センター、Azure アクティブ ディレクトリ アイデンティティ 保護。 その他の警告 プロバイダーは、次の月の間に統合されます。

## <a name="methods"></a>メソッド

| メソッド   | 戻り値の型|説明|
|:---------------|:--------|:----------|
|[警告の取得](../api/alert_get.md) | [警告](alert.md) |警告オブジェクトのプロパティと関係を参照してください。|
|[警告の更新](../api/alert_update.md) | [警告](alert.md) |警告オブジェクトを更新します。 |
|[警告の一覧表示](../api/alert_list.md) | [警告](alert.md) のコレクション |警告オブジェクトのコレクションを取得します。|

## <a name="properties"></a>プロパティ

| プロパティ   | 型|説明|
|:---------------|:--------|:----------|
|activityGroupName|文字列|この警告が属するアクティビティ グループ (攻撃者) の名前またはエイリアス。|
|assignedTo|文字列|警告が、選別、調査、または改善 ( [更新](../api/alert_update.md)がサポートされています) のために割り当てられているアナリストの名前。|
|azureSubscriptionId|文字列|Azure サブスクリプション IDは、アラートがAzure のリソースに関連している場合に存在します。|
|azureTenantId *|文字列|Azure アクティビティ ディレクトリ のテナント ID。|
|カテゴリー|文字列|(たとえば、credentialTheft、ransomware など) の警告のカテゴリです。|
|closedDateTime|DateTimeOffset|警告が終了した時間。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 例えば2014 年 1 月 1 日UTC 午前 0 時は、このようになります: `'2014-01-01T00:00:00Z'` ( [更新](../api/alert_update.md)がサポートされています)。|
|cloudAppStates|[cloudAppSecurityState](cloudappsecuritystate.md) コレクション|セキュリティに関連するステートフルな情報については、このアラートに関連するクラウド アプリケーションのプロバイダーによって生成されます。|
|コメント|文字列コレクション|警告 (警告管理の顧客) のお客様提供のコメント ( 更新がサポートされています)。[ ](../api/alert_update.md)|
|信認|Int32|検出ロジック (1 から 100のパーセンテージ) を信頼します。|
|createdDateTime|DateTimeOffset|警告が警告プロバイダーによって作成された時点の時間です。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|説明|文字列|アラートの説明です。|
|detectionIds|文字列コレクション| この警告のエンティティに関連する警告を設定します(各アラートは、個別のレコードとして SIEM にプッシュされます)。|
|eventDateTime|DateTimeOffset|アラートを生成するトリガーとして処理されるイベントが発生した時刻です。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|フィードバック|alertFeedback|警告に関するアナリストのフィードバックです。 可能な値は、`unknown`、`truePositive`、`falsePositive`、`benignPositive` です。 ( [更新](../api/alert_update.md)がサポートされています)|
|fileStates|[fileSecurityState](filesecuritystate.md) コレクション|セキュリティに関連するステートフルな情報については、この警告に関連するファイルのプロバイダーによって生成されます。|
|hostStates|[hostSecurityState](hostsecuritystate.md) コレクション|セキュリティに関連するステートフルな情報については、この警告に関連するホスト プロバイダーによって生成されます。|
|ID *|文字列|プロバイダーによって生成された GUID または一意の識別子。 (読み取り専用)|
|lastModifiedDateTime|DateTimeOffset|警告のエンティティが最後に修正された時間です。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|malwareStates|[malwareState](malwarestate.md) コレクション|この警告に関連するマルウェアに関する脅威インテリジェンスです。|
|networkConnections|[ネットワーク接続](networkconnection.md) のコレクション|セキュリティに関連するステートフルな情報については、この警告に関連するホスト プロバイダーによって生成されます。|
|プロセス|[プロセス](process.md) のコレクション|セキュリティに関連するステートフルな情報については、この警告に関連するプロセスのプロバイダーによって生成されます。|
|recommendedActions|文字列コレクション|ベンダー/プロバイダーには、警告の結果として実行するアクションをお勧めします(たとえば、特定のコンピューター、enforce2FA、ホストのイメージを再作成) 。|
|registryKeyStates|[registryKeyState](registrykeystate.md) コレクション|セキュリティに関連するステートフルな情報については、この警告に関連するホスト プロバイダーによって生成されます。|
|深刻度|alertSeverity|警告の深刻度－ベンダーまたはプロバイダーが設定します。 可能な値は、`unknown`、`informational`、`low`、`medium`、`high` です。|
|sourceMaterials|文字列コレクション|警告に関連するソース マテリアルへのハイパーリンク (URL)、例えばプロバイダーの警告用のユーザー インターフェイスまたはログ検索など。|
|状態*|alertStatus|アラートのライフ サイクル ステータス (ステージ)。 可能な値は、`unknown`、`newAlert`、`inProgress`、`resolved` です。 ( [更新](../api/alert_update.md)がサポートされています)|
|タグ|文字列コレクション|警告に適用でき、フィルター条件 ("HVA"、"SAW" など) として機能できるユーザーが定義可能なラベル( [更新](../api/alert_update.md)がサポートされています)。|
|タイトル*|文字列|警告タイトル。|
|トリガー|[alertTrigger](alerttrigger.md) コレクション|警告 (アラートに表示されるプロパティ) をトリガーする特定のプロパティについてのセキュリティに関連する情報です。 警告には、複数のユーザー、ホスト、ファイル、IP アドレスに関する情報が含まれます。 このフィールドは、どのプロパティが警告の生成をトリガーするかを示します。|
|userStates|[userSecurityState](usersecuritystate.md) コレクション|セキュリティに関連するステートフルな情報については、この警告に関連するホスト プロバイダーによって生成されます。|
|vendorInformation *|[securityVendorInformation](securityvendorinformation.md)|セキュリティ製品、またはサービスの仕入先、サービス プロバイダー、およびサービス サブプロバイダーの詳細を含む複合型 (仕入先 = Microsoft、プロバイダー = Windows Defender ATP、サブプロバイダー = AppLocker など)。|
|vulnerabilityStates|[vulnerabilityState](vulnerabilitystate.md) コレクション|この警告に関連する 1 つまたは複数の脆弱性に関連する脅威インテリジェンスです。|
(\* は、必須フィールドを表します)。

## <a name="relationships"></a>関係

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