---
title: Microsoft Graph ツールキットの Tasks コンポーネント
description: タスクコンポーネントを使用すると、ユーザーはタスクの表示、追加、削除、完了、または編集を行うことができます。 Microsoft Planner または Microsoft To Do のすべてのタスクで動作します。
localization_priority: Normal
author: benotter
ms.openlocfilehash: 3c2017acd7fe054c71a609c8d908e119e12a590b
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/26/2019
ms.locfileid: "35243052"
---
# <a name="tasks-component-in-the-microsoft-graph-toolkit"></a>Microsoft Graph ツールキットの Tasks コンポーネント

タスクコンポーネントを使用すると、ユーザーはタスクの表示、追加、削除、完了、または編集を行うことができます。 Microsoft Planner または Microsoft のタスクで機能します。

## <a name="example"></a>例

[jsfiddle の例](https://jsfiddle.net/metulev/qhg68m31/)

````html
    <mgt-tasks></mgt-tasks>
````

## <a name="properties"></a>プロパティ

| プロパティ | 属性 | 説明 |
| -- | -- | -- |
| `dataSource` | `data-source="todo/planner"` | タスクのデータソースを設定します。 Microsoft To Do または Microsoft Planner のいずれかです。 既定値は `planner` です。 |
| `readOnly` | `read-only` | タスクのインターフェイスを読み取り専用に設定します (タスクの追加や削除は行われません)。 既定値は `false` です。 |
| `initialId` | `initial-id="planner_id/folder_id"` | 最初に表示されたプランナーまたは folder を指定された ID に設定します。 |
| `initialBucketId` | `initial-bucket-id="bucket_id"` | 最初に表示されるバケット (Planner データソースのみ) を指定された ID に設定します。 |
| `targetId` | `target-id="planner_id/folder_id"` | タスクインターフェイスを、指定したプランナーまたはフォルダー ID にロックします。 |
| `targetBucketId` | `target-bucket-id="bucket_id"` | タスクインターフェイスを、指定されたバケット ID にロックします (Planner データソースのみ)。 |

次に例を示します。

````html
<mgt-tasks read-only initial-id="12345"></mgt-tasks>
````

## <a name="custom-css-variables"></a>カスタム CSS 変数

````css
mgt-tasks {
--tasks-header-padding
--tasks-header-margin 

--tasks-title-padding
--tasks-plan-title-font-size
--tasks-plan-title-padding

--tasks-new-button-width
--tasks-new-button-height
--tasks-new-button-color
--tasks-new-button-background
--tasks-new-button-border
--tasks-new-button-hover-background
--tasks-new-button-active-background

--tasks-new-task-name-margin

--task-margin
--task-box-shadow
--task-background
--task-border

--task-header-color
--task-header-margin

--task-detail-icon-margin

--task-new-margin
--task-new-border
--task-new-line-margin
--tasks-new-line-border
--task-new-input-margin
--task-new-input-padding
--task-new-input-font-size
--task-new-input-active-border
--task-new-select-border

--task-new-add-button-background
--task-new-add-button-disabled-background
--task-new-cancel-button-color

--task-complete-background
--task-complete-border
--task-complete-header-color
--task-complete-detail-color
--task-complete-detail-icon-color
}
````

## <a name="microsoft-graph-permissions"></a>Microsoft Graph のアクセス許可

このコントロールでは、次の Microsoft Graph Api とアクセス許可を使用します。

| リソース | アクセス許可/スコープ |
| - | - |
| プラン/プラン | `Group.Read.All` |
| /planner/plans/$ {id} | `Group.Read.All`, `Group.ReadWrite.All` |
| /プラン | `Group.ReadWrite.All` |
| /Me/Outlook/taskgroups | `Tasks.Read` |
| /Me/Outlook/taskfolders | `Tasks.Read`, `Tasks.ReadWrite` |
| /me/outlook/tasks | `Tasks.ReadWrite` |

Microsoft Planner データソースの場合、フェッチおよび読み取りタスクには、グループの読み取り権限が必要です。 タスクを追加、更新、または削除するには、すべてのアクセス許可が必要です。

Microsoft Todo データソースの場合は、タスクを取得および読み取りするための読み取りアクセス許可が必要です。 タスクを追加、更新、または削除するには、タスクの読み取りアクセス許可が必要です。

## <a name="authentication"></a>認証

タスクコンポーネントは、[認証のドキュメント](./../providers.md)で説明されているグローバル認証プロバイダを使用します。
