---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a23cd922028856979dd7c7226eec4e4b5d18d76e
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35714532"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/schools/10002')
    .version('beta')
    .delete();

```