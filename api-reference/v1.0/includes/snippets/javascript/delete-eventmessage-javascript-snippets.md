---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a4bfc7172adb61ed99b9f7d2fbc8f25a2c0e2177
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35514052"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages/{id}')
    .delete();

```