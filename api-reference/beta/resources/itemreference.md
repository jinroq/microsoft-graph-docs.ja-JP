---
author: JeremyKelley
description: ItemReference リソースは、DriveItem を処理するために必要な情報を API を介して提供します。
ms.date: 09/10/2017
title: ItemReference
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 434e3ed1da1f7536224e27b619cedf3bbef5f20e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967064"
---
# <a name="itemreference-resource-type"></a>ItemReference リソースの種類

**ItemReference** リソースは、[DriveItem](driveitem.md) を処理するために必要な情報を API を介して提供します。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "path", "shareId", "sharepointIds" ],
  "@odata.type": "microsoft.graph.itemReference"
}-->

```json
{
  "driveId": "string",
  "driveType": "personal | business | documentLibrary",
  "id": "string",
  "name": "string",
  "path": "string",
  "shareId": "string",
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" }
}
```

## <a name="properties"></a>プロパティ

| プロパティ      | 型              | 説明
|:--------------|:------------------|:-----------------------------------------
| driveId       | String            | アイテムを含むドライブ インスタンスの一意識別子。読み取り専用です。
| driveType     | String            | ドライブの種類を表します。 値については [drive][] リソースを参照してください。
| id            | 文字列            | ドライブ内のアイテムの一意識別子。読み取り専用です。
| name          | String            | 参照中のアイテムの名前。読み取り専用です。
| path          | String            | アイテムへの移動に使用可能なパス。読み取り専用です。
| shareId       | String            | [共有][] API 経由でアクセスできる共有リソースの一意識別子。
| sharepointIds | [sharepointIds][] | SharePoint REST 互換性に役立つ識別子を返します。読み取り専用です。

[drive]: ../resources/drive.md
[sharepointIds]: ../resources/sharepointids.md
[共有]: ../api/shares-get.md

## <a name="remarks"></a>備考

**itemReference** リソースからの **driveItem** を処理するには、次の形式の URL を構築します。

```http
GET https://graph.microsoft.com/v1.0/drives/{driveId}/items/{id}
```

**path** の値は、対象ドライブを基準にした API パスです。例: `/drive/root:/Documents/myfile.docx`。

階層リンクの人が認識できるパスを取得するために、パスの文字列内にある最初の `:` までのすべてを無視しても問題ありません。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ItemReference returns a pointer to another item.",
  "section": "documentation",
  "tocPath": "Resources/ItemReference"
} -->
