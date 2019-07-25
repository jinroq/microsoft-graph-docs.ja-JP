---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 1f3e27e82a250674899ddf1adb024898edb99467
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35712599"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/schools/10001')
    .version('beta')
    .get();

```