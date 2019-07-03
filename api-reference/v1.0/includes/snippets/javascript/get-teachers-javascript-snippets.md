---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 94ab6ac29d87b9e61f0cdb8ab73cf65c0710176a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35463120"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/classes/{class-id}/teachers')
    .get();

```