---
author: daspek
ms.author: dspektor
title: ItemActionSet リソースの種類
description: ItemActionSet オブジェクトは、アイテムのアクティビティの一部として行われたアクションに関する情報を提供します。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 065a6126e2e4a2f78cecfb2ae5497fac28e16899
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970759"
---
# <a name="itemactionset-resource-type"></a>itemActionSet リソースの種類

**Itemactionset**リソースは、アイテムの[アクティビティ][ itemActivity]を構成したアクションに関する情報を提供します。

>**注:** 現時点では、アイテムアクティビティレコードは SharePoint および OneDrive for business でのみ使用できます。

[itemActivity]: itemactivity.md

## <a name="properties"></a>プロパティ

現在、次の操作を実行できます。 今後、新しいアクションが追加される可能性があるため、アプリが不明なアクションを含む**Itemactionset**を処理できることを確認してください。

| プロパティ名 | 種類              | 説明
|:--------------|:------------------|:-----------------------------------------
| comment       | [commentAction][] | アイテムにコメントが追加されました。
| create        | [createAction][]  | アイテムが作成されました。
| delete        | [deleteAction][]  | アイテムが削除されました。
| edit          | [editAction][]    | アイテムが編集されました。
| mention       | [mentionAction][] | アイテムでユーザーがメンションされました。
| move          | [moveAction][]    | アイテムが移動されました。
| rename        | [renameAction][]  | アイテムの名前が変更されました。
| restore       | [restoreAction][] | アイテムが復元されました。
| share         | [shareAction][]   | アイテムが共有されました。
| version       | [versionAction][] | アイテムのバージョンが更新されました。

[commentAction]: commentaction.md
[createAction]: createaction.md
[deleteAction]: deleteaction.md
[editAction]: editaction.md
[mentionAction]: mentionaction.md
[moveAction]: moveaction.md
[renameAction]: renameaction.md
[restoreAction]: restoreaction.md
[shareAction]: shareaction.md
[versionAction]: versionaction.md

## <a name="json-representation"></a>JSON 表記

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "keyProperty": "id",
  "@type": "microsoft.graph.itemActionSet",
  "@type.aka": "oneDrive.action"
}-->

```json
{
  "comment": {"@odata.type": "microsoft.graph.commentAction"},
  "create": {"@odata.type": "microsoft.graph.createAction"},
  "delete": {"@odata.type": "microsoft.graph.deleteAction"},
  "edit": {"@odata.type": "microsoft.graph.editAction"},
  "mention": {"@odata.type": "microsoft.graph.mentionAction"},
  "move": {"@odata.type": "microsoft.graph.moveAction"},
  "rename": {"@odata.type": "microsoft.graph.renameAction"},
  "restore": {"@odata.type": "microsoft.graph.restoreAction"},
  "share": {"@odata.type": "microsoft.graph.shareAction"},
  "version": {"@odata.type": "microsoft.graph.versionAction"},
  
}
```

<!--
{
  "type": "#page.annotation",
  "description": "The itemActionSet object provides information about the actions that took place as part of an activity on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/itemActionSet",
  "suppressions": []
}
-->
