---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4b3794520372aa14e295cbb0646463263d733b93
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35721486"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages/{id}/mentions/{id}')
    .version('beta')
    .delete();

```