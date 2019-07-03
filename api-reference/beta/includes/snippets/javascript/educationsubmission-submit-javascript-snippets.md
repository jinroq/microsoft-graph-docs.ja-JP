---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: fba3e84128028cbe597fa98f1a1b1d9c71cd93cc
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35504553"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/classes/11021/assignments/19002/submissions/850f51b7/submit')
    .version('beta')
    .post();

```