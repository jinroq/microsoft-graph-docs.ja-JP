---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6a6abdaee2ea42cefdd9f63cbda04b38ecfcb49e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35504637"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/contacts/{id}/manager')
    .version('beta')
    .get();

```