---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 1b30f866aae9d418a7af79c09ce11cd5ecd60e66
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35740475"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/root/workbook/worksheets/{id}/range(address='A1:Z10')/visibleView/range')
    .get();

```