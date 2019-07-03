---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8642aafe1d11c8701907706e0376794c4da83f25
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35472124"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationUser = {
  @odata.id:"https://graph.microsoft.com/v1.0/education/users/14008"
};

let res = await client.api('/education/schools/{id}/users/$ref')
    .post({educationUser : educationUser});

```