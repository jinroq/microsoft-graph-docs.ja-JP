---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e680000fb85346872df28891fcb082fbf26b9386
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35729235"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/onenote/notebooks')
    .version('beta')
    .get();

```