---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 67c10e9f52ad598fc92d0584dd5a6f1273a4eabd
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35513238"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/conversations/{id}')
    .get();

```