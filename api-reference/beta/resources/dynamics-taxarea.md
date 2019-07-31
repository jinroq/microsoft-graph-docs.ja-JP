---
title: taxAreas リソースの種類
description: 税金エリア
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 09c1c51fed961489d824136f28aaa2f5b3859b44
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972895"
---
# <a name="taxareas-resource-type"></a>taxAreas リソースの種類
Dynamics 365 Business Central の税エリアリソースの種類を表します。

## <a name="methods"></a>メソッド
| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[TaxAreas を取得する](../api/dynamics-taxarea-get.md)|taxAreas|税エリアオブジェクトを取得します。|
|[Post taxAreas](../api/dynamics-create-taxarea.md)|taxAreas|Tax area オブジェクトを作成します。|
|[Patch taxAreas](../api/dynamics-taxarea-update.md)|taxAreas|Tax area オブジェクトを更新します。|
|[TaxAreas の削除](../api/dynamics-taxarea-delete.md)|none|Tax area オブジェクトを削除します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|id|GUID|税エリアの一意の ID です。 編集できません。|
|code|文字列、最大サイズ20| 税エリアのコード。|
|displayName|文字列、最大サイズ50| 税エリアの表示名。|
|taxType|string|税エリアの税タイプ。|
|lastModifiedDateTime|datetime|税エリアが変更された最後の datetime。 読み取り専用。|

## <a name="relationships"></a>リレーションシップ

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。


```json
{
  "id": "GUID",
  "code": "String",
  "displayName": "String",
  "taxType": "String",
  "lastModifiedDateTime": "datetime"
}
```


