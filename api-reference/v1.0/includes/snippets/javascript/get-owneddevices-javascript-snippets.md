---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e2e6aeb839929f019d81d4d8bae77d045a50fa87
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35737996"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/ownedDevices')
    .get();

```