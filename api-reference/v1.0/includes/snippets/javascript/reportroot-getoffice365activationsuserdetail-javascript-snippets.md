---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 11d39ab73dd03bc3e09f73de02869b326ef9d4c5
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35471995"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getOffice365ActivationsUserDetail')
    .get();

```