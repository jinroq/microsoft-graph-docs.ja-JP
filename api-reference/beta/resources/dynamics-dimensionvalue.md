---
title: dimensionvalues リソースの種類
description: Dynamics 365 Business Central の寸法値。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: da3935b8e784b05551af123c1832d5dc84a2c81c
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365319"
---
# <a name="dimensionvalues-resource-type"></a>dimensionvalues リソースの種類
Dynamics 365 Business Central のディメンション値を表します。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明                   |
|:-------------|:-------------|:-----------------------------|
|[dimensionvalues の値を取得する](../api/dynamics-dimensionvalue-get.md)|dimensionvalues|ディメンション値オブジェクトを取得します。|


## <a name="properties"></a>プロパティ
| プロパティ           | 型                  |説明                                        |
|:-------------------|:----------------------|:--------------------------------------------------|
|ID                  |GUID                   |アイテムの一意の ID です。                         |
|code                |文字列、最大サイズ20|寸法値コード。                          |
|displayName         |string                 |次元の値の名前を指定します。 この名前は、ディメンション値が使用される場所に表示されます。|
|lastModifiedDateTime|datetime               |ディメンション値が変更された最後の datetime。|  


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。


```json
{

    "id": "GUID",
    "code": "string",
    "displayName": "string",
    "lastModifiedDateTime": "datetime"
}
```


