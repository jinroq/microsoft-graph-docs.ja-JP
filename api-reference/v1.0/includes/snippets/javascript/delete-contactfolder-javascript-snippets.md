---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ba3fe481771a2456bac05866560cee5317b0285c
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35741005"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/contactFolders/{id}')
    .delete();

```