---
title: itemcategories リソースの種類
description: Dynamics 365 Business Central のアイテムカテゴリ。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: e18319683f6dbceddccc9cf83e48cd3ef89f895d
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365746"
---
# <a name="itemcategories-resource-type"></a>itemcategories リソースの種類
Dynamics 365 Business Central の複数のアイテムのカテゴリを表します。

## <a name="methods"></a>メソッド

| メソッド                                                          | 戻り値の型  |説明             |
|:----------------------------------------------------------------|:-------------|:-----------------------|
|[itemcategories を取得する](../api/dynamics-itemcategories-get.md)      |itemcategories|アイテムカテゴリを取得します。   |
|[アイテムカテゴリを投稿する](../api/dynamics-create-itemcategories.md)  |itemcategories|アイテムカテゴリを作成します。|
|[Patch itemcategories](../api/dynamics-itemcategories-update.md) |itemcategories|アイテムカテゴリを更新します。|
|[itemcategories の削除](../api/dynamics-itemcategories-delete.md)|none          |アイテムカテゴリを削除します。|

## <a name="properties"></a>プロパティ
| プロパティ           | 型   |説明                                     |
|:-------------------|:-------|:-----------------------------------------------|
|ID                  |GUID    |itemcategory の一意の ID。 編集不可。|
|code                |文字列  |itemcategory コード。                          |
|displayName         |string  |itemcategories の表示名。                |
|lastModifiedDateTime|datetime|itemcategory が変更された最後の datetime。 読み取り専用です。|  


## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記

ここでは、itemcategories の JSON 表記を示します。

```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "lastModifiedDateTime": "datetime"
}
```

