---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 7879beb10ea5ab20b9a3ea2daa777b8a644488e0
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35727455"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/onenote/sectionGroups/{id}/sectionGroups')
    .version('beta')
    .get();

```