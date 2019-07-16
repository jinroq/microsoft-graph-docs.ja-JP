---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a9e6a966a8cf722631f5e472fce6f3f45a5f198f
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35738682"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/calendar')
    .get();

```