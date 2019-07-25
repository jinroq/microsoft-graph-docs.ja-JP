---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a70506e89b600190f625644e876aa3dc9ec24ed8
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35730582"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/outlook/taskFolders')
    .version('beta')
    .get();

```