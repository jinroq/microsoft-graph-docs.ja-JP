---
title: oAuth2PermissionGrant リソースの種類
description: ユーザーまたは管理者の同意プロセスの一部としてアプリケーション (サービスプリンシパルによって表される) に付与された OAuth 2.0 スコープ (デリゲートされたアクセス許可) を表します。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 25f012baca1a7dfa5aeb62b8885b00b151a657ed
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966616"
---
# <a name="oauth2permissiongrant-resource-type"></a>oAuth2PermissionGrant リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ユーザーまたは管理者の同意プロセスの一部としてアプリケーション (サービスプリンシパルによって表される) に付与された OAuth 2.0 スコープ (デリゲートされたアクセス許可) を表します。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant"
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
|clientId|String| リソースにアクセスするときにユーザーを偽装する同意を付与するサービスプリンシパルの id (resourceId プロパティで表されます)。 |
|consentType|String| 同意が管理者によって (組織の代わりに) 提供されたか、個人によって提供されたかを示します。 使用可能な値は*allprincipals*または*Principal*です。 |
|expiryTime|DateTimeOffset| 現時点では、有効期限の値は無視されます。 |
|id|文字列| 一意の識別子。 読み取り専用です。|
|principalId|String| Consettings Type が*Allprincipals*の場合、この値は null になり、組織内のすべてのユーザーに同意が適用されます。 Conな種類が*Principal*の場合、このプロパティは同意を付与されたユーザーの id を指定し、そのユーザーに対してのみ適用されます。 |
|resourceId|String| アクセスが許可されているリソースサービスプリンシパルの id を指定します。 |
|scope|文字列| OAuth 2.0 アクセストークンでリソースアプリケーションが想定する[スコープ](/graph/permissions-reference)要求の値を指定します。 たとえば、「ユーザー」と表示*します。* |
|startTime|DateTimeOffset| 現時点では、開始時刻の値は無視されます。 |

## <a name="relationships"></a>リレーションシップ
なし


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[OAuth2PermissionGrant を取得する](../api/oauth2permissiongrant-get.md) | [oAuth2PermissionGrant](oauth2permissiongrant.md) |OAuth2PermissionGrant オブジェクトのプロパティとリレーションシップを読み取ります。|
|[リスト oAuth2PermissionGrants](../api/oauth2permissiongrant-list.md) | [oAuth2PermissionGrant](oauth2permissiongrant.md) コレクション | Oauth2PermissionGrant オブジェクトのリストを取得します。 |
|[OAuth2PermissionGrant の更新](../api/oauth2permissiongrant-update.md) | [oAuth2PermissionGrant](oauth2permissiongrant.md) |OAuth2PermissionGrant オブジェクトを更新します。 |
|[OAuth2PermissionGrant の削除](../api/oauth2permissiongrant-delete.md) | None |OAuth2PermissionGrant オブジェクトを削除します。 |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oAuth2PermissionGrant resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
