---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8a6cae59e36d3aec710e4c3c4f7a0a261ddc8d91
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35705634"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/classes/11023/teachers')
    .version('beta')
    .get();

```