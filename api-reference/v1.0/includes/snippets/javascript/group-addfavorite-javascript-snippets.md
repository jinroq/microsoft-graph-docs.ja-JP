---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: cb59c813634b30a295ced5547537bbc7a725f26a
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35740207"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/addFavorite')
    .post();

```