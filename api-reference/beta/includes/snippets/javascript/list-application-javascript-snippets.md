---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6e9fd5aad905bc79ef588a57ab75e20b2a4ee10b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35504149"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/applications')
    .version('beta')
    .get();

```