---
description: 自動生成されたファイル。 変更しないでください
ms.openlocfilehash: 0aaa3905f3bf23b19bb862a06324578f07524967
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35882496"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/calendar/events')
    .get();

```