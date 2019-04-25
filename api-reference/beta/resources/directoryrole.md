---
title: directoryRole リソース型
description: Azure AD ディレクトリ ロールを表します。 Azure AD ディレクトリ ロールは、*管理者ロール*と呼ばれることもあります。 ディレクトリ (管理者) ロールの詳細については、「Azure Active Directory での管理者ロールの割り当て」を参照してください。 Microsoft Graph では、ユーザーにディレクトリ ロールを割り当てることで、ターゲット ロールのアクセス許可をユーザーに付与できます。 ディレクトリ ロールを読み取る場合や、そのメンバーを更新する場合は、まず、そのディレクトリ ロールをテナントでアクティブにする必要があります。 既定では、会社の管理者 (Company Administrators) ディレクトリ ロールのみがアクティブ化されています。 他の利用可能なディレクトリロールをアクティブにするには、ディレクトリロールの基になる directoryroletemplate の ID を持つ POST 要求を送信します。 directoryObject から継承します。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 30b22313da70c33bffc0b759f9b474f4deac2ac1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535274"
---
# <a name="directoryrole-resource-type"></a>directoryRole リソース型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure AD ディレクトリ ロールを表します。 Azure AD ディレクトリ ロールは、*管理者ロール*と呼ばれることもあります。 ディレクトリ (管理者) ロールの詳細については、「[Azure Active Directory での管理者ロールの割り当て](https://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/)」を参照してください。 Microsoft Graph では、ユーザーにディレクトリ ロールを割り当てることで、ターゲット ロールのアクセス許可をユーザーに付与できます。 ディレクトリ ロールを読み取る場合や、そのメンバーを更新する場合は、まず、そのディレクトリ ロールをテナントでアクティブにする必要があります。 既定では、会社の管理者 (Company Administrators) ディレクトリ ロールのみがアクティブ化されています。 他の利用可能なディレクトリロールをアクティブにするには、ディレクトリロールの基になる[directoryroletemplate](directoryroletemplate.md)の ID を持つ POST 要求を送信します。 [directoryObject](directoryobject.md) から継承します。

既定では、ディレクトリの役割のスコープはテナント全体になります。  ただし、ディレクトリの役割 (現時点では、*ユーザーアカウント管理*者と*ヘルプデスク管理者*のみ) の範囲を[管理単位](administrativeunit.md)に設定することもできます。

このリソースは以下をサポートしています。

- [デルタ](../api/directoryrole-delta.md)関数を提供することにより、[デルタ クエリ](/graph/delta-query-overview)を使用して、増分の追加、削除、更新を追跡します。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[Get directoryRole](../api/directoryrole-get.md) | [directoryRole](directoryrole.md) |directoryRole オブジェクトのプロパティとリレーションシップを読み取ります。|
|[directoryroles を一覧表示する](../api/directoryrole-list.md) | [directoryRole](directoryrole.md) コレクション | テナントでアクティブになっているディレクトリ ロールを一覧表示します。 |
|[メンバーを追加する](../api/directoryrole-post-members.md) |[directoryObject](directoryobject.md)| members ナビゲーション プロパティを送信することで、ユーザーをディレクトリ ロールに追加します。|
|[List members](../api/directoryrole-list-members.md) |[directoryObject](directoryobject.md) collection| members ナビゲーション プロパティから、ディレクトリ ロールのメンバーであるユーザーを取得します。|
|[Remove a member](../api/directoryrole-delete-member.md) |[directoryObject](directoryobject.md)| ディレクトリロールからユーザーを削除します。|
|[スコープが指定された役割のメンバーを一覧表示する](../api/directoryrole-list-members.md) |[scopedRoleMembership](scopedrolemembership.md) コレクション| scopedRoleMembership リソースコレクションを使用して、[管理単位](administrativeunit.md)にスコープが設定されているこのディレクトリロールのメンバーを一覧表示します。|
|[delta](../api/directoryrole-delta.md)|directoryRole コレクション| ディレクトリロールの増分の変更を取得します。 |

## <a name="properties"></a>プロパティ
| プロパティ   | 型 |説明|
|:---------------|:--------|:----------|
|description|String|ディレクトリ ロールの説明。読み取り専用。 |
|displayName|String|ディレクトリ ロールの表示名。読み取り専用。 |
|id|String|ディレクトリ ロールの一意識別子。[directoryObject](directoryobject.md) から継承されます。キーであり、Null は許容されません。読み取り専用です。|
|roleTemplateId|String| このロールが基づいている **directoryRoleTemplate** の [id](directoryroletemplate.md)。このプロパティは、POST 操作でテナント内のディレクトリ ロールをアクティブ化するときに指定する必要があります。そのディレクトリ ロールがアクティブ化されると、このプロパティは読み取り専用になります。 |

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型 |説明|
|:---------------|:--------|:----------|
|members|[directoryObject](directoryobject.md) コレクション|このディレクトリ ロールのメンバーであるユーザー。HTTP メソッド: GET、POST、DELETE。読み取り専用。Null 許容型。|
|scopedMembers|[scopedRoleMembership](scopedrolemembership.md) コレクション| [管理単位](administrativeunit.md)にスコープ設定されたこのディレクトリロールのメンバ。 読み取り専用。 Null 許容型。|

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
