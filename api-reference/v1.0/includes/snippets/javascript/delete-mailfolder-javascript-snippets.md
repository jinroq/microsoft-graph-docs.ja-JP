---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a9e00c07b8f657f4d3319a7ec62d1d52ac2eefe2
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35731318"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/mailFolders/{id}')
    .delete();

```