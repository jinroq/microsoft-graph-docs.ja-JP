---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d026a836c3cc601af0338239d74efd64c6f69a7f
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35728316"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const programControl = {
    controlId: "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
    controlTypeId: "6e4f3d20-c5c3-407f-9695-8460952bcc68",
    programId: "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213"
};

let res = await client.api('/programControls')
    .version('beta')
    .post({programControl : programControl});

```