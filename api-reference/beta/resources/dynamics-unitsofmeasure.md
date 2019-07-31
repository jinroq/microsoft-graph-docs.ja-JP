---
title: unitsOfMeasure リソースの種類
description: Dynamics 365 Business Central の測定単位オブジェクト。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 3658c4c510194d3cc950094ec9e46db31589bc03
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972867"
---
# <a name="unitsofmeasure-resource-type"></a>unitsOfMeasure リソースの種類
Dynamics 365 Business Central の、数量の標準測定基準である測定単位を表します。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[UnitsOfMeasure を取得する](../api/dynamics-unitsofmeasure-get.md)|unitsOfMeasure|測定単位オブジェクトを取得します。|
|[Post unitsOfMeasure](../api/dynamics-create-unitsofmeasure.md)|unitsOfMeasure|測定単位オブジェクトを作成します。|
|[Patch unitsOfMeasure](../api/dynamics-unitsofmeasure-update.md)|unitsOfMeasure|測定単位オブジェクトを更新します。|
|[UnitsOfMeasure の削除](../api/dynamics-unitsofmeasure-delete.md)|none|測定単位オブジェクトを削除します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|id|GUID|UnitsOfMeasure の一意の ID。 編集できません。|
|code|string|測定単位のコードを指定します。|
|displayName|string|測定単位の表示名を指定します。|
|internationalStandardCode|string|営業ドキュメントの電子送信に関連して、UNECE Rec20 standard に従って表される測定単位コードの単位を指定します。|
|lastModifiedDateTime|datetime|測定単位が変更された最後の datetime。 読み取り専用。|  


## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記

ここでは、 **unitsOfMeasure**リソースの JSON 表記を示します。

```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "internationalStandardCode": "string",
  "lastModifiedDateTime": "datetime"
}

```
