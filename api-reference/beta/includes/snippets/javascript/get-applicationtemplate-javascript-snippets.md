---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ee7b8bf37e7556c58e407807802ed5bb0e87cc72
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35710148"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/applicationTemplates/{id}')
    .version('beta')
    .get();

```