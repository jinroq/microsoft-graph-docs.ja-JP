---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: cfeab76fee4f086cc4dd5759c4b487418905349c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35526815"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/threads')
    .version('beta')
    .get();

```