---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a817c3b3cfdc0da926a18eba75709d3a57535380
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35710549"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/agreements')
    .version('beta')
    .get();

```