---
title: oAuth2PermissionGrant リソースの種類
description: (サービス主体で表されます)、アプリケーションに与えられている OAuth 2.0 のスコープ (委任されたアクセス許可) をユーザーまたは管理者の承認プロセスの一環として表します。
localization_priority: Normal
ms.openlocfilehash: ea6486aedca4c3fcf73e59a5652ccf517fb01ddc
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640778"
---
# <a name="oauth2permissiongrant-resource-type"></a>oAuth2PermissionGrant リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

(サービス主体で表されます)、アプリケーションに与えられている OAuth 2.0 のスコープ (委任されたアクセス許可) をユーザーまたは管理者の承認プロセスの一環として表します。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.oAuth2Permissiongrant"
}-->

```json
{
  "clientId": "string",
  "consentType": "string",
  "expiryTime": "String (timestamp)",
  "id": "string (identifier)",
  "principalId": "string",
  "resourceId": "string",
  "scope": "string",
  "startTime": "String (timestamp)"
}

```
## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|clientId|String| サービス ・ プリンシパルの id 付与 (resourceId プロパティによって表される) リソースにアクセスするときにユーザーを偽装するのに同意するものです。 |
|consentType|String| 同意が管理者 (組織) のため、個人に提供されるかどうかを示します。 使用可能な値は、 *AllPrincipals*または*プリンシパル*です。 |
|expiryTime|DateTimeOffset| 現在、有効期限の時刻の値は無視されます。 |
|id|String| 一意の識別子です。 読み取り専用です。|
|principalId|String| ConsentType が*AllPrincipals*である場合は、この値が null の場合と同意は、組織内のすべてのユーザーに適用されます。 ConsentType が*主体*の場合は、このプロパティは同意を付与し、そのユーザーに対してのみ適用されるユーザーの id を指定します。 |
|resourceId|String| アクセスが許可されているリソース ・ サービス ・ プリンシパルの id を指定します。 |
|scope|String| OAuth 2.0 のアクセス トークンには、リソース アプリケーションが期待する[スコープ](/graph/permissions-reference)の要求の値を指定します。 たとえば、 *User.Read* |
|startTime|DateTimeOffset| 現時点では、開始時刻の値は無視されます。 |

## <a name="relationships"></a>リレーションシップ
なし


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[OAuth2PermissionGrant を取得します。](../api/oauth2permissiongrant-get.md) | [oAuth2PermissionGrant](oauth2permissiongrant.md) |OAuth2PermissionGrant オブジェクトのプロパティと関係を参照してください。|
|[リスト oAuth2PermissionGrants](../api/oauth2permissiongrant-list.md) | [oAuth2PermissionGrant](oauth2permissiongrant.md) コレクション | Oauth2PermissionGrant オブジェクトのリストを取得します。 |
|[OAuth2PermissionGrant を更新します。](../api/oauth2permissiongrant-update.md) | [oAuth2PermissionGrant](oauth2permissiongrant.md) |OAuth2PermissionGrant オブジェクトを更新します。 |
|[OAuth2PermissionGrant を削除します。](../api/oauth2permissiongrant-delete.md) | なし |OAuth2PermissionGrant オブジェクトを削除します。 |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oAuth2PermissionGrant resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/oauth2permissiongrant.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
