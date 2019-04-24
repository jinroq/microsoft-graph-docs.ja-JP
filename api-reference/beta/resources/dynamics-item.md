---
title: アイテムリソースの種類
description: Dynamics 365 Business Central の item オブジェクト。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 42ec7720e2e858f319beab8576fbe57542dd470c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507309"
---
# <a name="items-resource-type"></a>アイテムリソースの種類
Dynamics 365 Business Central のアイテムを表します。

## <a name="methods"></a>メソッド

| メソッド                                      |戻り値の型|説明 |
|:--------------------------------------------|:----------|:-----------|
|[項目を取得する](../api/dynamics-item-get.md)      |items     |アイテムオブジェクトを取得します。   |
|[投稿アイテム](../api/dynamics-create-item.md)  |items     |アイテムオブジェクトを作成します。|
|[Patch 項目](../api/dynamics-item-update.md)  |items     |アイテムオブジェクトを更新します。|
|[アイテムの削除](../api/dynamics-item-delete.md)|なし      |アイテムオブジェクトを削除します。|

## <a name="properties"></a>プロパティ
| プロパティ           | 型 |説明                                          |
|:-------------------|:-------|:----------------------------------------------------|
|id                  |GUID    |アイテムの一意の ID です。 編集できません。             |
|number              |string  |アイテム番号を指定します。                                     |
|displayName         |string  |アイテムの説明を指定します。                 |
|type                |数値 |アイテムの在庫の種類。 1 = 在庫アイテム、2 = サービスアイテム。 これは必須プロパティです。|
|ブロック             |ブール値 |アイテムが検疫状態にあるなどの理由で、アイテムのトランザクションを投稿できないことを指定します。 アイテムがブロックされている場合は**true**に設定します。|
|baseunitofmeasureid |GUID    |測定単位の ID を指定します。             |
|baseunitofmeasure   |[ナビゲーション.unitofmeasure](../resources/dynamics-complextypes.md)|品目が在庫に保持される単位を指定します。|
|gtin                |数値 |これは、グローバルな取引項目番号です。                |
|itemcategoryid      |GUID |アイテムが属するカテゴリを指定します。 アイテムカテゴリには、割り当てられたアイテム属性も含まれます。|
|inventory           |decimal |アイテムの、在庫にある、断片、箱、缶などの単位数を指定します。 読み取り専用です。|
|販売           |decimal |指定した通貨でのアイテムの1単位の価格を指定します。|
|priceIncludesTax    |ブール値 |unitPrice に税が含まれることを指定します。 unitPrice に tax が含まれる場合は**true**に設定します。|
|unitCost            |decimal |アイテムの単位あたりのコストを指定します。             |
|taxGroupId          |GUID    |アイテムの税グループの ID を指定します。      |
|taxGroupCode        |数値 |税グループは、同一の税用語の対象となる在庫品目またはリソースのグループを表します。|
|lastModifiedDateTime|datetime|アイテムが最後に変更された datetime。 読み取り専用。  |  


## <a name="relationships"></a>リレーションシップ
税グループ (taxGroupCode) は、税グループテーブルに存在する必要があります。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。


```json
{
      "id": "GUID",
      "number": "string",
      "displayName": "string",
      "type": "string",
      "blocked": "boolean",
      "baseUnitOfMeasureId": "GUID",
      "baseUnitOfMeasure": "NAV.UnitOfMeasure",
      "gtin": "numeric",
      "itemCategoryId": "GUID",
      "inventory": "decimal",
      "unitPrice": "decimal",
      "priceIncludesTax": "boolean",
      "unitCost": "decimal",
      "taxGroupId": "GUID",
      "taxGroupCode": "string",
      "lastModifiedDateTime": "datetime"
}

```


