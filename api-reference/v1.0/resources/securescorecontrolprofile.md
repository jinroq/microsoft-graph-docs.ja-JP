---
title: secureScoreControlProfile リソースの種類
description: テナントのセキュリティスコア (コントロールデータごと) を表します。 既定では、テナントのすべてのコントロールを返し、個々のコントロールを明示的に取得することができます。
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 40bee951d3030772973911510ebba7cc90f412ae
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034490"
---
# <a name="securescorecontrolprofile-resource-type"></a>secureScoreControlProfile リソースの種類

テナントのセキュリティスコア (コントロールデータごと) を表します。 既定では、テナントのすべてのコントロールを返し、個々のコントロールを明示的に取得することができます。


## <a name="methods"></a>メソッド

| メソッド   | 戻り値の型|説明|
|:---------------|:--------|:----------|
|[secureScoreControlProfiles のリスト](../api/security-list-securescorecontrolprofiles.md) | [secureScoreControlProfile](securescorecontrolprofile.md) |Securescorecontrolprofiles のオブジェクトのプロパティとメタデータを読み取ります。|
|[secureScoreControlProfile の取得](../api/securescorecontrolprofile-get.md) | [securescorecontrolprofile](securescorecontrolprofile.md) |Securescorecontrolprofiles のオブジェクトのプロパティとメタデータを読み取ります。|
|[Securescorecontrolprofile の更新](../api/securescorecontrolprofile-update.md) | [securescorecontrolprofile](securescorecontrolprofile.md) |Securescorecontrolprofile オブジェクトを更新します。 |


## <a name="properties"></a>プロパティ

|名前 |型 |説明 |
|:--|:--|:--|
|id|String|プロバイダーによって生成された GUID/一意の識別子。 読み取り専用です。 必須です。|
|azureTenantId|String|テナント ID の GUID 文字列。|
|actionType|String|アクションの種類 (Config、Review、Behavior) を制御します。|
|actionUrl|String|コントロールを actioned できる場所の URL。 |
|controlCategory|String|コントロールアクションカテゴリ (Id、データ、デバイス、アプリ、インフラストラクチャ)。|
|title|String|コントロールのタイトルを指定します。|
|予定|Boolean|コントロールが減価償却されているかどうかを示すフラグです。|
|implementationCost|String|Implemmentating コントロールのリソースコスト (低、中、高)。|
|lastModifiedDateTime|DateTimeOffset|コントロールプロファイルエンティティが最後に変更された時刻。 タイムスタンプの種類は、日付と時刻を表します。| 
|maxScore|2 行分|コントロールの最大達成数スコア。|
|rank|Int32|Microsoft のスタックランキング。|
|修復|String|修復に役立つコントロールの説明。|
|remediationImpact|String|修復のユーザーへの影響についての説明。|
|service|String|コントロールを所有するサービス (Exchange、Sharepoint、Azure AD)。|
|主|文字列コレクション|統制によって軽減される脅威のリスト (accountBreach、dataDeletion、Dataexフィルター、、
elevationOfPrivilege、maliciousInsider、passwordCracking、phishingOrWhaling、スプーフィング)。|
|層|String|Control 層 (コア、多層防御、詳細)   |
|userImpact|String|制御を実装するユーザーへの影響 (低、中、高)。   |
|complianceInformation|[complianceInformation](complianceinformation.md)コレクション|セキュリティで保護されたスコアコントロールに関連付けられているコンプライアンス情報のコレクション|
|controlStateUpdates|[secureScoreControlStateUpdate](securescorecontrolstateupdate.md)コレクション|テナントがコントロールをマークした場所を示すフラグ (無視、thirdParty、レビュー済み) ([更新プログラム](../api/securescorecontrolprofile-update.md)をサポート)。|
|vendorInformation|[securityVendorInformation](securityvendorinformation.md)|セキュリティ製品/サービスベンダー、プロバイダー、およびサブプロバイダに関する詳細を含む複合型 (たとえば、vendor = Microsoft; provider = SecureScore)。 必須です。|

## <a name="relationships"></a>リレーションシップ

なし。

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.secureScoreControlProfile"
}-->

```json
{
  "id": "String (identifier)",
  "azureTenantId": "String",
  "actionType": "String",
  "actionUrl": "String",
  "controlCategory": "String",
  "title": "String", 
  "deprecated": "Boolean",
  "implementationCost": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "maxScore": "Double",
  "rank": "Int32",
  "remediation": "String",
  "remediationImpact": "String",
  "service": "String",
  "threats": ["String"],
  "tier": "String",
  "userImpact": "String",
  "complianceInformation": [{"@odata.type": "microsoft.graph.complianceInformation"}], 
  "controlStateUpdates": [{"@odata.type": "microsoft.graph.secureScoreControlStateUpdate"}],
  "vendorInformation": {"@odata.type": "microsoft.graph.securityVendorInformation"},
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "secureScoreControlProfiles resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
