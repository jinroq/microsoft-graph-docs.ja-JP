---
title: secureScoreControlProfiles リソースの種類
description: コントロールのデータごとのテナントのセキュリティで保護されたスコアを表します。 既定では、テナントのすべてのコントロールを返し、個々 のコントロールを明示的に取得できます。
localization_priority: Normal
ms.openlocfilehash: 4e599bbffd291de51ba478f8661999d01c8c8998
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576060"
---
# <a name="securescorecontrolprofiles-resource-type"></a>secureScoreControlProfiles リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

コントロールのデータごとのテナントのセキュリティで保護されたスコアを表します。 既定では、テナントのすべてのコントロールを返し、個々 のコントロールを明示的に取得できます。


## <a name="methods"></a>メソッド

| メソッド   | 戻り値の型|説明|
|:---------------|:--------|:----------|
|[secureScoreControlProfiles のリスト](../api/securescorecontrolprofiles-list.md) | [secureScoreControlProfile](securescorecontrolprofiles.md) |プロパティと、secureScoreControlProfiles オブジェクトのメタデータを参照してください。|


## <a name="properties"></a>プロパティ

|名前 |型 |説明 |
|:--|:--|:--|
|   azureTenantId   |   String  |   テナントの GUID の文字列 id。  |
|   controlName |   String  |   コントロールの名前です。 |
|   タイトル   |   String  |   コントロールのタイトルです。   |
|   controlCategory |   String  |   コントロールのアクションのカテゴリ (アカウント、データ、デバイス、アプリケーション、インフラストラクチャ) です。  |
|   actionType  |   String  |   アクションの種類 (構成、レビュー、動作) を制御します。 |
|   service |   String  |   (Exchange、Sharepoint、Azure AD) のコントロールを所有しているサービスです。 |
|   maxScore |  倍精度浮動小数点数  |   現在では、指定した日付の最大のスコアを取得します。   |
|   層 |  String  |   制御層 (コア、防御の深さ、高度な)。    |
|   userImpact |    String  | コントロール (低、中、高) を実装するためのユーザーへの影響。    |
|   implementationCost |    String  |   Implemmentating コントロール (低、中、高) のリソースのコストです。 |
|   rank |  Int32   |   マイクロソフトのコントロールのレベルを調整します。   |
|   脅威 |   文字列コレクション   |   コントロールを軽減する脅威の一覧 (accountBreach、dataDeletion、dataExfiltration、dataSpillage、elevationOfPrivilege、maliciousInsider、passwordCracking、phishingOrWhaling、なりすましが行われる)。 |
|   非推奨 |    Boolean |   コントロールで減価償却されるかどうかを示すためにフラグを設定します。   |
|   改善計画 |   String  |   どのようなコントロールの説明は、改善に役立ちます。 |
|   remediationImpact | String  |   改善のユーザーへの影響の説明です。 |
|   actionUrl | String  |   URL は、コントロールが対象になることです。 |
|   lastModifiedDateTime |  文字列 (DateTimeOffset) |   最終更新日 |
|   controlStateUpdates |   [secureScoreControlStateUpdate](securescorecontrolstateupdate.md)コレクション |  テナントには、コントロールとしてのマークを指定するフラグ (無視して、レビュー、サード ・ パーティ) ([更新](../api/securescorecontrolprofiles-update.md)がサポートされています)。 |
|   vendorInformation | [securityVendorInformation](securityvendorinformation.md) | セキュリティ製品やサービスの仕入先、プロバイダー、および subprovider の詳細が含まれています (たとえば、ベンダー = Microsoft; プロバイダー = Windows Defender の分析ツールです。 subProvider AppLocker を =)。|

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
    "title": "String", 
    "azureTenantId": "String (identifier)", 
    "referenceId": "String", 
    "controlName": "String", 
    "maxScore": "Double",
    "controlCategory": "string",
    "actionType": "string",
    "service": "String",
    "tier": "string",
    "userImpact": "string",
    "implementationCost ": "string",
    "rank ": "Int32",
    "deprecated ": "Boolean",
    "remediation": "String",
    "remediationImpact ": "String",
    "actionUrl": "String",
    "lastModifiedDateTime": "   String (DateTimeOffset)",
    "controlStateUpdates": [{"odata.type":"microsoft.graph.secureScorecontrolStateUpdates"}],
    "tenantNotes": "String",
    "upn": "String",    
    "vendorInformation" : "microsoft.graph.securityVendorInformation"
}


```


<!--
{
  "type": "#page.annotation",
  "description": "secureScoreControlProfiles resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/securescorecontrolprofiles.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
