---
title: Microsoft Graph ツールキットのスタイル設定
description: CSS カスタムプロパティを使用してコンポーネントスタイルを変更する
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 41262c4e58973d84f4fec56a6d5abe8dfaf555ef
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/26/2019
ms.locfileid: "35243044"
---
# <a name="styling-components-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="009ff-103">Microsoft Graph ツールキットのコンポーネントのスタイル設定</span><span class="sxs-lookup"><span data-stu-id="009ff-103">Styling components in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="009ff-104">コンポーネントスタイルを変更するには、CSS カスタムプロパティを使用します。</span><span class="sxs-lookup"><span data-stu-id="009ff-104">Use CSS custom properties to modify the component styles.</span></span>

<span data-ttu-id="009ff-105">各コンポーネントには、特定の要素の外観を変更するために使用できる[CSS カスタムプロパティ](https://developer.mozilla.org/en-US/docs/Web/CSS/Using_CSS_custom_properties)のセットが記載されています。</span><span class="sxs-lookup"><span data-stu-id="009ff-105">Each component documents a set of [CSS custom properties](https://developer.mozilla.org/en-US/docs/Web/CSS/Using_CSS_custom_properties) that you can use to change the look and feel of certain elements.</span></span> <span data-ttu-id="009ff-106">次に例を示します。</span><span class="sxs-lookup"><span data-stu-id="009ff-106">For example:</span></span>

```css
mgt-person {
  --avatar-size: 34px;
}
```

<span data-ttu-id="009ff-107">CSS カスタムプロパティを指定しない場合、コンポーネントの内部要素をスタイル設定することはできません。</span><span class="sxs-lookup"><span data-stu-id="009ff-107">You can't style internal elements of a component unless you provide a CSS custom property.</span></span> <span data-ttu-id="009ff-108">コンポーネント子要素は、[シャドウ dom](https://developer.mozilla.org/en-US/docs/Web/Web_Components/Using_shadow_DOM)でホストされます。</span><span class="sxs-lookup"><span data-stu-id="009ff-108">The component child elements are hosted in a [shadow dom](https://developer.mozilla.org/en-US/docs/Web/Web_Components/Using_shadow_DOM).</span></span>

<span data-ttu-id="009ff-109">柔軟性を高めるために、[カスタムテンプレート](./templates.md)の使用を検討してください。</span><span class="sxs-lookup"><span data-stu-id="009ff-109">For more flexibility, consider using [custom templates](./templates.md).</span></span>

## <a name="disable-the-shadow-dom-experimental"></a><span data-ttu-id="009ff-110">シャドウ dom (実験的) を無効にする</span><span class="sxs-lookup"><span data-stu-id="009ff-110">Disable the shadow dom (experimental)</span></span>

<span data-ttu-id="009ff-111">シャドウ dom を無効にして、通常のブラウザースタイルシートを使用して内部要素のスタイルを`useShadowDom`直接設定`MgtBaseComponent`することができます。そのためには、いずれかのプロパティを false に設定してから、任意のプロパティを使用します。</span><span class="sxs-lookup"><span data-stu-id="009ff-111">You can disable the shadow dom, and directly style internal elements using normal browser stylesheets, by setting the static property `useShadowDom` of the `MgtBaseComponent` class to false before using any MGT tags.</span></span>


```html
<script type="module">
  import { MgtBaseComponent } from './dist/es6/components/baseComponent.js';
   MgtBaseComponent.useShadowRoot = false;
</script>

<script type="module" src="./dist/es6/components/mgt-tasks/mgt-tasks.js"></script>
````
