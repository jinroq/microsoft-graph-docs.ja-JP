---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActionSet
localization_priority: Normal
ms.openlocfilehash: 194530da1df449d5ba523e084b2e72cd91bbe13d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27873095"
---
# <a name="itemactionset-resource-type"></a>ItemActionSet リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

**ItemActionSet** リソースは、アイテムに対する[アクティビティ][itemActivity]を発生させたアクションに関する情報を提供します。

[itemActivity]: itemactivity.md

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

## <a name="properties"></a>プロパティ

現在使用可能なアクションを次に示します。
将来、新しいアクションがログに記録される可能性があるため、アプリが認識するアクションがなくても、アプリが **itemActionSet** の処理を受け入れることを確認してください。

| プロパティ名 | Type              | 説明
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

## <a name="remarks"></a>備考

アイテムのアクティビティの記録は、現在、SharePoint と OneDrive for Business でのみ使用できます。

<!-- {
  "type": "#page.annotation",
  "description": "The ItemActionSet object provides information about the actions that took place as part of an activity on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/ItemActionSet"
} -->
