---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 44e4c2978e315b03a05e01ab555079fbb0e5eeca
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35737583"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getEmailActivityUserDetail(period='D7')')
    .get();

```