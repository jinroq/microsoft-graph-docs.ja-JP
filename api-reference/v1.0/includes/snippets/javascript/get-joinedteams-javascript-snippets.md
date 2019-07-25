---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5e72c61ae60ac6a69bc28309855f8cd914008220
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35714614"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/joinedTeams')
    .get();

```