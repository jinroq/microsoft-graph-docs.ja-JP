---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 80736f9b3ddfdd6b83415f5c9b1af3e71716f0b3
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/27/2019
ms.locfileid: "36637784"
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
    .post(educationUser);

```