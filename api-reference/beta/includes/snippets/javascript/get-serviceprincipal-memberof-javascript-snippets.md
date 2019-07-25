---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b12472c937c0dae48bc89d9b768456d0129e3cb2
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35725276"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/servicePrincipals/{id}/memberOf')
    .version('beta')
    .get();

```