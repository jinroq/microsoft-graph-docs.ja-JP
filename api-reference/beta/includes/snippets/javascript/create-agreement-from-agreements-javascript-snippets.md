---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 81297af4879ae96719d7e83922bf84231f4b0e46
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/27/2019
ms.locfileid: "36637857"
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
    .post(agreement);

```