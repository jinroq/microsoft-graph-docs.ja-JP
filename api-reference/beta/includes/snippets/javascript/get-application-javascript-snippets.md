---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 00b02d3abdeb67c00905e72687cd83205d565ff9
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35710316"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/applications/{id}')
    .version('beta')
    .get();

```