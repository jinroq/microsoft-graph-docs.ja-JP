---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c18dfdd84198a9acfa5935febe670792f90a8ecf
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35714714"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/usedRange(valuesOnly=true)')
    .get();

```