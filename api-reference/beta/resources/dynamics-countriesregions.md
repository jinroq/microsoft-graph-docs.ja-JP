---
title: countriesRegions リソースの種類
description: Dynamics 365 Business Central の国/地域オブジェクト。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: b6f50ba3046a402f2b8729529675653286808459
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365487"
---
# <a name="countriesregions-resource-type"></a>countriesRegions リソースの種類
countriesRegions オブジェクトを Dynamics 365 Business Central で表します。これは、アドレスの一部です。

## <a name="methods"></a>メソッド

| メソッド                                                              | 戻り値の型    |説明                |
|:--------------------------------------------------------------------|:---------------|:--------------------------|
|[countriesRegions を取得する](../api/dynamics-countriesregions-get.md)      |countriesRegions|国/地域を取得します。   |
|[Post countriesRegions](../api/dynamics-create-countriesregions.md)  |countriesRegions|国/地域を作成します。|
|[Patch countriesRegions](../api/dynamics-countriesregions-update.md) |countriesRegions|国/地域を更新します。|
|[countriesRegions の削除](../api/dynamics-countriesregions-delete.md)|none            |国/地域を削除します。|

## <a name="properties"></a>プロパティ
| プロパティ       | 型       |説明                                                  |
|:---------------|:-----------|:------------------------------------------------------------|
|ID              |GUID        |国/地域の一意の ID。 編集不可。           |
|code            |文字列      |国/地域のコードを指定します。                    |
|displayName     |string      |国/地域の表示名を指定します。            |
|addressformat   |string      |外部向けドキュメントに表示されるアドレスの形式を指定します。 住所形式を国/地域コードにリンクして、その国/地域コードを含むカードまたはドキュメントに基づく外部向けのドキュメントで、指定されたアドレス形式を使用するようにします。|
|lastModifiedDateTime|datetime|国/地域が変更された最後の datetime。 読み取り専用です。|  


## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記

countriesRegions の JSON 表記を次に示します。


```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "addressFormat": "string",
  "lastModifiedDateTime": "datetime"
}

```


