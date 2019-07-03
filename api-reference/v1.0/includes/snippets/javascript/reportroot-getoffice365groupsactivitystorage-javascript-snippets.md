---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6471722119cd53243baf9e2270c11efe2b6ef3aa
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35514391"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getOffice365GroupsActivityStorage(period='D7')')
    .get();

```