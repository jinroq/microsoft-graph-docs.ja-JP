---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 57b14a4656a2e473cd19eb2a1159e3f7e7597a93
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35495771"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChartAxisTitle = {
  text: "text-value",
  visible: true
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/title')
    .update({workbookChartAxisTitle : workbookChartAxisTitle});

```