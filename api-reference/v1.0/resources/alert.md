---
title: alert リソースの種類
description: Microsoft またはパートナーのセキュリティ ソリューションが識別した、お客様のテナント内における潜在的なセキュリティ問題を表します。 警告を使用して、統合ソリューション全体のセキュリティ問題管理を統合し、合理化してください。 詳細については、Graph エクスプローラーのサンプル クエリを参照してください。
localization_priority: Priority
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 7248fb61f62c9b17d639a5e7e2c3d8b4b2e92719
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033231"
---
# <a name="alert-resource-type"></a>alert リソースの種類

Microsoft またはパートナーのセキュリティ ソリューションが識別した、お客様のテナント内における潜在的なセキュリティ問題を表します。 警告を使用して、統合ソリューション全体のセキュリティ問題管理を統合し、合理化してください。 詳細については、[Graph エクスプローラー](https://developer.microsoft.com/graph/graph-explorer)のサンプル クエリを参照してください。

警告は、「[Microsoft Graph セキュリティの概要](security-api-overview.md)」に記載されているさまざまなセキュリティ プロバイダーから取得できます。

## <a name="methods"></a>メソッド

| メソッド   | 戻り値の型|説明|
|:---------------|:--------|:----------|
|[警告の取得](../api/alert-get.md) | [alert](alert.md) |警告オブジェクトのプロパティとリレーションシップを読み取ります。|
|[警告の更新](../api/alert-update.md) | [alert](alert.md) |警告オブジェクトを更新します。 |
|[警告の一覧表示](../api/alert-list.md) | [alert](alert.md) コレクション |警告オブジェクトのコレクションを取得します。|

## <a name="properties"></a>プロパティ

| プロパティ   | 型|説明|
|:---------------|:--------|:----------|
|activityGroupName|String|この警告に起因するアクティビティ グループ (攻撃者) の名前またはエイリアス。|
|assignedTo|String|トリアージ、調査、修復のために警告が割り当てられているアナリストの名前です ([更新](../api/alert-update.md)をサポートしています)。|
|azureSubscriptionId|String|Azure サブスクリプション ID (この警告が Azure リソースに関連している場合に提示されます)。|
|azureTenantId |String|Azure Active Directory テナント ID。 必須です。|
|category|String|警告のカテゴリ (たとえば、credentialTheft、ransomware など)。|
|closedDateTime|DateTimeOffset|警告が閉じられた時刻。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、`'2014-01-01T00:00:00Z'` のようになります ([更新](../api/alert-update.md)をサポートしています)。|
|cloudAppStates|[cloudAppSecurityState](cloudappsecuritystate.md) コレクション|この警告に関連するクラウド アプリケーションについて、プロバイダーによって生成されるセキュリティ関連のステートフル情報。|
|comments|String コレクション|警告に対する顧客提供のコメント (顧客警告管理の場合) ([更新](../api/alert-update.md)をサポートしています)。|
|confidence|Int32|検出ロジックの信頼性 (1 ～ 100 のパーセンテージ値)。|
|createdDateTime |DateTimeOffset|警告が警告プロバイダーによって作成された時刻。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'` 必須です。|
|説明|String|警告の説明。|
|detectionIds|String コレクション|この警告エンティティに関連する警告のセット (各警告は個別のレコードとして SIEM にプッシュされます)。|
|eventDateTime |DateTimeOffset|警告を生成するトリガーとして処理されるイベントの発生時刻。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'` 必須です。|
|feedback|alertFeedback|警告に関するアナリストのフィードバック。 使用可能な値は、`unknown`、`truePositive`、`falsePositive`、`benignPositive` です。 ([更新](../api/alert-update.md)をサポートしています)|
|fileStates|[fileSecurityState](filesecuritystate.md) コレクション|この警告に関連するファイルについて、プロバイダーによって生成されるセキュリティ関連のステートフル情報。|
|hostStates|[hostSecurityState](hostsecuritystate.md) コレクション|この警告に関連するホストについて、プロバイダーによって生成されるセキュリティ関連のステートフル情報。|
|id |String|プロバイダーによって生成された GUID/一意の識別子。 読み取り専用です。 必須です。|
|lastModifiedDateTime|DateTimeOffset|警告エンティティが最後に変更された時刻。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|malwareStates|[malwareState](malwarestate.md) コレクション|この警告に関連したマルウェアについての脅威インテリジェンス。|
|networkConnections|[networkConnection](networkconnection.md) コレクション|この警告に関連するネットワーク接続について、プロバイダーによって生成されるセキュリティ関連のステートフル情報。|
|processes|[process](process.md) コレクション|この警告に関連するプロセスについて、プロバイダーによって生成されるセキュリティ関連のステートフル情報。|
|recommendedActions|String コレクション|警告の結果として実行する仕入先/プロバイダー推奨アクション (たとえば、マシンの分離、enforce2FA、再イメージ化ホスト)。|
|registryKeyStates|[registryKeyState](registrykeystate.md) コレクション|この警告に関連するレジストリ キーについて、プロバイダーによって生成されるセキュリティ関連のステートフル情報。|
|severity |alertSeverity|警告の重要度 - 仕入先/プロバイダーが設定します。 可能な値は、`unknown`、`informational`、`low`、`medium`、`high` です。 必須です。|
|sourceMaterials|String コレクション|警告に関連するソース マテリアルへのハイパーリンク (URI)、たとえば、プロバイダーの警告やログ検索のためのユーザー インターフェイスなど。|
|status |alertStatus|警告のライフサイクル ステータス (ステージ)。 使用可能な値は、`unknown`、`newAlert`、`inProgress`、`resolved` です。 ([更新](../api/alert-update.md)をサポートしています)。 必須です。|
|タグ|String collection|警告に適用でき、フィルター条件として使用できるユーザー定義可能なラベル (例 "HVA"、"SAW" など) ([更新](../api/alert-update.md)をサポートしています)。|
|title |String|警告タイトル。 必須です。|
|triggers|[alertTrigger](alerttrigger.md) コレクション|警告をトリガーした特定のプロパティ (警告に表示されるプロパティ) に関するセキュリティ関連の情報。 警告には、複数のユーザー、ホスト、ファイル、IP アドレスに関する情報が含まれる場合があります。 このフィールドは、警告の生成をトリガーしたプロパティを示します。|
|userStates|[userSecurityState](usersecuritystate.md) コレクション|この警告に関連するユーザー アカウントについて、プロバイダーによって生成されるセキュリティ関連のステートフル情報。|
|vendorInformation |[securityVendorInformation](securityvendorinformation.md)|セキュリティ製品/サービスの仕入先、プロバイダー、サブプロバイダーに関する詳細を含む複合型 (たとえば、仕入先 = Microsoft、プロバイダー = Windows Defender ATP、サブプロバイダー = AppLocker)。 必須です。|
|vulnerabilityStates|[vulnerabilityState](vulnerabilitystate.md) コレクション|この警告に関連した 1 つかそれ以上の脆弱性についての脅威インテリジェンス。|

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
