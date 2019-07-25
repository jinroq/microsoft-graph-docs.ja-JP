---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ac666ae15eeae2ab936cf377150710ef8e1efbe4
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35728939"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/outlook/taskFolders/AAMkADIyAAAhrbPXAAA=')
    .version('beta')
    .delete();

```