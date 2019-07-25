---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c994f0260f61a4bf213b34b063d5c208cd2cb63f
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35728749"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/onenote/pages/{id}')
    .version('beta')
    .delete();

```