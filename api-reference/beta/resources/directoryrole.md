---
title: directoryRole リソース型
description: Azure AD ディレクトリ ロールを表します。Azure AD ディレクトリ ロールは、*管理者ロール*と呼ばれることもあります。ディレクトリ (管理者) ロールの詳細については、「Azure Active Directory での管理者ロールの割り当て」を参照してください。Microsoft Graph では、ユーザーにディレクトリ ロールを割り当てることで、ターゲット ロールのアクセス許可をユーザーに付与できます。ディレクトリ ロールを読み取る場合や、そのメンバーを更新する場合は、まず、そのディレクトリ ロールをテナントでアクティブにする必要があります。既定では、会社の管理者 (Company Administrators) ディレクトリ ロールのみがアクティブ化されています。その他の使用可能なディレクトリ ロールをアクティブ化するには、directoryRoleTemplate の ID を使用して POST 要求を送信します。この ID は、ディレクトリ ロールに基づきます。directoryObject から継承します。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 30b22313da70c33bffc0b759f9b474f4deac2ac1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521251"
---
# <a name="directoryrole-resource-type"></a>directoryRole リソース型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure AD ディレクトリ ロールを表します。Azure AD ディレクトリ ロールは、*管理者ロール*と呼ばれることもあります。ディレクトリ (管理者) ロールの詳細については、「[Azure Active Directory での管理者ロールの割り当て](https://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/)」を参照してください。Microsoft Graph では、ユーザーにディレクトリ ロールを割り当てることで、ターゲット ロールのアクセス許可をユーザーに付与できます。ディレクトリ ロールを読み取る場合や、そのメンバーを更新する場合は、まず、そのディレクトリ ロールをテナントでアクティブにする必要があります。既定では、会社の管理者 (Company Administrators) ディレクトリ ロールのみがアクティブ化されています。その他の使用可能なディレクトリ ロールをアクティブ化するには、[directoryRoleTemplate](directoryroletemplate.md) の ID を使用して POST 要求を送信します。この ID は、ディレクトリ ロールに基づきます。[directoryObject](directoryobject.md) から継承します。

ディレクトリの役割は、既定では、テナント全体に適用されます。  ただし、ディレクトリの役割 (現在のみ*のユーザー アカウントの管理者**ヘルプデスクの管理者*) は[管理単位](administrativeunit.md)にスコープも可能性があります。

このリソースは以下をサポートしています。

- [デルタ](../api/directoryrole-delta.md)関数を提供することにより、[デルタ クエリ](/graph/delta-query-overview)を使用して、増分の追加、削除、更新を追跡します。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[Get directoryRole](../api/directoryrole-get.md) | [directoryRole](directoryrole.md) |directoryRole オブジェクトのプロパティとリレーションシップを読み取ります。|
|[directoryRoles を一覧表示する](../api/directoryrole-list.md) | [directoryRole](directoryrole.md) コレクション | テナントでアクティブになっているディレクトリ ロールを一覧表示します。 |
|[メンバーを追加する](../api/directoryrole-post-members.md) |[directoryObject](directoryobject.md)| members ナビゲーション プロパティを送信することで、ユーザーをディレクトリ ロールに追加します。|
|[List members](../api/directoryrole-list-members.md) |[directoryObject](directoryobject.md) コレクション| members ナビゲーション プロパティから、ディレクトリ ロールのメンバーであるユーザーを取得します。|
|[メンバーを削除する](../api/directoryrole-delete-member.md) |[directoryObject](directoryobject.md)| ディレクトリ ロールからユーザーを削除します。|
|[スコープ ロールのメンバーの一覧](../api/directoryrole-list-members.md) |scopedRoleMembership コレクション| スコープは、[管理単位](administrativeunit.md)、scopedRoleMembership リソースのコレクションをこのディレクトリのロールのメンバーを一覧表示します。|
|[delta](../api/directoryrole-delta.md)|directoryRole コレクション| ディレクトリの役割の増分の変更を取得します。 |

## <a name="properties"></a>プロパティ
| プロパティ   | 型 |説明|
|:---------------|:--------|:----------|
|説明|文字列|ディレクトリ ロールの説明。読み取り専用。 |
|displayName|String|ディレクトリ ロールの表示名。読み取り専用。 |
|id|文字列|ディレクトリ ロールの一意識別子。[directoryObject](directoryobject.md) から継承されます。キーであり、Null は許容されません。読み取り専用です。|
|roleTemplateId|String| このロールが基づいている [directoryRoleTemplate](directoryroletemplate.md) の **id**。このプロパティは、POST 操作でテナント内のディレクトリ ロールをアクティブ化するときに指定する必要があります。そのディレクトリ ロールがアクティブ化されると、このプロパティは読み取り専用になります。 |

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型 |説明|
|:---------------|:--------|:----------|
|members|[directoryObject](directoryobject.md) コレクション|このディレクトリ ロールのメンバーであるユーザー。HTTP メソッド: GET、POST、DELETE。読み取り専用。Null 許容型。|
|scopedMembers|scopedRoleMembership コレクション| [管理単位](administrativeunit.md)のスコープはこのディレクトリのロールのメンバーです。 読み取り専用です。 Null 許容型。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "memberOf",
    "members",
    "ownedObjects",
    "owners"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directoryRole"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)",
  "roleTemplateId": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directoryRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/directoryrole.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
