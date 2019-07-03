---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5a8af9420f8cb6d8c6eba2e251ea52fa98f80b00
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35485053"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/events/{id}/attachments/{id}')
    .version('beta')
    .delete();

```