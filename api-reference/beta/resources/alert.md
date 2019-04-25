---
title: alert リソースの種類
description: Microsoft またはパートナーのセキュリティソリューションが特定した、お客様のテナント内の潜在的なセキュリティ上の問題を表します。 アラートを使用して、すべての統合ソリューションにわたるセキュリティ問題の管理を統合および合理化します。 詳細については、「Graph Explorer のサンプルクエリ」を参照してください。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 8fa945cc69b3bc7779ae9ce23e2ee672c48eb1f8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535801"
---
# <a name="alert-resource-type"></a>alert リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft またはパートナーのセキュリティソリューションが特定した、お客様のテナント内の潜在的なセキュリティ上の問題を表します。 アラートを使用して、すべての統合ソリューションにわたるセキュリティ問題の管理を統合および合理化します。 詳細については、「 [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer)のサンプルクエリ」を参照してください。

通知は、 [「Microsoft Graph のセキュリティの概要](security-api-overview.md)」に記載されているさまざまなセキュリティプロバイダーから取得できます。

## <a name="methods"></a>メソッド

| メソッド   | 戻り値の型|説明|
|:---------------|:--------|:----------|
|[警告の取得](../api/alert-get.md) | [警告](alert.md) |alert オブジェクトのプロパティとリレーションシップを読み取ります。|
|[警告の更新](../api/alert-update.md) | [警告](alert.md) |通知オブジェクトを更新します。 |
|[警告の一覧表示](../api/alert-list.md) | [alert](alert.md)コレクション |通知オブジェクトのコレクションを取得します。|
|[アラートを更新する](../api/alert-updatealerts.md)|[alert](alert.md)コレクション|複数の alert オブジェクトを更新します。|

## <a name="properties"></a>プロパティ

| プロパティ   | 型|説明|
|:---------------|:--------|:----------|
|activitygroupname|String|この通知の対象となるアクティビティグループの名前またはエイリアス (攻撃者)。|
|assignedTo|String|アラートが割り当てられているアナリストの名前。トリアージ、調査、または修復 ([更新](../api/alert-update.md)をサポート)。|
|azuresubscriptionid|String|azure サブスクリプション ID。このアラートが azure リソースに関連している場合に表示されます。|
|azureTenantId |String|Azure Active Directory テナント ID。 必須です。 |
|category|文字列|アラートのカテゴリ (例: credentialtheft、ランサムウェアなど)。|
|closeddatetime|DateTimeOffset|通知が終了した時刻。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014年1月1日の午前0時は、次`'2014-01-01T00:00:00Z'`のように表示されます ([更新プログラム](../api/alert-update.md)をサポート)。|
|cloudappstates|[cloudappsecuritystate](cloudappsecuritystate.md)コレクション|このアラートに関連するクラウドアプリケーション/s に関する、プロバイダーによって生成されるセキュリティ関連のステートフル情報。|
|コメント|String collection|お客様からの警告に関するコメント (顧客の警告管理) ([更新プログラム](../api/alert-update.md)をサポート)。|
|confidence|Int32|検出ロジックの信頼性 (1-100 間の割合)。|
|createdDateTime |DateTimeOffset|通知プロバイダによって通知が作成された時刻。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'` 必須です。|
|description|String|通知の説明。|
|detectionIds|String collection|このアラートエンティティに関連する警告のセット (各警告は、別のレコードとして SIEM にプッシュされます)。|
|eventDateTime |DateTimeOffset|トリガーとして処理されたイベントが発生した時点でアラートが発生した時刻。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'` 必須です。|
|feedback|alertFeedback|アラートに関するアナリストのフィードバック。 可能な値は、`unknown`、`truePositive`、`falsePositive`、`benignPositive` です。 ([更新プログラム](../api/alert-update.md)のサポート)|
|fileStates|[fileSecurityState](filesecuritystate.md)コレクション|このアラートに関連するファイルに関する、プロバイダーによって生成されるセキュリティ関連のステートフル情報。|
|履歴の状態|[alertHistoryState](alerthistorystate.md)コレクション| **alertHistoryStates**のコレクション。通知に対して行われたすべての更新の監査ログを構成します。 |
|hoststates|[hostsecuritystate](hostsecuritystate.md)コレクション|このアラートに関連するホストに関する、プロバイダーによって生成されるセキュリティ関連のステートフル情報。|
|id |String|プロバイダー生成の GUID/一意識別子。 読み取り専用。 必須です。|
|lastModifiedDateTime|DateTimeOffset|通知エンティティが最後に変更された時刻。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|malwareStates|[malwareState](malwarestate.md)コレクション|このアラートに関連するマルウェアに関する脅威インテリジェンス。|
|networkconnections|[networkConnection](networkconnection.md)コレクション|このアラートに関連するネットワーク接続に関する、プロバイダーによって生成されるセキュリティ関連のステートフル情報。|
|工程|[プロセス](process.md)コレクション|このアラートに関連するプロセスまたはプロセスに関する、プロバイダーによって生成されるセキュリティ関連のステートフル情報。|
|recommendedActions|String collection|通知の結果として実行されるベンダー/プロバイダー推奨アクション (たとえば、enforce2FA、再イメージ化されたホスト)。|
|registrykeystates|[registrykeystate](registrykeystate.md)コレクション|このアラートに関連するレジストリキーに関する、プロバイダーによって生成されるセキュリティ関連のステートフル情報。|
|重大度 |alertSeverity|アラート重大度-ベンダー/プロバイダーによって設定されます。 可能な値は、`unknown`、`informational`、`low`、`medium`、`high` です。 必須です。|
|sourceMaterials|String collection|アラートに関連するソース素材へのハイパーリンク (uri)。たとえば、通知やログ検索用のプロバイダーのユーザーインターフェイスなど。|
|status |alertStatus|アラートのライフサイクル状態 (ステージ)。 可能な値は、`unknown`、`newAlert`、`inProgress`、`resolved` です。 ([更新プログラム](../api/alert-update.md)をサポート)。 必須です。|
|tags|String コレクション|通知に適用することができ、フィルター条件として機能することができる、ユーザー定義のラベル (たとえば、"hva"、"のこぎり" など)。([更新プログラム](../api/alert-update.md)をサポート)。|
|title |String|通知のタイトル。 必須です。|
|ログオフ|[alerttrigger](alerttrigger.md)コレクション|アラートをトリガーした特定のプロパティに関するセキュリティ関連の情報 (アラートに表示されるプロパティ)。 通知には、複数のユーザー、ホスト、ファイル、ip アドレスに関する情報が含まれることがあります。 このフィールドは、アラート生成をトリガーしたプロパティを示します。|
|userstates|[usersecuritystate](usersecuritystate.md)コレクション|この通知に関連するユーザーアカウントに関する、プロバイダーによって生成されるセキュリティ関連のステートフル情報。|
|vendorInformation |[securityVendorInformation](securityvendorinformation.md)|セキュリティ製品/サービスのベンダー、プロバイダ、およびサブプロバイダに関する詳細を含む複合型 (たとえば、vendor = Microsoft; provider = Windows Defender ATP; subprovider = AppLocker)。 必須です。|
|vulnerabilityStates|[vulnerabilityState](vulnerabilitystate.md)コレクション|このアラートに関連する1つまたは複数の脆弱性に関する脅威インテリジェンス。|

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
  "historyStates": [{"@odata.type": "microsoft.graph.alertHistoryState"}],
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
<!--
{
  "type": "#page.annotation",
  "description": "alert resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/alert.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
