---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6471722119cd53243baf9e2270c11efe2b6ef3aa
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35739337"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getOffice365GroupsActivityStorage(period='D7')')
    .get();

```