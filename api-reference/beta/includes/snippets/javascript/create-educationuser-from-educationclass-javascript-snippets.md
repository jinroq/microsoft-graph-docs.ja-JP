---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9638b89d82e1da4386e12a01f36164a570f13385
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35705616"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationUser = {
  @odata.id:"https://graph.microsoft.com/beta/education/users/14011"
};

let res = await client.api('/education/classes/11017/teachers/$ref')
    .version('beta')
    .post({educationUser : educationUser});

```