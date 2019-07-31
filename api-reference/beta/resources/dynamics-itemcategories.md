---
title: itemCategories リソースの種類
description: Dynamics 365 Business Central のアイテムカテゴリ。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 18017c580637bb53a70b5f7a331ff7be1dc7a07c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972923"
---
# <a name="itemcategories-resource-type"></a>itemCategories リソースの種類
Dynamics 365 Business Central の複数のアイテムのカテゴリを表します。

## <a name="methods"></a>メソッド

| メソッド                                                          | 戻り値の型  |説明             |
|:----------------------------------------------------------------|:-------------|:-----------------------|
|[ItemCategories を取得する](../api/dynamics-itemcategories-get.md)      |itemCategories|アイテムカテゴリを取得します。   |
|[アイテムカテゴリを投稿する](../api/dynamics-create-itemcategories.md)  |itemCategories|アイテムカテゴリを作成します。|
|[Patch itemCategories](../api/dynamics-itemcategories-update.md) |itemCategories|アイテムカテゴリを更新します。|
|[ItemCategories の削除](../api/dynamics-itemcategories-delete.md)|none          |アイテムカテゴリを削除します。|

## <a name="properties"></a>プロパティ
| プロパティ           | 型   |説明                                     |
|:-------------------|:-------|:-----------------------------------------------|
|id                  |GUID    |ItemCategory の一意の ID。 編集できません。|
|code                |string  |ItemCategory コード。                          |
|displayName         |string  |ItemCategories の表示名。                |
|lastModifiedDateTime|datetime|ItemCategory が変更された最後の datetime。 読み取り専用。|  


## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記

ここでは、itemCategories の JSON 表記を示します。

```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "lastModifiedDateTime": "datetime"
}
```

