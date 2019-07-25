---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 94ab6ac29d87b9e61f0cdb8ab73cf65c0710176a
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35715462"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/classes/{class-id}/teachers')
    .get();

```