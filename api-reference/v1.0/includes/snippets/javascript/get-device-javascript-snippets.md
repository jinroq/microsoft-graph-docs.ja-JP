---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 15e8f1f739783669bb15b369c04aa017c61a8c2b
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35735202"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/devices/{id}')
    .get();

```