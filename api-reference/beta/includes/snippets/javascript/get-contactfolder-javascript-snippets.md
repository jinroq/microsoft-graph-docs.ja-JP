---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 87d172bda4c1dd797860ed13647f0ed0ddf39c64
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35707475"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/contactFolders/{id}')
    .version('beta')
    .get();

```