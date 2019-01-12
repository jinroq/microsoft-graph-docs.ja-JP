---
title: directoryRole リソース型
description: Azure AD ディレクトリの役割を表します。 Azure AD ディレクトリの役割は、*管理者の役割*とも呼ばれます。 ディレクトリ (管理者) の役割の詳細については、Azure AD の管理者の役割の割り当てを参照してください。 Graph とには、ターゲットのロールのアクセス許可を付与するディレクトリのロールにユーザーを割り当てることができます。 ディレクトリのロールの読み取りや、そのメンバーにする必要があります最初でアクティブにするテナントです。 会社の管理者のディレクトリの役割のみが既定でアクティブにします。 その他の利用可能なディレクトリの役割を有効にするのにはディレクトリの役割の基になる directoryRoleTemplate の ID で POST 要求を送信します。 directoryObject から継承します。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e6753369be070ab04419cab0c870aec7e96b1fb2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27927745"
---
# <a name="directoryrole-resource-type"></a>directoryRole リソース型

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

Azure AD ディレクトリの役割を表します。 Azure AD ディレクトリの役割は、*管理者の役割*とも呼ばれます。 ディレクトリ (管理者) の役割の詳細については、 [Azure AD の管理者ロールの割り当て](https://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/)を参照してください。 Graph とには、ターゲットのロールのアクセス許可を付与するディレクトリのロールにユーザーを割り当てることができます。 ディレクトリのロールの読み取りや、そのメンバーにする必要があります最初でアクティブにするテナントです。 会社の管理者のディレクトリの役割のみが既定でアクティブにします。 その他の利用可能なディレクトリの役割を有効にするのにはディレクトリの役割の基になる[directoryRoleTemplate](directoryroletemplate.md)の ID で POST 要求を送信します。 [directoryObject](directoryobject.md) から継承します。

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
|[スコープ ロールのメンバーの一覧](../api/directoryrole-list-members.md) |[scopedRoleMembership](scopedrolemembership.md) コレクション| スコープは、[管理単位](administrativeunit.md)、scopedRoleMembership リソースのコレクションをこのディレクトリのロールのメンバーを一覧表示します。|
|[delta](../api/directoryrole-delta.md)|directoryRole コレクション| ディレクトリの役割の増分の変更を取得します。 |

## <a name="properties"></a>プロパティ
| プロパティ   | 種類 |説明|
|:---------------|:--------|:----------|
|説明|String|ディレクトリ ロールの説明。読み取り専用。 |
|displayName|String|ディレクトリ ロールの表示名。読み取り専用。 |
|id|文字列|ディレクトリ ロールの一意識別子。[directoryObject](directoryobject.md) から継承されます。キーであり、Null は許容されません。読み取り専用です。|
|roleTemplateId|String| このロールが基づいている [directoryRoleTemplate](directoryroletemplate.md) の **id**。このプロパティは、POST 操作でテナント内のディレクトリ ロールをアクティブ化するときに指定する必要があります。そのディレクトリ ロールがアクティブ化されると、このプロパティは読み取り専用になります。 |

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型 |説明|
|:---------------|:--------|:----------|
|members|[directoryObject](directoryobject.md) コレクション|このディレクトリ ロールのメンバーであるユーザー。HTTP メソッド: GET、POST、DELETE。読み取り専用。Null 許容型。|
|scopedMembers|[scopedRoleMembership](scopedrolemembership.md) コレクション| [管理単位](administrativeunit.md)のスコープはこのディレクトリのロールのメンバーです。 読み取り専用です。 Null 許容型。|

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
<!-- {
  "type": "#page.annotation",
  "description": "directoryRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
