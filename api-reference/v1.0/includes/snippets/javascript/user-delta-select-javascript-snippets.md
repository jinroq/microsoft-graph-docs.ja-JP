---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 29663036263e53dd35b20c5575424959a7c665b1
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35496275"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/delta')
    .select('displayName,jobTitle,mobilePhone')
    .get();

```