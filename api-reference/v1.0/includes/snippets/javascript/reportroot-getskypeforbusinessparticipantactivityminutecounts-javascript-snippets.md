---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6b8d50fe227958c27df29196e7de009e71c0a5c6
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35734636"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSkypeForBusinessParticipantActivityMinuteCounts(period='D7')')
    .get();

```