---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c2c5d415eeb36a72056f08b408f5380d2c878492
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35714327"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationUser = {
  displayName: "Rogelio Cazares",
  givenName: "Rogelio",
  middleName: "Fernando",
  surname: "Cazares",
};

let res = await client.api('/education/users/13020')
    .version('beta')
    .update({educationUser : educationUser});

```