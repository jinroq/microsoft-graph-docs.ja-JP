---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6559999e0a6c3f4f0bbb90efc77030e67993454f
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35728960"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const outlookTaskFolder = {
  name: "Charity work"
};

let res = await client.api('/me/outlook/taskFolders/AAMkADIyAAAhrbPWAAA=')
    .version('beta')
    .update({outlookTaskFolder : outlookTaskFolder});

```