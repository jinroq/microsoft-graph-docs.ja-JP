---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5e2bccfddad42a7da548f6177e85a7842a32e436
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35731289"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/mailFolders/AAMkAGVmMDEzM')
    .get();

```