---
title: dimensionValues リソースの種類
description: Dynamics 365 Business Central の寸法値。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: af7ba3b49051a4e89fcdf2a4a408a1f72fc547ad
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973616"
---
# <a name="dimensionvalues-resource-type"></a>dimensionValues リソースの種類
Dynamics 365 Business Central のディメンション値を表します。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明                   |
|:-------------|:-------------|:-----------------------------|
|[DimensionValues の値を取得する](../api/dynamics-dimensionvalue-get.md)|dimensionValues|ディメンション値オブジェクトを取得します。|


## <a name="properties"></a>プロパティ
| プロパティ           | 型                  |説明                                        |
|:-------------------|:----------------------|:--------------------------------------------------|
|id                  |GUID                   |アイテムの一意の ID です。                         |
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


