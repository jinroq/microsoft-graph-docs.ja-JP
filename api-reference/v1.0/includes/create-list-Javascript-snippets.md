---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6372ce64804a005fff43afb38076f0149f026afa
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34456054"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const list = {
  name: "Books",
  columns: [
    {
      name: "Author",
      text: { }
    },
    {
      name: "PageCount",
      number: { }
    }
  ],
  list: {
    template: "genericList"
  }
};

let res = await client.api('/sites/{site-id}/lists')
    .post({list : list});

```