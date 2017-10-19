---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SpecialFolder
ms.openlocfilehash: 84e67df8aae6e72363d4ba148e92f9046f41bb29
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/28/2017
---
# <a name="specialfolder-resource-type"></a>SpecialFolder リソース型

**SpecialFolder** リソースは、特殊フォルダー関連のデータ項目を単一の構造にグループ化します。

**DriveItem** が null 以外の **specialFolder** ファセットを持つ場合、その項目は特殊な (名前が付けられた) フォルダーを示します。
特殊なフォルダーは [特殊なフォルダーのコレクション](../api/drive_get_specialfolder.md) 経由で直接アクセスできます。

特殊なフォルダーは、フォルダーを (ローカライズが必要となる) パスで探したり、ID を持つフォルダーを参照したりせずに、既知のフォルダーにアクセスするための、単純なエイリアスを提供します。特殊なフォルダーが名前変更されたりドライブ内の別の場所に移動されたりした場合、この構文はそのフォルダーを返し続けます。

特殊なフォルダーは、まだ存在していない場合、アプリケーションが最初に書き込みを試行したときに自動的に作成されます。ユーザーが削除した場合は、もう一度書き込まれたときに再作成されます。

**注:** アプリが **Files.Read** スコープのみを要求していて、存在しない特殊なフォルダーを要求する場合、返答は `403 Forbidden` エラーになります。

## <a name="json-representation"></a>JSON 表記

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.specialFolder"
}-->
```json
{
  "name": "string"
}
```

## <a name="properties"></a>プロパティ

| プロパティ  | 型   | 説明                                                            |
|:----------|:-------|:-----------------------------------------------------------------------|
| name      | string | `/drive/special` コレクション内のこの項目の一意識別子 |

## <a name="special-folders"></a>特殊なフォルダー

以下は OneDrive Personal および OneDrive for Business で利用可能な特殊なフォルダーです。

| 名前        | フォルダー ID    | 説明                                                              |
|:------------|:-------------|:-------------------------------------------------------------------------|
| App Root    | `approot`    | そのアプリケーションの個人用フォルダー。通常は `/Apps/{Application Name}` 内 |
| Camera Roll | `cameraroll` | カメラ ロールのバックアップ フォルダー。OneDrive for Business では利用不可です。   |
| ドキュメント   | `documents`  | ドキュメント フォルダーです。                                                    |
| Music       | `music`      | ミュージック フォルダーです。OneDrive for Business では利用不可です。                |
| Photos      | `photos`     | フォト フォルダーです。                                                       |

## <a name="remarks"></a>備考 

DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。

<!-- {
  "type": "#page.annotation",
  "description": "The SpecialFolder facet provides information about folders accessible as special folders.",
  "keywords": "special folder,item,facet",
  "section": "documentation",
  "tocPath": "Facets/SpecialFolder"
} -->
