---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a46abe6071333cfafc15bdc21ae625cc5b965a31
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35472131"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationUser = {
  @odata.id:"https://graph.microsoft.com/v1.0/education/users/14011"
};

let res = await client.api('/education/classes/{class-id}/teachers/$ref')
    .post({educationUser : educationUser});

```