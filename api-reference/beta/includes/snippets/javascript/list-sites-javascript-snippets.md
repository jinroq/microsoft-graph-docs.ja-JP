---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d456ab2c81247fea29c216bf3053d14a9afe4cb3
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35725172"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/sites?select=siteCollection,webUrl&filter=siteCollection/root%20ne%20null')
    .version('beta')
    .filter('siteCollection/root ne null')
    .get();

```