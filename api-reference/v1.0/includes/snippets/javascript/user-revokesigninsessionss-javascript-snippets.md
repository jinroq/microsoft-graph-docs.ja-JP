---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 3ffaacaf29edfbab48d23e503b845c8d4c271861
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35711298"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/revokeSignInSessions')
    .post();

```