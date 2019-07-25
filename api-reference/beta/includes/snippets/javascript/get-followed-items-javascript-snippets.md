---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b903c65608c5b61d0c148cdb753a95683dbcd90a
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35706221"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/following')
    .version('beta')
    .get();

```