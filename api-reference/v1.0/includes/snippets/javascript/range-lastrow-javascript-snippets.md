---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 7f3b60f6d3d9a5f3eff155a3b3589f1a6f8bb9d3
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35733929"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/lastRow')
    .get();

```