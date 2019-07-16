---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8bfb7bdf55d666a55d7f7576ca9616c481007f46
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35740860"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/inferenceClassification/overrides')
    .get();

```