---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 2b6558d30cff58ca1ff3e16bb8ff246411c62692
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35527734"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/{id}/chats')
    .version('beta')
    .get();

```