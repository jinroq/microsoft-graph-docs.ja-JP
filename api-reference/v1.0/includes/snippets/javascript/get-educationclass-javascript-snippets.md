---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a764022f5cdd42f6a51e8b18d2e56cc18ccfac93
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35715505"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/classes/{class-id}')
    .get();

```