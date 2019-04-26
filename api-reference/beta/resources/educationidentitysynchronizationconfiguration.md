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

## <a name="json-representation"></a>JSON 表記
<!-- {
  "blockType": "resource",
   "isAbstract":true,
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentitySynchronizationConfiguration"
}-->

```json
{
}
```

