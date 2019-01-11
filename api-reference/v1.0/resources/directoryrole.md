---
title: directoryRole リソース型
description: Azure AD ディレクトリの役割を表します。 Azure AD ディレクトリの役割は、*管理者の役割*とも呼ばれます。 ディレクトリ (管理者) の役割の詳細については、Azure AD の管理者の役割の割り当てを参照してください。 Graph とには、ターゲットのロールのアクセス許可を付与するディレクトリのロールにユーザーを割り当てることができます。 ディレクトリのロールの読み取りや、そのメンバーにする必要があります最初でアクティブにするテナントです。 会社の管理者のディレクトリの役割のみが既定でアクティブにします。 ディレクトリの役割の基になる directoryRoleTemplate の ID で POST 要求を送信するその他の利用可能なディレクトリの役割をアクティブ化します。 directoryObject から継承します。
localization_priority: Priority
ms.openlocfilehash: 05d897d6426b2feab7c08adaa125788590675f66
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820868"
---
# <a name="directoryrole-resource-type"></a>directoryRole リソース型

Azure AD ディレクトリの役割を表します。 Azure AD ディレクトリの役割は、*管理者の役割*とも呼ばれます。 ディレクトリ (管理者) の役割の詳細については、 [Azure AD の管理者ロールの割り当て](http://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/)を参照してください。 Graph とには、ターゲットのロールのアクセス許可を付与するディレクトリのロールにユーザーを割り当てることができます。 ディレクトリのロールの読み取りや、そのメンバーにする必要があります最初でアクティブにするテナントです。 会社の管理者のディレクトリの役割のみが既定でアクティブにします。 ディレクトリの役割の基になる[directoryRoleTemplate](directoryroletemplate.md)の ID で POST 要求を送信するその他の利用可能なディレクトリの役割をアクティブ化します。 [directoryObject](directoryobject.md) から継承します。
このリソースは以下をサポートしています。

- [デルタ](../api/directoryrole-delta.md)関数を提供することにより、[デルタ クエリ](/graph/delta-query-overview)を使用して、増分の追加、削除、更新を追跡します。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[Get directoryRole](../api/directoryrole-get.md) | [directoryRole](directoryrole.md) | directoryRole オブジェクトのプロパティとリレーションシップを読み取ります。 |
|[directoryRoles を一覧表示する](../api/directoryrole-list.md) | [directoryRole](directoryrole.md) コレクション | テナントでアクティブになっているディレクトリ ロールを一覧表示します。 |
|[メンバーを追加する](../api/directoryrole-post-members.md) |[directoryObject](directoryobject.md)| members ナビゲーション プロパティを送信することで、ユーザーをディレクトリ ロールに追加します。|
|[List members](../api/directoryrole-list-members.md) |[directoryObject](directoryobject.md) コレクション| members ナビゲーション プロパティから、ディレクトリ ロールのメンバーであるユーザーを取得します。|
|[メンバーを削除する](../api/directoryrole-delete-member.md) |[directoryObject](directoryobject.md)| ディレクトリ ロールからユーザーを削除します。|
|[Activate directoryRole](../api/directoryrole-post-directoryroles.md) |[directoryRole](directoryrole.md) | ディレクトリ ロールをアクティブにします。|
|[delta](../api/directoryrole-delta.md)|directoryRole コレクション| ディレクトリの役割の増分の変更を取得します。 |

## <a name="properties"></a>プロパティ
| プロパティ   | 種類 | 説明 |
|:---------------|:--------|:----------|
|説明|String|ディレクトリ ロールの説明。読み取り専用。 |
|displayName|String|ディレクトリ ロールの表示名。読み取り専用。 |
|id|文字列|ディレクトリ ロールの一意識別子。[directoryObject](directoryobject.md) から継承されます。キーであり、Null は許容されません。読み取り専用です。|
|roleTemplateId|String| このロールが基づいている [directoryRoleTemplate](directoryroletemplate.md) の **id**。このプロパティは、POST 操作でテナント内のディレクトリ ロールをアクティブ化するときに指定する必要があります。そのディレクトリ ロールがアクティブ化されると、このプロパティは読み取り専用になります。 |

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型 |説明|
|:---------------|:--------|:----------|
|members|[directoryObject](directoryobject.md) コレクション|このディレクトリ ロールのメンバーであるユーザー。HTTP メソッド: GET、POST、DELETE。読み取り専用。Null 許容型。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [
    "memberOf",
    "members",
    "ownedObjects",
    "owners"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.directoryObject",
  "@odata.type": "microsoft.graph.directoryRole",
  "@odata.annotations": [
    {
      "capabilities": {
        "toppable": false
      }
    }
  ]
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
<!-- {
  "type": "#page.annotation",
  "description": "directoryRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
