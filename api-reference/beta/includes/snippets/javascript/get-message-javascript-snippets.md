---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c57ae5d1231c2c9c6a867c6a286e91afe410b674
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35729848"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages/AAMkAGI1AAAoZCfHAAA=')
    .version('beta')
    .get();

```