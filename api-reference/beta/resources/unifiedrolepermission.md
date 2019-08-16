---
title: unifiedRolePermission リソースの種類
description: ディレクトリロールのアクセス許可は、許可されているリソースのアクションと条件の集合です。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d15e2709c429be3c6400b59db5174093892d3009
ms.sourcegitcommit: 567d0420243765b4088bc8029306a517f92926fd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/16/2019
ms.locfileid: "36437861"
---
# <a name="unifiedrolepermission-resource-type"></a>unifiedRolePermission リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

許可されたリソースアクションのコレクションと、アクションを有効にするために満たす必要がある条件を表します。 リソースアクションとは、リソースに対して perfomed が可能なタスクのことです。 たとえば、アプリケーションリソースは、[作成]、[更新]、[削除]、および [パスワードのリセット] リソースアクションをサポートしています。

## <a name="properties"></a>プロパティ

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
|allowedResourceActions|文字列コレクション| リソースに対して perfomed が可能な一連のタスク。 |
|文|String| アクセス許可を有効にするために満たす必要のあるオプション制約。 |

### <a name="allowedresourceactions-property"></a>allowedResourceActions プロパティ

リソースアクションのスキーマは次のとおりです。 

```
<Namespace>/<Entity>/<PropertySet>/<Action>  
```
例: `microsoft.directory/applications/credentials/update`。  

- 名前空間-タスクを公開するサービス。 たとえば、Azure Active Directory のすべてのタスクは、名前空間の microsoft directory を使用します。  
- エンティティ-Microsoft Graph のサービスによって公開される論理機能またはコンポーネント。 たとえば、アプリケーション、サービスプリンシパル、グループなどです。
- PropertySet-アクセスが許可されているエンティティの特定のプロパティまたは側面。 たとえば、で`microsoft.directory/applications/authentication/read`は、Azure AD の**application**オブジェクトの応答 url、ログアウト url、および暗黙的フロープロパティを読み取る機能を付与します。 一般的なプロパティセットに対して予約されている名前を次に示します。  
  - allProperties-特権プロパティを含む、エンティティのすべてのプロパティを指定します。 例`microsoft.directory/applications/allProperties/read`を`microsoft.directory/applications/allProperties/update`示します。
  - 基本-一般的な読み取りプロパティを指定しますが、特権付きプロパティを除外します。 たとえば、に`microsoft.directory/applications/basic/update`は、表示名などの標準プロパティを更新する機能が含まれています。
  - standard-共通の更新プロパティを指定します。ただし、特権付きのプロパティを除外します。 たとえば、`microsoft.directory/applications/standard/read` などです。
- アクション-付与されている操作。 ほとんどの場合、アクセス許可は CRUD または allTasks で表現する必要があります。 アクションには次のものがあります。
  - Create-エンティティの新しいインスタンスを作成する機能。
  - 読み取り-特定のプロパティセットを読み取る機能 (allProperties を含む)。
  - 更新-特定のプロパティセットを更新する機能 (allProperties を含む)。
  - 削除-特定のエンティティを削除する機能。
  - AllTasks-すべての CRUD 操作 (作成、読み取り、更新、および削除) を表します。 

### <a name="condition-property"></a>condition プロパティ
条件では、満たされる必要のある制約が定義されます。 たとえば、プリンシパルがターゲットの "所有者" になるという要件があります。 以下に、サポートされている条件を示します。

- Self: "@Subject = = @Resource objectId"
- Owner: "@Subject Any_of @Resource owners"

次に示すのは、条件を持つロール権限の例です。

```json
"rolePermissions": [
        {
            "allowedResourceActions": [
                "microsoft.directory/applications/basic/update",
                "microsoft.directory/applications/credentials/update"
            ],
            "condition":  "@Subject.objectId Any_of @Resource.owners"
        }
    ]

```

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.unifiedRolePermission",
  "baseType": null
}-->

```json
{
  "allowedResourceActions": ["String"],
  "condition": "String"
}
```
## <a name="see-also"></a>関連項目

- [Azure Active directory の管理者の役割のアクセス](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles)許可-組み込みのディレクトリの役割のアクセス許可についての情報。
- [Azure Active Directory のアプリケーション登録サブタイプとアクセス許可](https://docs.microsoft.com/azure/active-directory/users-groups-roles/roles-custom-available-permissions)-カスタムディレクトリロールで使用可能なアクセス許可についての情報。 

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "unifiedRolePermission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
