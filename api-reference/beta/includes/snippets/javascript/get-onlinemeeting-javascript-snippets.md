---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 35f669d6d339991e5c224bf652f800faae7ac5ae
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35485712"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/app/onlineMeetings/{id}')
    .version('beta')
    .get();

```