---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ff08acb71ae40c11d2ae987b4dfa5aaa32f9417c
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35706082"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/root/delta?token=latest')
    .version('beta')
    .get();

```