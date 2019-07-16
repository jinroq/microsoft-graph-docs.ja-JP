---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: be82bda0d060953968f01cd153c3e41a4ab06b59
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35740581"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/root/workbook/worksheets/{id}/range/rowsBelow')
    .get();

```