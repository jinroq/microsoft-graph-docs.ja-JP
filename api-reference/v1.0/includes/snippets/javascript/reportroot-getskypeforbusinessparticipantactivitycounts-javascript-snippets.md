---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0d9ea6add3dd56644a87b0b5c3100a07b5bba80d
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35734616"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSkypeForBusinessParticipantActivityCounts(period='D7')')
    .get();

```