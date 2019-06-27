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
# <a name="styling-components-in-the-microsoft-graph-toolkit"></a>Microsoft Graph ツールキットのコンポーネントのスタイル設定

コンポーネントスタイルを変更するには、CSS カスタムプロパティを使用します。

各コンポーネントには、特定の要素の外観を変更するために使用できる[CSS カスタムプロパティ](https://developer.mozilla.org/en-US/docs/Web/CSS/Using_CSS_custom_properties)のセットが記載されています。 次に例を示します。

```css
mgt-person {
  --avatar-size: 34px;
}
```

CSS カスタムプロパティを指定しない場合、コンポーネントの内部要素をスタイル設定することはできません。 コンポーネント子要素は、[シャドウ dom](https://developer.mozilla.org/en-US/docs/Web/Web_Components/Using_shadow_DOM)でホストされます。

柔軟性を高めるために、[カスタムテンプレート](./templates.md)の使用を検討してください。

## <a name="disable-the-shadow-dom-experimental"></a>シャドウ dom (実験的) を無効にする

シャドウ dom を無効にして、通常のブラウザースタイルシートを使用して内部要素のスタイルを`useShadowDom`直接設定`MgtBaseComponent`することができます。そのためには、いずれかのプロパティを false に設定してから、任意のプロパティを使用します。


```html
<script type="module">
  import { MgtBaseComponent } from './dist/es6/components/baseComponent.js';
   MgtBaseComponent.useShadowRoot = false;
</script>

<script type="module" src="./dist/es6/components/mgt-tasks/mgt-tasks.js"></script>
````
