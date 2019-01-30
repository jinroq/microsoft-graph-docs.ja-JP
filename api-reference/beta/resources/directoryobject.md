---
title: directoryObject リソースの種類
description: Azure Active Directory オブジェクトを表します。**directoryObject** 型は、他の多くのディレクトリ エンティティ型の基本型です。
localization_priority: Priority
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 87fb1c21e2fa1e9788890d97f6afbd0b494c555e
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640568"
---
# <a name="directoryobject-resource-type"></a>directoryObject リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure Active Directory オブジェクトを表します。**directoryObject** 型は、他の多くのディレクトリ エンティティ型の基本型です。

このリソースは以下をサポートしています。

- [デルタ](../api/directoryobject-delta.md)関数を提供することにより、[デルタ クエリ](/graph/delta-query-overview)を使用して、増分の追加、削除、更新を追跡します。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[directoryObject を取得する](../api/directoryobject-get.md) | [directoryObject](directoryobject.md) |ディレクトリ オブジェクトのプロパティを読み取ります。|
|[Delete](../api/directoryobject-delete.md) | なし |ディレクトリ オブジェクトを削除します。 |
|[checkMemberGroups](../api/directoryobject-checkmembergroups.md)|String collection|グループの一覧内のメンバーシップを確認します。チェックは推移的です。|
|[getMemberGroups](../api/directoryobject-getmembergroups.md)|String collection|ユーザー オブジェクト、グループ オブジェクト、またはディレクトリ オブジェクトがメンバーであるすべてのグループを返します。チェックは推移的です。|
|[getMemberObjects](../api/directoryobject-getmemberobjects.md)|String collection| ユーザー オブジェクト、グループ オブジェクト、またはディレクトリ オブジェクトがメンバーであるすべてのグループとディレクトリ ロールを返します。チェックは推移的です。 |
|[getByIds](../api/directoryobject-getbyids.md) | [directoryObject](directoryobject.md) コレクション | 指定された一連の ID に基づいて、一連のディレクトリ オブジェクトを取得します。 |
|[validateProperties](../api/directoryobject-validateproperties.md)|JSON| 名前付けポリシーに準拠した Office 365 グループの表示名またはメール ニックネームを検証します。 |
|[delta](../api/directoryobject-delta.md)|directoryObject コレクション| ディレクトリ オブジェクトの増分の変更を取得します。 派生した型によるフィルター処理をサポートします。 |

## <a name="properties"></a>プロパティ

| プロパティ   | 型 |説明|
|:---------------|:--------|:----------|
|id|String|オブジェクトの一意識別子である Guid。例: 12345678-9abc-def0-1234-56789abcde12。 キー。 null 許容ではありません。 読み取り専用です。|

## <a name="relationships"></a>関係

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
<!--
{
  "type": "#page.annotation",
  "description": "directoryObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/directoryobject.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
