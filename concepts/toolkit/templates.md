---
title: Microsoft Graph ツールキットのテンプレート
description: コンポーネントのコンテンツを変更するには、カスタムテンプレートを使用します。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: f0648d0ac1348fbadad6cebe8a022f9445fcf1e3
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/26/2019
ms.locfileid: "35243041"
---
# <a name="templates-in-the-microsoft-graph-toolkit"></a>Microsoft Graph ツールキットのテンプレート

コンポーネントのコンテンツを変更するには、カスタムテンプレートを使用します。

すべての web コンポーネントは、 `<template>`要素に基づくテンプレートをサポートしています。 たとえば、コンポーネントのテンプレートを上書きするには、コンポーネント内`<template>`に要素を追加します。

```html
<mgt-agenda>
  <template data-type="event">
      <div>{{event.subject}}</div>
      <div data-for='attendee in event.attendees'>
          <mgt-person person-query="{{attendee.emailAddress.name}}">
            <template>
              <div data-if="person.image">
                <img src="{{person.image}}" />
              </div>
              <div data-else>
                {{person.displayName}}
              </div>
            </template>
          </mgt-person>
      </div>
  </template>
</mgt-agenda>
```

次のテンプレート機能がサポートされています。

- 2つの波かっこ (`{{expression}}`) を使用して、式を展開します。 前の例では、 `<mgt-person>`は、 `person`テンプレートで使用できるオブジェクトを渡しています。
- 条件付き`data-if`レンダリング`data-else`の属性と属性を使用します。 など`event.attendees.length > 2`の条件式がサポートされています。
- を使用`data-for`して要素を繰り返します。
- を使用`data-type`して、コンポーネントのどの部分をテンプレートに含めるかを指定します。 型を指定しない場合は、テンプレートがコンポーネント全体に適用されます。

各コンポーネントは、サポート`data-type`されている値と、各テンプレートに渡されるデータコンテキストを文書にします。

テンプレートは、シャドウ dom の外側でレンダリングされるときに、通常どおりにスタイル設定できます。
