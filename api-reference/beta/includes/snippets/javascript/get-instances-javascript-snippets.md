---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d05366f4e69a696f31acf0d1ea54b5ba6a068bb9
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35714146"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/events/AAMkAGUzYRgWAAA=/instances?startDateTime=2019-04-08T09:00:00.0000000&endDateTime=2019-04-30T09:00:00.0000000&$select=subject,bodyPreview,seriesMasterId,type,recurrence,start,end')
    .version('beta')
    .select('subject,bodyPreview,seriesMasterId,type,recurrence,start,end')
    .get();

```