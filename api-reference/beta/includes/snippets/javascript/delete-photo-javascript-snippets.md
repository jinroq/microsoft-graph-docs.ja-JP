---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d636417de97e4c3a56392cd7b21de07ef33d31a3
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35720733"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/{id|userPrincipalName}/photo')
    .version('beta')
    .delete();

```