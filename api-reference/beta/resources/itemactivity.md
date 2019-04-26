---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActivity
localization_priority: Normal
ms.openlocfilehash: 5e2be549c3e3e9e799449679b605577ecd782a94
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561888"
---
# <a name="itemactivity-resource-type"></a>ItemActivity リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**ItemActivity** リソースは、アイテムまたはコンテナー内で発生したアクティビティについての情報を提供します。
現在、SharePoint と OneDrive for Business でのみ使用できます。

## <a name="json-representation"></a>JSON 表記

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "keyProperty": "id",
  "@type": "microsoft.graph.itemActivity",
  "@type.aka": "oneDrive.activityEntity"
}-->

```json
{
  "id": "string (identifier)",
  "access": "microsoft.graph.accessAction",
  "action": {"@odata.type": "microsoft.graph.itemActionSet"},
  "actor": {"@odata.type": "microsoft.graph.identitySet"},
  "driveItem": {"@odata.type": "microsoft.graph.driveItem"},
  "listItem": {"@odata.type": "microsoft.graph.listItem"},
  "location": {"@odata.type": "microsoft.graph.location"},
  "times": {"@odata.type": "microsoft.graph.itemActivityTimeSet"}
}
```

## <a name="properties"></a>プロパティ

| プロパティ | 型                    | 説明
|:---------|:------------------------|:----------------------------------------
| id       | string                  | アクティビティの一意識別子。 読み取り専用です。
| 接続   | [accessaction][]        | アイテムがアクセスされました。
| action   | [itemActionSet][]       | 発生したアクションについての詳細。 読み取り専用です。
| actor    | [identitySet][]         | アクションを実行したユーザーの識別情報。 読み取り専用です。
| location | [location][]            | アクションが実行された物理的な場所。 読み取り専用です。
| times    | [itemActivityTimeSet][] | アクティビティがいつ発生したかについての詳細。 読み取り専用です。

[identitySet]: identityset.md
[itemActionSet]: itemactionset.md
[itemActivityTimeSet]: itemactivitytimeset.md

## <a name="relationships"></a>リレーションシップ

| リレーションシップ名 | 種類          | 説明
|:------------------|:--------------|:-----------------------------------------
| driveItem         | [driveItem][] | このアクティビティのターゲットとなった **driveItem** を表します。
| listItem          | [listItem][]  | このアクティビティのターゲットとなった **listItem** を表します。

[driveItem]: driveitem.md
[listItem]: listitem.md

## <a name="actions"></a>アクション

アクティビティ内で発生したアクションについては、**action** プロパティで詳しく記述されます。
現在使用可能なアクションを次に示します。
将来、新しいアクションがログに記録される可能性があるため、アプリが認識するアクションがなくても、アプリが **itemActivity** の処理を受け入れることを確認してください。

| アクション名 | 型              | 説明
|:------------|:------------------|:-------------------------------------------
| comment     | [commentAction][] | アイテムにコメントが追加されました。
| create      | [createAction][]  | アイテムが作成されました。
| delete      | [deleteAction][]  | アイテムが削除されました。
| edit        | [editAction][]    | アイテムが編集されました。
| mention     | [mentionAction][] | アイテムでユーザーがメンションされました。
| move        | [moveAction][]    | アイテムが移動されました。
| rename      | [renameAction][]  | アイテムの名前が変更されました。
| restore     | [restoreAction][] | アイテムが復元されました。
| share       | [shareAction][]   | アイテムが共有されました。
| version     | [versionAction][] | アイテムのバージョンが更新されました。

[accessaction]: accessaction.md
[commentAction]: commentaction.md
[createAction]: createaction.md
[deleteAction]: deleteaction.md
[editAction]: editaction.md
[location]: location.md
[mentionAction]: mentionaction.md
[moveAction]: moveaction.md
[renameAction]: renameaction.md
[restoreAction]: restoreaction.md
[shareAction]: shareaction.md
[versionAction]: versionaction.md

## <a name="remarks"></a>備考

現在、**ItemActivity** は SharePoint と OneDrive for Business でのみ使用できます。

<!--
{
  "type": "#page.annotation",
  "description": "The ItemActivity object provides information about an activity that took place on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/ItemActivity",
  "suppressions": []
}
-->
