---
title: servicePrincipal リソースの種類
description: ディレクトリ内のアプリケーションのインスタンスを表します。 directoryObject から継承します。
localization_priority: Priority
ms.openlocfilehash: d36a82ae885725387e788cf280442afe09fa63de
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574188"
---
# <a name="serviceprincipal-resource-type"></a>servicePrincipal リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ディレクトリ内のアプリケーションのインスタンスを表します。 [directoryObject](directoryobject.md) から継承します。

このリソースは以下をサポートしています。

- [デルタ](../api/serviceprincipal-delta.md)関数を提供することにより、[デルタ クエリ](/graph/delta-query-overview)を使用して、増分の追加、削除、更新を追跡します。

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "appRoleAssignedTo",
    "appRoleAssignments",
    "createdObjects",
    "createdOnBehalfOf",
    "memberOf",
    "oauth2PermissionGrants",
    "ownedObjects",
    "owners"
  ],
  "@odata.type": "microsoft.graph.servicePrincipal"
}-->

```json
{
  "accountEnabled": true,
  "addIns": [{"@odata.type": "microsoft.graph.addIn"}],
  "appDisplayName": "string",
  "appId": "string",
  "appOwnerOrganizationId": "guid",
  "appRoleAssignmentRequired": true,
  "displayName": "string",
  "errorUrl": "string",
  "homepage": "string",
  "id": "string (identifier)",
  "keyCredentials": [{"@odata.type": "microsoft.graph.keyCredential"}],
  "logoutUrl": "string",
  "oauth2Permissions": [{"@odata.type": "microsoft.graph.oAuth2Permission"}],
  "passwordCredentials": [{"@odata.type": "microsoft.graph.passwordCredential"}],
  "preferredTokenSigningKeyThumbprint": "string",
  "publisherName": "string",
  "replyUrls": ["string"],
  "samlMetadataUrl": "string",
  "servicePrincipalNames": ["string"],
  "tags": ["string"]
}

```
## <a name="properties"></a>プロパティ
| プロパティ     | 型 |説明|
|:---------------|:--------|:----------|
|accountEnabled|Boolean| サービス プリンシパルのアカウントが有効な場合は **true**。それ以外の場合は **false**。            |
|appDisplayName|String|関連付けられているアプリケーションによって公開される表示名。|
|appId|String|関連付けられたアプリケーションの一意の識別子 (その **appId** プロパティ)。|
|appRoleAssignmentRequired|Boolean|Azure AD からアプリケーションにユーザー トークンまたはアクセス トークンが発行される前に、ユーザーまたはグループに対する **appRoleAssignment** が必要かどうかを指定します。 null 許容型ではありません。 |
|appRoles|[appRole](approle.md) コレクション|関連付けられているアプリケーションによって公開されるアプリケーション ロール。 さらに詳しい情報については、[アプリケーション](application.md) エンティティの **appRoles** プロパティの定義を参照してください。 null 許容型ではありません。 |
|displayName|String|サービス プリンシパルの表示名。|
|errorUrl|String|            |
|HomePage|String|関連付けられたアプリケーションのホーム ページの URL。|
|keyCredentials|[keyCredential](keycredential.md) コレクション|サービス プリンシパルに関連付けられているキー資格情報のコレクションです。null 許容型ではありません。 null 許容型ではありません。            |
|logoutUrl|String| Microsoft の承認サービスで、[フロント チャネル](https://openid.net/specs/openid-connect-frontchannel-1_0.html)、[バック チャネル](https://openid.net/specs/openid-connect-backchannel-1_0.html)または SAML ログアウト プロトコルを使ってユーザーのログアウトするのに使う URL を指定します。  |
|oauth2Permissions|[oAuth2Permission](oauth2permission.md) コレクション|関連付けられているアプリケーションによって公開される OAuth 2.0 のアクセス許可。 さらに詳しい情報については、[アプリケーション](application.md) エンティティの **oauth2Permissions** プロパティの定義を参照してください。 null 許容型ではありません。            |
|id|String|サービス プリンシパルの一意識別子。 [directoryObject](directoryobject.md) から継承されます。 キー。 null 許容ではありません。 読み取り専用です。|
|passwordCredentials|[passwordCredential](passwordcredential.md) コレクション|サービス プリンシパルに関連付けられているパスワード資格情報のコレクションです。null 許容型ではありません。 null 許容型ではありません。 |
|preferredTokenSigningKeyThumbprint|String|内部使用専用に予約済みです。 このプロパティに書き込みしたり、依存したりしないでください。 将来のバージョンで削除される可能性があります。 |
|publisherName|String|関連付けられたアプリケーションが指定されているテナントの表示名。|
|replyUrls|String コレクション|関連付けられたアプリケーションにサインインするためにユーザー トークンが送信される URL、または関連付けられたアプリケーションに対して OAuth 2.0 認証コードとアクセス トークンが送信されるリダイレクト URI。 null 許容型ではありません。 |
|samlMetadataUrl|String| |
|servicePrincipalNames|String コレクション|関連するアプリケーションを識別する URI です。 詳細情報については、「[アプリケーション オブジェクトとサービス プリンシパル オブジェクト](https://msdn.microsoft.com/library/azure/dn132633.aspx)」を参照してください。複数値プロパティのフィルター式には **any** 演算子が必要です。  null 許容型ではありません。 |
|tags|String コレクション| null 許容型ではありません。 |

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型 |説明|
|:---------------|:--------|:----------|
|appRoleAssignedTo| [appRoleAssignment](approleassignment.md) |このサービス プリンシパルに割り当てられているプリンシパル (ユーザー、グループ、サービス プリンシパル)。 読み取り専用です。|
|appRoleAssignments|[appRoleAssignment](approleassignment.md) コレクション|サービス プリンシパルが割り当てられているアプリケーション。 読み取り専用です。 Null 許容型。|
|createdObjects|[directoryObject](directoryobject.md) コレクション|このサービス プリンシパルで作成したディレクトリ オブジェクト。 読み取り専用です。 Null 許容型。|
|memberOf| [directoryObject](directoryobject.md) コレクション|このサービス プリンシパルがメンバーになっているロール。 HTTP メソッド: GET 読み取り専用。 Null 許容型です。|
|oauth2PermissionGrants| [oAuth2PermissionGrant](oauth2permissiongrant.md) コレクション|このサービス プリンシパルに関連付けられているユーザーの偽装許可です。 読み取り専用です。 Null 許容型。|
|ownedObjects| [directoryObject](directoryobject.md) コレクション|このサービス プリンシパルで所有しているディレクトリ オブジェクト。 読み取り専用です。 Null 許容型です。|
|owners| [directoryObject](directoryobject.md) コレクション|このサービス プリンシパルで所有者であるディレクトリ オブジェクト。 所有者は、このオブジェクトの変更を許可されている管理者以外のユーザーです。 読み取り専用です。 Null 許容型です。|
|policy| [policy](policy.md) コレクション|このサービス プリンシパルに割り当てられているポリシー。|

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[servicePrincipal を取得する](../api/serviceprincipal-get.md) | [servicePrincipal](serviceprincipal.md) |servicePrincipal オブジェクトのプロパティとリレーションシップを読み取ります。|
|[servicePrincipals を一覧表示する](../api/serviceprincipal-list.md) | [servicePrincipal](serviceprincipal.md) コレクション | servicePrincipal オブジェクトの一覧を取得します。 |
|[appRoleAssignment を作成する](../api/serviceprincipal-post-approleassignments.md) |[appRoleAssignment](approleassignment.md)| appRoleAssignment コレクションに投稿して新しい AppRoleAssignments を作成します。|
|[appRoleAssignments を一覧表示する](../api/serviceprincipal-list-approleassignments.md) |[appRoleAssignment](approleassignment.md) コレクション| appRoleAssignment オブジェクト コレクションを取得します。|
|[createdObjects を一覧表示する](../api/serviceprincipal-list-createdobjects.md) |[directoryObject](directoryobject.md) コレクション| createdObject オブジェクト コレクションを取得します。|
|[memberOf を一覧表示する](../api/serviceprincipal-list-memberof.md) |[directoryObject](directoryobject.md) コレクション| memberOf ナビゲーション プロパティからこのサービス プリンシパルが直接のメンバーであるグループを取得します。|
|[推移的な memberOf を一覧表示する](../api/serviceprincipal-list-transitivememberof.md) |[directoryObject](directoryobject.md) コレクション| このサービス プリンシパルがメンバーになっているグループを一覧表示します。 この操作は推移的で、このサービス プリンシパルが入れ子のメンバーになっているグループが含まれます。 |
|[割り当てられているポリシーを一覧表示する](../api/policy-list-assigned.md)| [policy](policy.md) コレクション| このオブジェクトに割り当てられているすべてのポリシーを取得します。|
|[oauth2PermissionGrants を一覧表示する](../api/serviceprincipal-list-oauth2permissiongrants.md) |[oAuth2PermissionGrant](oauth2permissiongrant.md) コレクション| oAuth2PermissionGrant オブジェクト コレクションを取得します。|
|[ownedObjects を一覧表示する](../api/serviceprincipal-list-ownedobjects.md) |[directoryObject](directoryobject.md) コレクション| ownedObject オブジェクト コレクションを取得します。|
|[所有者を追加する](../api/serviceprincipal-post-owners.md) |[directoryObject](directoryobject.md)| 所有者のコレクションに投稿して、新しい所有者を作成します。|
|[所有者を一覧表示する](../api/serviceprincipal-list-owners.md) |[directoryObject](directoryobject.md) コレクション| owner オブジェクトのコレクションを取得します。|
|[更新する](../api/serviceprincipal-update.md) | [servicePrincipal](serviceprincipal.md)  |servicePrincipal オブジェクトを更新します。 |
|[削除する](../api/serviceprincipal-delete.md) | なし |servicePrincipal オブジェクトを削除します。 |
|[checkMemberGroups](../api/serviceprincipal-checkmembergroups.md)|String コレクション||
|[getMemberGroups](../api/serviceprincipal-getmembergroups.md)|String コレクション||
|[getMemberObjects](../api/serviceprincipal-getmemberobjects.md)|String コレクション||
|[差分](../api/serviceprincipal-delta.md)|servicePrincipal コレクション| サービス プリンシパルに対する増分の変更を取得します。 |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "servicePrincipal resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/serviceprincipal.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
