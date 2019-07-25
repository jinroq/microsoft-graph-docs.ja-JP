---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e9e12670caaa15b33d78ce1294e7b48a2ce64fb1
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35707335"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/contracts')
    .version('beta')
    .get();

```