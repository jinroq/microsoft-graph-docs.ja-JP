---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 7dd2eaa24ac14eaa65112293d61a3ee2f2c46174
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36373643"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/findMeetingTimes')
    .post();

```