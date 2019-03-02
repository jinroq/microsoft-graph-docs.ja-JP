---
title: 複合型 JSON
description: Dynamics 365 Business Central 用の JSON の複雑なデータ型。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 4fc4d4f53014f5b8c656cd069cadf7b19190e0f0
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366768"
---
# <a name="complex-types-json"></a>複合型 JSON
これらは、Dynamics 365 Business Central のさまざまな複合型です。 これらの複合型の使用方法は、それらを利用するさまざまな個別のメソッドで確認できます。

## <a name="postal-address"></a>郵送先住所

Dynamics 365 Business Central の郵送先住所の複合型を表します。

### <a name="properties"></a>プロパティ
| プロパティ     | 型       |説明             |
|:-------------|:---------|:-----------------------|
|street        |string    |郵送先住所  |
|city          |string    |市町村 (郵送先)    |
|state         |string    |都道府県 (郵送先住所)   |
|countryLetterCode|string |郵送先住所の文字コード (2 文字の単語)|
|postalCode    |string    |郵便アドレスの post コード|

```json
"PostalAddress" 
{ 
"street": "string",
"city": "string", 
"state": "string", 
"countryLetterCode": "string", 
"postalCode": "string" 
} 
 ```

