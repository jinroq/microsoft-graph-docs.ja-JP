---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 161636dac4a8270b9693d1594bf25b3a9ba6b08a
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35705740"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/classes/11021/assignments/19002/publish')
    .version('beta')
    .post();

```