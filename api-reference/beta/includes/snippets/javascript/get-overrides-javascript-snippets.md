---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c6a0fc91fa0adbd4aec8036990ca96a1ae3d9670
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35527412"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/inferenceClassification/overrides')
    .version('beta')
    .get();

```