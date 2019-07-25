---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a4bfc7172adb61ed99b9f7d2fbc8f25a2c0e2177
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35732157"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages/{id}')
    .delete();

```