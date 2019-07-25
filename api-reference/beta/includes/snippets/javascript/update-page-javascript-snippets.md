---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 819318934baf928978419467e3f474584ffce711
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35728725"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const Stream = [
   {
    'target':'#para-id',
    'action':'insert',
    'position':'before',
    'content':'<img src="image-url-or-part-name" alt="image-alt-text" />'
  }, 
  {
    'target':'#list-id',
    'action':'append',
    'content':'<li>new-page-content</li>'
  }
];

let res = await client.api('/me/onenote/pages/{id}/content')
    .version('beta')
    .update({Stream : Stream});

```