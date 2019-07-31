---
title: 複合型 JSON
description: Dynamics 365 Business Central 用の JSON の複雑なデータ型。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: bb61450ab7f1d62d459f525f6341093f25b1686f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012640"
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

