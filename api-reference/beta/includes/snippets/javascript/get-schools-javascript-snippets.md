---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 97a50d98be2d4640d690af7ea35e5d6ed0055eb5
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35712668"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/me/schools')
    .version('beta')
    .get();

```