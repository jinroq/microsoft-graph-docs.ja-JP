---
title: directoryObject リソースの種類
description: Azure Active Directory オブジェクトを表します。**directoryObject** 型は、他の多くのディレクトリ エンティティ型の基本型です。
localization_priority: Priority
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: da596d80bee17e55f8ecffe8f212e686af8e30d7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27964138"
---
# <a name="directoryobject-resource-type"></a>directoryObject リソースの種類

Azure Active Directory オブジェクトを表します。**directoryObject** 型は、他の多くのディレクトリ エンティティ型の基本型です。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[directoryObject を取得する](../api/directoryobject-get.md) | [directoryObject](directoryobject.md) |ディレクトリ オブジェクトのプロパティを読み取ります。|
|[directoryObject を削除する](../api/directoryobject-delete.md) | なし |ディレクトリ オブジェクトを削除します。 |
|[checkMemberGroups](../api/directoryobject-checkmembergroups.md)|String コレクション|グループの一覧内のメンバーシップを確認します。チェックは推移的です。|
|[getMemberGroups](../api/directoryobject-getmembergroups.md)|String コレクション|ユーザー オブジェクト、グループ オブジェクト、またはディレクトリ オブジェクトがメンバーであるすべてのグループを返します。チェックは推移的です。|
|[getMemberObjects](../api/directoryobject-getmemberobjects.md)|String コレクション| ユーザー オブジェクト、グループ オブジェクト、またはディレクトリ オブジェクトがメンバーであるすべてのグループとディレクトリ ロールを返します。チェックは推移的です。 |
|[getByIds](../api/directoryobject-getbyids.md) | [directoryObject](directoryobject.md) コレクション | 指定された一連の ID に基づいて、一連のディレクトリ オブジェクトを取得します。 |

## <a name="properties"></a>プロパティ

| プロパティ   | 種類 |説明|
|:---------------|:--------|:----------|
|ID|String|オブジェクトの一意識別子である Guid。例: 12345678-9abc-def0-1234-56789abcde。キー。null 許容ではありません。読み取り専用です。|

## <a name="relationships"></a>リレーションシップ

なし


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.directoryObject",
  "@odata.annotations": [
    {
      "capabilities": {
        "skippable": false,
        "countable": false,
        "expandable": false,
        "filterable": false,
        "referenceable": false,
        "selectable": false
      }
    }
  ]
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
