---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 302589e969e46ba0912f1e305ee4cdf5ce9490e1
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35464594"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const agreement = {
  displayName: "MSGraph Sample",
  isViewingBeforeAcceptanceRequired: true,
  files: [
    {
      fileName: "TOU.pdf",
      language: "en",
      isDefault: true,
      fileData: {
        data: "SGVsbG8gd29ybGQ="
      }
    }
  ]
};

let res = await client.api('/agreements')
    .version('beta')
    .post({agreement : agreement});

```