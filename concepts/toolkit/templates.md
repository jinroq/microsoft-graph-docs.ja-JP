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
# <a name="templates-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="d1fd5-103">Microsoft Graph ツールキットのテンプレート</span><span class="sxs-lookup"><span data-stu-id="d1fd5-103">Templates in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="d1fd5-104">コンポーネントのコンテンツを変更するには、カスタムテンプレートを使用します。</span><span class="sxs-lookup"><span data-stu-id="d1fd5-104">Use custom templates to modify the content of a component.</span></span>

<span data-ttu-id="d1fd5-105">すべての web コンポーネントは、 `<template>`要素に基づくテンプレートをサポートしています。</span><span class="sxs-lookup"><span data-stu-id="d1fd5-105">All web components support templates based on the `<template>` element.</span></span> <span data-ttu-id="d1fd5-106">たとえば、コンポーネントのテンプレートを上書きするには、コンポーネント内`<template>`に要素を追加します。</span><span class="sxs-lookup"><span data-stu-id="d1fd5-106">For example, to override the template of a component, add a `<template>` element inside a component.</span></span>

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

<span data-ttu-id="d1fd5-107">次のテンプレート機能がサポートされています。</span><span class="sxs-lookup"><span data-stu-id="d1fd5-107">The following template features are supported:</span></span>

- <span data-ttu-id="d1fd5-108">2つの波かっこ (`{{expression}}`) を使用して、式を展開します。</span><span class="sxs-lookup"><span data-stu-id="d1fd5-108">Use the double curly brackets (`{{expression}}`) to expand an expression.</span></span> <span data-ttu-id="d1fd5-109">前の例では、 `<mgt-person>`は、 `person`テンプレートで使用できるオブジェクトを渡しています。</span><span class="sxs-lookup"><span data-stu-id="d1fd5-109">In the previous example, the `<mgt-person>` passes a `person` object that you can use in the template.</span></span>
- <span data-ttu-id="d1fd5-110">条件付き`data-if`レンダリング`data-else`の属性と属性を使用します。</span><span class="sxs-lookup"><span data-stu-id="d1fd5-110">Use the `data-if` and `data-else` attributes for conditional rendering.</span></span> <span data-ttu-id="d1fd5-111">など`event.attendees.length > 2`の条件式がサポートされています。</span><span class="sxs-lookup"><span data-stu-id="d1fd5-111">Conditional expressions such as `event.attendees.length > 2` are supported.</span></span>
- <span data-ttu-id="d1fd5-112">を使用`data-for`して要素を繰り返します。</span><span class="sxs-lookup"><span data-stu-id="d1fd5-112">Use the `data-for` to repeat an element.</span></span>
- <span data-ttu-id="d1fd5-113">を使用`data-type`して、コンポーネントのどの部分をテンプレートに含めるかを指定します。</span><span class="sxs-lookup"><span data-stu-id="d1fd5-113">Use the `data-type` to specify what part of the component to template.</span></span> <span data-ttu-id="d1fd5-114">型を指定しない場合は、テンプレートがコンポーネント全体に適用されます。</span><span class="sxs-lookup"><span data-stu-id="d1fd5-114">Not specifying the type will apply the template to the entire component.</span></span>

<span data-ttu-id="d1fd5-115">各コンポーネントは、サポート`data-type`されている値と、各テンプレートに渡されるデータコンテキストを文書にします。</span><span class="sxs-lookup"><span data-stu-id="d1fd5-115">Each component documents the supported `data-type` values and what data context is passed down to each template.</span></span>

<span data-ttu-id="d1fd5-116">テンプレートは、シャドウ dom の外側でレンダリングされるときに、通常どおりにスタイル設定できます。</span><span class="sxs-lookup"><span data-stu-id="d1fd5-116">The templates can be styled normally as they are rendered outside of the shadow dom.</span></span>
