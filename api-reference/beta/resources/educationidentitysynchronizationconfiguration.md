    ---
タイトル:「educationIdentitySynchronizationConfiguration のリソースの種類」の説明:「すべて学校データ プロファイル id の同期設定の基本クラスを抽象化します。 派生クラスは、識別情報を同期するための動作を定義します。 次の派生型」
作成者: mmast-溺"localization_priority: 通常の ms.prod:「教育」
---

# <a name="educationidentitysynchronizationconfiguration-resource-type"></a>educationIdentitySynchronizationConfiguration リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

すべて学校データ プロファイルの id の同期設定の抽象基本クラスです。 派生クラスは、識別情報を同期するための動作を定義します。 派生型を次に示します。

## <a name="derived-types"></a>派生型
| 型 | 説明 |
|:-|:-|
| [**educationIdentityMatchingConfiguration**](educationidentitymatchingconfiguration.md) | Azure Active Directory (AD の Azure) 内の既存のユーザー アカウントを一致させるには、この型を使用します。 |
| [**educationIdentityCreationConfiguration**](educationidentitycreationconfiguration.md) | Azure AD で新しいユーザー アカウントを作成するのにには、この型を使用します。 |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationidentitysynchronizationconfiguration.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
