    ---
title: "educationIdentitySynchronizationConfiguration resource type" description: "すべての学校データプロファイル id 同期構成の抽象基本クラス。 派生クラスは、id を同期するための動作を定義します。 派生型の例を次に示します。
著者: "mmast-msft" 送受信: 通常の ms 製品: "教育"
---

# <a name="educationidentitysynchronizationconfiguration-resource-type"></a>educationIdentitySynchronizationConfiguration リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

すべての学校データプロファイル id 同期構成の抽象基本クラス。 派生クラスは、id を同期するための動作を定義します。 派生型を次に示します。

## <a name="derived-types"></a>派生型
| 型 | 説明 |
|:-|:-|
| [**educationIdentityMatchingConfiguration**](educationidentitymatchingconfiguration.md) | この種類を使用して、azure Active Directory (azure AD) の既存のユーザーアカウントと照合します。 |
| [**educationIdentityCreationConfiguration**](educationidentitycreationconfiguration.md) | この種類を使用して、Azure AD で新しいユーザーアカウントを作成します。 |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationidentitysynchronizationconfiguration.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
