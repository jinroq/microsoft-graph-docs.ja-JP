---
title: servicePrincipal リソースの種類
description: ディレクトリ内のアプリケーションのインスタンスを表します。 directoryObject から継承します。
localization_priority: Priority
ms.openlocfilehash: 2df27225f62e7c2b7b026bb3d829abf546241267
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27880207"
---
# <a name="serviceprincipal-resource-type"></a>servicePrincipal リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

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
  "@odata.type": "microsoft.graph.serviceprincipal"
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
| プロパティ     | 種類 |説明|
|:---------------|:--------|:----------|
|accountEnabled|ブール型| **true**サービス プリンシパル アカウントは、有効な場合それ以外の場合、 **false を指定**します。            |
|appDisplayName|String|関連付けられたアプリケーションによって公開される表示名です。|
|appId|文字列型 (String)|関連付けられているアプリケーション (その**appId**プロパティの一意の識別子です。|
|appRoleAssignmentRequired|ブール型|Azure AD アプリケーションに、ユーザーまたはアクセス トークンの発行は前にユーザーまたはグループに、 **appRoleAssignment**が必要かどうかを指定します。 null 許容ではありません。 |
|appRoles|[エンティティ](approle.md)のコレクション|アプリケーション ロールは、関連付けられたアプリケーションによって公開されています。 詳細については、[アプリケーション](application.md)エンティティの**appRoles**プロパティの定義を参照してください。 null 許容ではありません。 |
|displayName|String|サービス ・ プリンシパルの表示名です。|
|errorUrl|String|            |
|ホームページ|String|関連付けられたアプリケーションのホーム ページの URL です。|
|keyCredentials|[keyCredential](keycredential.md)コレクション|サービス ・ プリンシパルに関連付けられているキーの資格情報のコレクションです。 null 許容ではありません。            |
|logoutUrl|String| [前方チャンネル](https://openid.net/specs/openid-connect-frontchannel-1_0.html)、[背面チャネル](https://openid.net/specs/openid-connect-backchannel-1_0.html)または SAML ログアウトのプロトコルを使用してユーザーをログアウトするマイクロソフトの承認のサービスによって使用される URL を指定します。  |
|oauth2Permissions|[oAuth2Permission](oauth2permission.md)コレクション|関連付けられたアプリケーションによって公開される OAuth 2.0 のアクセス許可。 詳細については、[アプリケーション](application.md)エンティティの**oauth2Permissions**プロパティの定義を参照してください。 null 許容ではありません。            |
|id|String|サービス ・ プリンシパルの一意の識別子です。 [directoryObject](directoryobject.md) から継承されます。 キー。 null 許容ではありません。 読み取り専用です。|
|passwordCredentials|[passwordCredential](passwordcredential.md)コレクション|サービス ・ プリンシパルに関連付けられているパスワード資格情報のコレクションです。 null 許容ではありません。 |
|preferredTokenSigningKeyThumbprint|String|内部使用専用として予約されています。   記述したり、それ以外の場合、このプロパティに依存しないでください。 将来のバージョンで削除する可能性があります。 |
|publisherName|文字列型 (String)|関連付けられたアプリケーションが指定されているテナントの表示名です。|
|replyUrls|String コレクション|ユーザー トークン用に送信される、関連するアプリケーション、またはリダイレクトを使用して記号を OAuth 2.0 の Uri の認証コードをアクセス トークンは、関連付けられたアプリケーション用に送信される Url です。 null 許容ではありません。 |
|samlMetadataUrl|String| |
|servicePrincipalNames|String コレクション|関連付けられたアプリケーションを識別する Uri。 詳細情報は、「[アプリケーションのオブジェクトおよびオブジェクトのサービス プリンシパル](https://msdn.microsoft.com/library/azure/dn132633.aspx)です。**Any**演算子は、複数値を持つプロパティのフィルター式に必要です。  null 許容ではありません。 |
|タグの前に追加されるマークアップ|String コレクション| null 許容ではありません。 |

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型 |説明|
|:---------------|:--------|:----------|
|appRoleAssignedTo|[appRoleAssignment](approleassignment.md)|プリンシパル (ユーザー、グループ、およびサービス プリンシパル) このサービス ・ プリンシパルに割り当てられています。 読み取り専用です。|
|appRoleAssignments|[appRoleAssignment](approleassignment.md)コレクション|サービス ・ プリンシパルが割り当てられているアプリケーションです。 読み取り専用です。 Null 許容型。|
|createdObjects|[directoryObject](directoryobject.md) コレクション|ディレクトリ オブジェクトがこのサービス ・ プリンシパルを作成します。 読み取り専用です。 Null 許容型。|
|memberOf|[directoryObject](directoryobject.md) コレクション|このサービス主体のメンバーである役割。 : の HTTP メソッドは、読み取り専用を取得します。 Null 許容型。|
|oauth2PermissionGrants|[oAuth2PermissionGrant](oauth2permissiongrant.md)コレクション|ユーザーの偽装の補助金がこのサービス ・ プリンシパルに関連付けられています。 読み取り専用です。 Null 許容型。|
|ownedObjects|[directoryObject](directoryobject.md) コレクション|このサービス ・ プリンシパルが所有するディレクトリ オブジェクトです。 読み取り専用です。 Null 許容型。|
|owners|[directoryObject](directoryobject.md) コレクション|このサービス ・ プリンシパルの所有者であるディレクトリ オブジェクトです。 所有者は、このオブジェクトを変更するのには許可されている管理者以外のユーザーのセットです。 読み取り専用です。 Null 許容型。|
|役割|[ポリシー](policy.md)コレクション|このサービス ・ プリンシパルに割り当てられているポリシーです。|

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[ServicePrincipal を取得します。](../api/serviceprincipal-get.md) | [servicePrincipal](serviceprincipal.md) |ServicePrincipal オブジェクトのプロパティと関係を参照してください。|
|[リスト servicePrincipals](../api/serviceprincipal-list.md) | [servicePrincipal](serviceprincipal.md)コレクション | ServicePrincipal オブジェクトのリストを取得します。 |
|[AppRoleAssignment を作成します。](../api/serviceprincipal-post-approleassignments.md) |[appRoleAssignment](approleassignment.md)| AppRoleAssignments コレクションへの投稿には、新しい appRoleAssignment を作成します。|
|[リスト appRoleAssignments](../api/serviceprincipal-list-approleassignments.md) |[appRoleAssignment](approleassignment.md)コレクション| AppRoleAssignment オブジェクトのコレクションを取得します。|
|[List createdObjects](../api/serviceprincipal-list-createdobjects.md) |[directoryObject](directoryobject.md) collection| CreatedObject オブジェクトのコレクションを取得します。|
|[memberOf を一覧表示する](../api/serviceprincipal-list-memberof.md) |[directoryObject](directoryobject.md) コレクション| このサービス ・ プリンシパルがへの後方リンクのナビゲーション プロパティからの直接メンバーであるグループを取得します。|
|[推移的な所属するグループ] ボックスの一覧](../api/serviceprincipal-list-transitivememberof.md) |[directoryObject](directoryobject.md) コレクション| このサービス主体のメンバーであるグループを一覧表示します。 この操作では、推移的では、このサービス ・ プリンシパルの入れ子にされたメンバーであるグループが含まれています。 |
|[リストが割り当てられているポリシー](../api/policy-list-assigned.md)| [ポリシー](policy.md)コレクション| このオブジェクトに割り当てられているすべてのポリシーを取得します。|
|[リスト oauth2PermissionGrants](../api/serviceprincipal-list-oauth2permissiongrants.md) |[oAuth2PermissionGrant](oauth2permissiongrant.md)コレクション| OAuth2PermissionGrant オブジェクトのコレクションを取得します。|
|[List ownedObjects](../api/serviceprincipal-list-ownedobjects.md) |[directoryObject](directoryobject.md) collection| OwnedObject オブジェクトのコレクションを取得します。|
|[Add owner](../api/serviceprincipal-post-owners.md) |[directoryObject](directoryobject.md)| 所有者のコレクションへの投稿には、新しい所有者を作成します。|
|[所有者を一覧表示する](../api/serviceprincipal-list-owners.md) |[directoryObject](directoryobject.md) コレクション| 所有者のオブジェクトのコレクションを取得します。|
|[Update](../api/serviceprincipal-update.md) | [servicePrincipal](serviceprincipal.md)  |ServicePrincipal オブジェクトを更新します。 |
|[Delete](../api/serviceprincipal-delete.md) | なし |ServicePrincipal オブジェクトを削除します。 |
|[checkMemberGroups](../api/serviceprincipal-checkmembergroups.md)|String コレクション||
|[getMemberGroups](../api/serviceprincipal-getmembergroups.md)|String コレクション||
|[getMemberObjects](../api/serviceprincipal-getmemberobjects.md)|String コレクション||
|[delta](../api/serviceprincipal-delta.md)|servicePrincipal コレクション| サービス ・ プリンシパルの増分の変更を取得します。 |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "servicePrincipal resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
