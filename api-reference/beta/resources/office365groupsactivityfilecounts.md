---
title: office365GroupsActivityFileCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: adff009d9047aa147c8042059fbdab8491288fb7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972559"
---
# <a name="office365groupsactivityfilecounts-resource-type"></a>office365GroupsActivityFileCounts リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ          | 種類   | 説明                              |
| :---------------- | :----- | ---------------------------------------- |
| reportRefreshDate | 日付   | コンテンツの最新の日付。          |
| total             | Int64  | グループの SharePoint ドキュメント ライブラリ内のファイルの合計数です。 |
| アクティブです            | Int64  | 、表示されたファイルの数は、編集、共有、またはグループの SharePoint ドキュメント ライブラリに同期します。 |
| reportDate        | 日付   | グループの SharePoint サイトにアクティブだったファイルの数の日付です。 |
| reportPeriod      | String | レポートの対象日数です。    |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {

  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365GroupsActivityFileCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "total": 1024, 
  "active": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
