---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d2fbfe55aaa8cdb9628a6df27d3e53866719fd12
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35717668"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{teamId}/schedule/shifts/{shiftId}')
    .version('beta')
    .get();

```