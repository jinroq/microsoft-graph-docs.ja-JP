---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: DeleteAction
ms.openlocfilehash: 041552f88561981338fa2ea5719d5af102fb3574
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068983"
---
# <a name="deleteaction-resource-type"></a>DeleteAction リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

[**itemActivity**][activity] に **DeleteAction** リソースがある場合、アクティビティがアイテムを削除したことを示します。

[activity]: itemactivity.md

## <a name="json-representation"></a>JSON 表記

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.deleteAction"
}-->

```json
{
  "name": "string",
  "objectType": "File | Folder"
}
```

## <a name="properties"></a>プロパティ

| プロパティ名 | 型   | 説明
|:--------------|:-------|:----------------------------------------------------
| name          | 文字列 | 削除されたアイテムの名前。
| objectType    | 文字列 | `File`または`Folder`に削除された項目の種類に依存します。

## <a name="remarks"></a>備考

アイテムのアクティビティの記録は、現在、SharePoint と OneDrive for Business でのみ使用できます。

<!-- {
  "type": "#page.annotation",
  "description": "The DeleteAction object provides information about the deletion of an item.",
  "keywords": "activities,activity,action,delete,deletion",
  "section": "documentation",
  "tocPath": "Resources/DeleteAction"
} -->
