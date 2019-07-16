---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c193c8d3db8c0b66ca0ab9bcd0fe9e8ff037b9c6
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35738864"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}')
    .get();

```