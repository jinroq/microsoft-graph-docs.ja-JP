---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 2f4f8dbf4a0ab46530cce24a0d12ed5f396c4973
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35724878"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/convertToRange')
    .version('beta')
    .post();

```