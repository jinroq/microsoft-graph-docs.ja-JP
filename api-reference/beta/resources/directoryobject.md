---
title: directoryObject リソースの種類
description: Azure Active Directory オブジェクトを表します。**directoryObject** 型は、他の多くのディレクトリ エンティティ型の基本型です。
localization_priority: Priority
ms.openlocfilehash: a03ec966f966df556ab0122958b0b8f5464cf4fc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889720"
---
# <a name="directoryobject-resource-type"></a>directoryObject リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

Azure Active Directory オブジェクトを表します。**directoryObject** 型は、他の多くのディレクトリ エンティティ型の基本型です。

このリソースは以下をサポートしています。

- [デルタ](../api/directoryobject-delta.md)関数を提供することにより、[デルタ クエリ](/graph/delta-query-overview)を使用して、増分の追加、削除、更新を追跡します。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[directoryObject を取得する](../api/directoryobject-get.md) | [directoryObject](directoryobject.md) |ディレクトリ オブジェクトのプロパティを読み取ります。|
|[Delete](../api/directoryobject-delete.md) | なし |ディレクトリ オブジェクトを削除します。 |
|[checkMemberGroups](../api/directoryobject-checkmembergroups.md)|String コレクション|グループの一覧内のメンバーシップを確認します。チェックは推移的です。|
|[getMemberGroups](../api/directoryobject-getmembergroups.md)|String コレクション|ユーザー オブジェクト、グループ オブジェクト、またはディレクトリ オブジェクトがメンバーであるすべてのグループを返します。チェックは推移的です。|
|[getMemberObjects](../api/directoryobject-getmemberobjects.md)|String コレクション| ユーザー オブジェクト、グループ オブジェクト、またはディレクトリ オブジェクトがメンバーであるすべてのグループとディレクトリ ロールを返します。チェックは推移的です。 |
|[getByIds](../api/directoryobject-getbyids.md) | [directoryObject](directoryobject.md) コレクション | 指定された一連の ID に基づいて、一連のディレクトリ オブジェクトを取得します。 |
|[validateProperties](../api/directoryobject-validateproperties.md)|JSON| メールのニックネームは、命名ポリシーに準拠しているまたは、Office 365 のグループの表示名を検証します。 |
|[delta](../api/directoryobject-delta.md)|directoryObject コレクション| ディレクトリ オブジェクトに対して増分の変更を取得します。 Derrived の種類でフィルター処理をサポートします。 |

## <a name="properties"></a>プロパティ

| プロパティ   | 種類 |説明|
|:---------------|:--------|:----------|
|ID|String|オブジェクトの一意の識別子である Guidたとえば、12345678-9abc-def0-1234-56789abcde12 です。 キー。 null 許容ではありません。 読み取り専用です。|

## <a name="relationships"></a>リレーションシップ

なし

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directoryObject"
}-->

```json
{
  "id": "string (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
