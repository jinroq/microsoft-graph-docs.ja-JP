---
title: secureScores リソースの種類
description: '上部 = n、n = のデータを取得する日数です。 '
localization_priority: Normal
ms.openlocfilehash: fef5c43130aecf1604677d07f785a0cee0539568
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576081"
---
# <a name="securescores-resource-type"></a>secureScores リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

テナントとコントロール レベルでのデータのスコアの 1 日あたりのテナントのセキュリティで保護されたスコアを表します。 既定では、90 日間のデータを保持しています。 このデータの並べ替えに**createdDateTime**から最初に最新です。 これにより、ページの応答に $top を使用して = n、n = のデータを取得する日数です。 


## <a name="methods"></a>メソッド

| メソッド   | 戻り値の型|説明|
|:---------------|:--------|:----------|
|[secureScores のリスト](../api/securescores-list.md) | [secureScores](securescores.md) |プロパティと、secureScores オブジェクトのメタデータを参照してください。|


## <a name="properties"></a>プロパティ
テナントのセキュリティのエンティティの型を含むプロパティ (日単位のスナップショット データ) のスコアです。

|プロパティ |型 |説明 |
|:--|:--|:--|
|   azureTenantId   |   String  |   テナントの GUID の文字列 id。  |
|   createdDateTime |   DateTimeOffset  |   エンティティが作成されたときの日付。  |
|   id  |   String  |   AzureTenantId_createdDateTime の組み合わせです。   |
|   licensedUserCount   |   Int32   |   特定のテナントのユーザー数のライセンスを取得します。    |
|   activeUserCount |   Int32   |   特定のテナントのアクティブなユーザー数です。  |
|   currentScore    |   倍精度浮動小数点数  |   現在のテナントは、指定した日付のスコアを達成します。    |
|   maxScore |  倍精度浮動小数点数  |   有効最大スコアを指定した日付のテナントです。    |
|   enabledServices |   String コレクション   |   (たとえば、Exchange のオンライン、Skype、Sharepoint) テナントの Microsoft 提供のサービスです。   |
|   averageComparativeScores |  [averageComparativeScore](averagecomparativescore.md)コレクション    |さまざまなスコープ (業界では、座席で平均での平均値など) およびコントロールの分類 (識別情報、データ、デバイス、アプリケーション、インフラストラクチャ) のスコープ内での平均スコアです。 |
|   controlScores | [controlScore](controlscore.md)コレクション  |   コントロールのセットのテナントのスコアが含まれています。   |
|   vendorInformation | [securityVendorInformation](securityvendorinformation.md) | セキュリティ製品やサービスの仕入先、プロバイダー、および subprovider の詳細が含まれています (たとえば、ベンダー = Microsoft; プロバイダー = Windows Defender の分析ツールです。 subProvider AppLocker を =)。|

## <a name="relationships"></a>リレーションシップ

なし。

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.secureScore"
}-->

```json
{
    "id": "String",
    "azureTenantId": "String (identifier)",
    "createdDateTime": "DateTimeOffset",
    "licensedUserCount": "Int32",
    "activeUserCount": "Int32",
    "currentScore": "Double",
    "maxScore": "Double",    
    "enabledServices": ["String"],
    "averageComparativeScores": [{ "@odata.type":"microsoft.graph.averageComparativeScores"}],
    "controlScores": [{"@odata.type":"microsoft.graph.controlScores"}],
    "vendorInformation" : "microsoft.graph.securityVendorInformation"
}
```


<!--
{
  "type": "#page.annotation",
  "description": "secureScores resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/securescores.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
