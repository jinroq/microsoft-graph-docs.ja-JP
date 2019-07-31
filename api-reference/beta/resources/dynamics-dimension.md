---
title: dimensions リソースの種類
description: Dynamics 365 Business Central のディメンション。
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 5bd5382ae020baaf726db53f9252c4d3498833ee
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973626"
---
# <a name="dimensions-resource-type"></a>Dimensions リソースの種類
Dynamics 365 Business Central のディメンションを表します。

## <a name="methods"></a>メソッド
| メソッド       | 戻り値の型  |説明|
|:-------------|:-------------|:----------|
|[ディメンションを取得する](../api/dynamics-dimension-get.md)|大きさ|次元を取得します。|


## <a name="properties"></a>プロパティ
| プロパティ           | 型                  |説明               |
|:-------------------|:----------------------|:-------------------------|
|id                  |GUID                   |アイテムの一意の ID です。|
|code                |文字列、最大サイズ20|次元コード。       |
|displayName         |string                 |ディメンションの名前を指定します。 この名前は、ディメンションが使用される場所に表示されます。|
|lastModifiedDateTime|datetime               |ディメンションが変更された最後の datetime。|  


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

