---
title: dimensions リソースの種類
description: Dynamics 365 Business Central のディメンション。
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 92ba48a7ad55b6a7dff28ccc1547769c149e378b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543089"
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

