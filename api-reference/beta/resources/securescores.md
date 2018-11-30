---
title: secureScores リソースの種類
description: '上部 = n、n = のデータを取得する日数です。 '
ms.openlocfilehash: 96d5c487bb854559b0128d93ea8e0783fcc61f0c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067316"
---
# <a name="securescores-resource-type"></a>secureScores リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

テナントとコントロール レベルでのデータのスコアの 1 日あたりのテナントのセキュリティで保護されたスコアを表します。 既定では、90 日間のデータを保持しています。 このデータの並べ替えに**createdDateTime**から最初に最新です。 これにより、ページの応答に $top を使用して = n、n = のデータを取得する日数です。 


## <a name="methods"></a>メソッド

| メソッド   | 戻り値の型|説明|
|:---------------|:--------|:----------|
|[リスト secureScores](../api/securescores-list.md) | [secureScores](securescores.md) |プロパティと、secureScores オブジェクトのメタデータを参照してください。|


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


## <a name="relationships"></a>リレーションシップ

なし。

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.secureScores"
}-->

```json
{
"id": "String",
"azureTenantId": "Guid",
"createdDate": "DateTimeOffset",
"licensedUserCount": "Int32",
"activeUserCount": "Int32",
"currentScore": "Int32",
"maxScore": "Int32",
"averageScore": "Double",
"enabledServices": "Collection(string)",
"averageComparativeScores": "Collection(microsoft.graph.SecureScore.averageComparativeScores)",
"controlScores": "Collection(microsoft.graph.SecureScore.controlScores)",
}

```


<!-- {
  "type": "#page.annotation",
  "description": "secureScores resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
