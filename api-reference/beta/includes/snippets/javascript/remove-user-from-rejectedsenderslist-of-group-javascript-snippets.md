---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5a589af90237d49dfc03f68de2aa3cf1b8fce105
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35712138"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/rejectedSenders/$ref')
    .version('beta')
    .delete();

```