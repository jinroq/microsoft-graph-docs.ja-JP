---
title: UnifiedRoleDefinition の更新
description: UnifiedRoleDefinition オブジェクトのプロパティを更新します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3be16446147e3e0dd9d4c2a481b5fdae63312f6a
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/19/2019
ms.locfileid: "36461635"
---
# <a name="update-unifiedroledefinition"></a>UnifiedRoleDefinition の更新

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[UnifiedRoleDefinition](../resources/unifiedroledefinition.md)オブジェクトのプロパティを更新します。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

| アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ) |
|:---------------------------------------|:--------------------------------------------|
| 委任 (職場または学校のアカウント)     | RoleManagement、RoleManagement、またはディレクトリ |
| 委任 (個人用 Microsoft アカウント) | サポートされていません。 |
| アプリケーション                            | RoleManagement、RoleManagement、またはディレクトリ |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
PATCH /roleManagement/directory/roleDefinitions/{id}
```

## <a name="request-headers"></a>要求ヘッダー

| 名前       | 説明|
|:-----------|:-----------|
| Authorization | ベアラー {トークン} |

## <a name="request-body"></a>要求本文

要求本文で、更新する関連フィールドの値を指定します。 要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。 最適なパフォーマンスを得るために、変更されていない既存の値を含めないでください。

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
|description|String| ロール定義の説明。 IsBuiltIn が true の場合は、値の取得のみ可能です。 |
|displayName|String| ロール定義の表示名。 IsBuiltIn が true の場合は、値の取得のみ可能です。 必須。|
|id|文字列| ロール定義の一意識別子。 キー。 null 許容ではありません。読み取り専用です。 |
|isBuiltIn|Boolean| ロール定義が product または custom に含まれる既定のセットの一部であるかどうかを示すフラグ。 読み取り専用。 |
|isEnabled|Boolean| 役割が割り当てに対して有効になっているかどうかを示すフラグ。 False の場合、役割は割り当てに使用できません。 IsBuiltIn が true の場合は、値の取得のみ可能です。 |
|resourceScopes|String コレクション| ロール定義によって付与される範囲のアクセス許可の一覧が適用されます。 現時点では "/" のみがサポートされています。 IsBuiltIn が true の場合は、値の取得のみ可能です。 |
|rolePermissions|[unifiedRolePermission](../resources/unifiedrolepermission.md)コレクション| 役割に含まれるアクセス許可の一覧。 IsBuiltIn が true の場合は、値の取得のみ可能です。 必須です。 |
|templateId|String| IsBuiltIn が false のときに設定できるカスタムテンプレート識別子。 この識別子は、通常、異なるディレクトリ間で識別子を同じにする必要がある場合に使用されます。 IsBuiltIn が true の場合は、値の取得のみ可能です。 |
|version|String| ロール定義のバージョンを示します。 IsBuiltIn が true の場合は、値の取得のみ可能です。|

## <a name="response"></a>応答

成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[unifiedRoleDefinition](../resources/unifiedroledefinition.md)オブジェクトを返します。

## <a name="example"></a>例

### <a name="request"></a>要求

要求の例を次に示します。

# <a name="httptabhttp"></a>[プロトコル](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_unifiedroledefinition"
}-->

```http
PATCH https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/0d55728d-3e24-4309-9b1b-5ac09921475a
Content-type: application/json

{
  "description": "Update basic properties of application registrations",
  "displayName": "Application Registration Support Administrator",
  "rolePermissions":
    [
        {
            "allowedResourceActions": 
            [
                "microsoft.directory/applications/basic/read"
            ]
        }
    ]
}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目的-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>応答

応答の例を次に示します。

> **注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleDefinition"
} -->

```http
HTTP/1.1 204 OK
Content-type: application/json

```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update unifiedroledefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
