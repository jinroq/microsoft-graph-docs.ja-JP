---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8bfb7bdf55d666a55d7f7576ca9616c481007f46
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35472340"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/inferenceClassification/overrides')
    .get();

```