---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9c9570a6125eeabc8d17eca5578ef81617233e5c
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35711522"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const application = {
  allowPublicClient: true,
  displayName: "Display name"
};

let res = await client.api('/applications')
    .version('beta')
    .post({application : application});

```