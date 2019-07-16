---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8a4df57dac0991a176e810541ae613e611ddcad3
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35740579"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/root/workbook/worksheets/{id}/range/rowsBelow(count=2)')
    .post();

```