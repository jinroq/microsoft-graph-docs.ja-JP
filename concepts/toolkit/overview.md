---
title: Microsoft Graph Toolkit (プレビュー)
description: Microsoft Graph Toolkit は、フレームワークに依存しない web コンポーネントと、Microsoft Graph にアクセスして作業するためのヘルパーのコレクションです。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: e6d5974029625a8dd1bef0c7b981fcf2b36b747c
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/26/2019
ms.locfileid: "35243063"
---
# <a name="microsoft-graph-toolkit-preview"></a><span data-ttu-id="9462b-103">Microsoft Graph Toolkit (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="9462b-103">Microsoft Graph Toolkit (preview)</span></span>

<span data-ttu-id="9462b-104">Microsoft Graph Toolkit は、フレームワークに依存しない web コンポーネントと、Microsoft Graph にアクセスして作業するためのヘルパーのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="9462b-104">The Microsoft Graph Toolkit is a collection of framework-agnostic web components and helpers for accessing and working with Microsoft Graph.</span></span> <span data-ttu-id="9462b-105">すべてのコンポーネントは、カスタマイズを必要とせずに Microsoft Graph にアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="9462b-105">ALl components can access Microsoft Graph without any customization required.</span></span>

>[!NOTE]
><span data-ttu-id="9462b-106">このライブラリはプレビュー版で、初期段階の開発に含まれています。</span><span class="sxs-lookup"><span data-stu-id="9462b-106">This library is in preview and is in early development.</span></span> <span data-ttu-id="9462b-107">コミュニティからのフィードバックに基づいて、すべてのコンポーネントと Api に変更が加えられ、強化されることを期待しています。</span><span class="sxs-lookup"><span data-stu-id="9462b-107">We expect to make changes and improvements to all components and APIs based on feedback from the community.</span></span>

## <a name="get-started"></a><span data-ttu-id="9462b-108">作業の開始</span><span class="sxs-lookup"><span data-stu-id="9462b-108">Get started</span></span>

<span data-ttu-id="9462b-109">コンポーネントを使用するには、そのローダーを直接 (または、pkg を介して) 参照するか、または npm パッケージをインストールします。</span><span class="sxs-lookup"><span data-stu-id="9462b-109">You can use the components by referencing the loader directly (via unpkg), or by installing the npm package.</span></span>

<span data-ttu-id="9462b-110">Microsoft Graph Toolkit を使用して作業を開始する方法の詳細については、「はじめに」の[ビデオ](https://www.youtube.com/watch?v=oZCGb2MMxa0)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9462b-110">For details about how to get started with the Microsoft Graph Toolkit, see the [Get started video](https://www.youtube.com/watch?v=oZCGb2MMxa0).</span></span>

### <a name="use-via-mgt-loader"></a><span data-ttu-id="9462b-111">Via による使用-ローダー</span><span class="sxs-lookup"><span data-stu-id="9462b-111">Use via mgt-loader</span></span>

<span data-ttu-id="9462b-112">[次の jsfiddle 例](https://jsfiddle.net/metulev/9phqxLd5/)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9462b-112">See the folowing [jsfiddle example](https://jsfiddle.net/metulev/9phqxLd5/).</span></span>

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
```

<span data-ttu-id="9462b-113">その後、HTML ページのコンポーネントの使用を開始できます。</span><span class="sxs-lookup"><span data-stu-id="9462b-113">You can then start using the components in your HTML page.</span></span> <span data-ttu-id="9462b-114">以下に、MSAL プロバイダーを使用した完全な作業例を示します。</span><span class="sxs-lookup"><span data-stu-id="9462b-114">The following is a full working example with the MSAL provider.</span></span>

```html
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>
<mgt-msal-provider client-id="[CLIENT-ID]"></mgt-msal-provider>
<mgt-login></mgt-login>

<!-- <script>
    // alternatively, you can set the provider in code and provide more options
    mgt.Providers.globalProvider = new mgt.MsalProvider({clientId: '[CLIENT-ID]'});
</script> -->
```

> <span data-ttu-id="9462b-115">**注:** MSAL では、認証リダイレクト用に web サーバーでページをホストする必要があります。</span><span class="sxs-lookup"><span data-stu-id="9462b-115">**Note:** MSAL requires the page to be hosted in a web server for the authentication redirects.</span></span> <span data-ttu-id="9462b-116">すぐにプレイしたい場合は、Visual Studio Code で[live サーバー](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer)を使用することができます。</span><span class="sxs-lookup"><span data-stu-id="9462b-116">If you're just getting started and want to play around, you can use [live server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) in Visual Studio Code.</span></span>

### <a name="use-via-npm-es6-modules"></a><span data-ttu-id="9462b-117">NPM 経由で使用する (es6 モジュール)</span><span class="sxs-lookup"><span data-stu-id="9462b-117">Use via NPM (es6 modules)</span></span>

<span data-ttu-id="9462b-118">Es6 モジュールを使用すると、バンドル処理を完全に制御でき、サイトに必要なコードのみをバンドルできます。</span><span class="sxs-lookup"><span data-stu-id="9462b-118">By using the es6 modules, you have full control of the bundling process and you can bundle only the code you need for your site.</span></span> <span data-ttu-id="9462b-119">最初に、npm パッケージを追加します。</span><span class="sxs-lookup"><span data-stu-id="9462b-119">First, add the npm package:</span></span>

```bash
npm install @microsoft/mgt
```

<span data-ttu-id="9462b-120">これで、使用しているページのすべてのコンポーネントを参照できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="9462b-120">Now you can reference all components at the page you are using:</span></span>

```html
<script src="node_modules/@microsoft/mgt/dist/es6/components.js"></script>
```

<span data-ttu-id="9462b-121">または、必要なコンポーネントを参照するだけで、それ以外のすべての読み込みが行われないようにします。</span><span class="sxs-lookup"><span data-stu-id="9462b-121">Or, just reference the component you need and avoid loading everything else:</span></span>

```html
<script src="node_modules/@microsoft/mgt/dist/es6/components/mgt-login/mgt-login.js"></script>
```

<span data-ttu-id="9462b-122">同様に、プロバイダーを追加するには、それをコンポーネントとして追加します。</span><span class="sxs-lookup"><span data-stu-id="9462b-122">Similarly, to add a provider, you can add it as a component:</span></span>

```html
<script src="node_modules/@microsoft/mgt/dist/es6/components/providers/mgt-msal-provider.js"></script>

<mgt-msal-provider client-id="[CLIENT-ID]"></mgt-msal-provider>
```

<span data-ttu-id="9462b-123">または、コードに追加します。</span><span class="sxs-lookup"><span data-stu-id="9462b-123">or, add it in your code:</span></span>

```html
<script type="module">
  import { Providers, MsalProvider } from '@microsoft/mgt';

  Providers.globalProvider = new MsalProvider({ clientId: '[CLIENT-ID]' });
</script>
```

## <a name="providers"></a><span data-ttu-id="9462b-124">会社</span><span class="sxs-lookup"><span data-stu-id="9462b-124">Providers</span></span>

<span data-ttu-id="9462b-125">コンポーネントは、[プロバイダー](./providers.md)で使用する場合に最適に機能します。</span><span class="sxs-lookup"><span data-stu-id="9462b-125">The components work best when used with a [provider](./providers.md).</span></span> <span data-ttu-id="9462b-126">プロバイダーは、コンポーネントが Microsoft Graph を呼び出すために使用する認証と Api を公開します。</span><span class="sxs-lookup"><span data-stu-id="9462b-126">The provider exposes authentication and APIs that the components use to call Microsoft Graph.</span></span>

<span data-ttu-id="9462b-127">ツールキットには、 [Msal](./providers/msal.md)、 [SharePoint](./providers/sharepoint.md)、 [Teams](./providers/teams.md)、Office アドインのプロバイダーが含まれています (近日中)。</span><span class="sxs-lookup"><span data-stu-id="9462b-127">The toolkit contains providers for [MSAL](./providers/msal.md), [SharePoint](./providers/sharepoint.md), [Teams](./providers/teams.md), and Office Add-ins (coming soon).</span></span> <span data-ttu-id="9462b-128">[IProvider] 抽象クラスを拡張して、独自のプロバイダーを作成することもできます。</span><span class="sxs-lookup"><span data-stu-id="9462b-128">You can also create your own providers by extending the [IProvider] abstract class.</span></span>

## <a name="polyfills"></a><span data-ttu-id="9462b-129">Polyfills.ts</span><span class="sxs-lookup"><span data-stu-id="9462b-129">Polyfills</span></span>

<span data-ttu-id="9462b-130">Npm パッケージの es6 モジュールを使用している場合は、polyfills.ts が自動的に含まれないように、プロジェクトにを含めるようにしてください。</span><span class="sxs-lookup"><span data-stu-id="9462b-130">If you're using the es6 modules from the npm package, make sure to include polyfills in your project as they are not included automatically.</span></span> <span data-ttu-id="9462b-131">詳細については、「 [polyfills.ts](https://www.webcomponents.org/polyfills)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9462b-131">To learn more, see [polyfills](https://www.webcomponents.org/polyfills).</span></span>

<span data-ttu-id="9462b-132">Mgt-loader スクリプトをパッケージ化されていないパッケージから使用している場合、polyfills.ts は既に含まれています。</span><span class="sxs-lookup"><span data-stu-id="9462b-132">If you're using the mgt-loader.js script from the bundle on unpkg, the polyfills are already included.</span></span>


## <a name="using-the-components-with-react-angular-and-other-frameworks"></a><span data-ttu-id="9462b-133">コンポーネントを反応、角度、およびその他のフレームワークで使用する</span><span class="sxs-lookup"><span data-stu-id="9462b-133">Using the components with React, Angular, and other frameworks</span></span>

<span data-ttu-id="9462b-134">Web コンポーネントは、いくつかの web 標準に基づいており、既に使用しているフレームワークで使用できます。</span><span class="sxs-lookup"><span data-stu-id="9462b-134">Web components are based on several web standards and can be used with any framework you're already using.</span></span> <span data-ttu-id="9462b-135">ただし、すべてのフレームワークが web コンポーネントを同じ方法で処理するわけではありません。</span><span class="sxs-lookup"><span data-stu-id="9462b-135">However, not all frameworks handle web components the same way.</span></span> <span data-ttu-id="9462b-136">フレームワークに応じて適用される可能性のある考慮事項の詳細については、「すべての場所のプロジェクトに[カスタム要素](https://custom-elements-everywhere.com/)を表示する」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9462b-136">To learn more about the considerations that might apply depending on your framework, see the [Custom Elements Everywhere](https://custom-elements-everywhere.com/) project.</span></span>

<span data-ttu-id="9462b-137">次のセクションでは、Microsoft Graph のツールキットコンポーネントを使用して、反応があり、角度を指定する方法の概要を簡単に説明します。</span><span class="sxs-lookup"><span data-stu-id="9462b-137">The following sections provide a quick overview of using the Microsoft Graph Toolkit components with React and Angular.</span></span>

### <a name="react"></a><span data-ttu-id="9462b-138">React</span><span class="sxs-lookup"><span data-stu-id="9462b-138">React</span></span>

<span data-ttu-id="9462b-139">応答は、すべてのデータを HTML 属性の形式でカスタム要素に渡します。</span><span class="sxs-lookup"><span data-stu-id="9462b-139">React passes all data to Custom Elements in the form of HTML attributes.</span></span> <span data-ttu-id="9462b-140">プリミティブデータの場合、これは問題ありませんが、オブジェクトや配列などの豊富なデータを渡すときには動作しません。</span><span class="sxs-lookup"><span data-stu-id="9462b-140">For primitive data this is fine, but it does not work when passing rich data, like objects or arrays.</span></span> <span data-ttu-id="9462b-141">そのような場合は、 `ref`を使用してオブジェクトを渡す必要があります。</span><span class="sxs-lookup"><span data-stu-id="9462b-141">In those cases you will need to use a `ref` to pass in the object.</span></span>

<span data-ttu-id="9462b-142">渡し</span><span class="sxs-lookup"><span data-stu-id="9462b-142">Ex:</span></span>

```jsx
// import all the components
import '@microsoft/mgt';

class App extends Component {
  render() {
    return <mgt-person show-name ref={el => (el.personDetails = { displayName: 'Nikola Metulev' })} />;
  }
}
```

<span data-ttu-id="9462b-143">応答は独自の代理イベントシステムを実装するため、回避策を使用せずにカスタム要素からの DOM イベントをリッスンすることはできません。</span><span class="sxs-lookup"><span data-stu-id="9462b-143">Because React implements its own synthetic event system, it cannot listen for DOM events coming from custom elements without the use of a workaround.</span></span> <span data-ttu-id="9462b-144">次の例に示すよう`ref`に、を使用して、ツールキットコンポーネントを参照し、イベントリスナーを addEventListener で手動でアタッチする必要があります。</span><span class="sxs-lookup"><span data-stu-id="9462b-144">You will need to use a `ref` to reference the toolkit components and manually attach event listeners with addEventListener, as shown in the following example.</span></span>

```jsx
// you can just import a single component
import '@microsoft/mgt/dist/es6/components/mgt-login/mgt-login.js';

class App extends Component {
  render() {
    return <mgt-login ref="loginComponent" />;
  }

  componentDidMount() {
    this.refs.loginComponent.addEventListener('loginCompleted', e => {
      // handle event
    });
  }
}
```

#### <a name="react-typescript-and-tsx"></a><span data-ttu-id="9462b-145">反応、Typescript、および TSX</span><span class="sxs-lookup"><span data-stu-id="9462b-145">React, Typescript, and TSX</span></span>

<span data-ttu-id="9462b-146">対応および Typescript でカスタム要素を使用すると、既知の問題が発生することがあります。</span><span class="sxs-lookup"><span data-stu-id="9462b-146">A known issue can occur when you use custom elements with React and Typescript.</span></span> <span data-ttu-id="9462b-147">Tsx でコンポーネントを使用しようとすると、Typescript によってエラーがスローされます。</span><span class="sxs-lookup"><span data-stu-id="9462b-147">Typescript will throw an error when trying to use a component in tsx.</span></span> <span data-ttu-id="9462b-148">回避策は、コードでカスタム要素を定義することです。以下に例を示します。</span><span class="sxs-lookup"><span data-stu-id="9462b-148">The workaround is to define the custom element in your code, as shown.</span></span>

```ts
declare global {
  namespace JSX {
    interface IntrinsicElements {
      'mgt-login': any;
    }
  }
}
```

<span data-ttu-id="9462b-149">その後、を tsx で使用でき`<mgt-login></mgt-login>`ます。</span><span class="sxs-lookup"><span data-stu-id="9462b-149">You can then use it in your tsx as `<mgt-login></mgt-login>`.</span></span>

### <a name="angular"></a><span data-ttu-id="9462b-150">Angular</span><span class="sxs-lookup"><span data-stu-id="9462b-150">Angular</span></span>

<span data-ttu-id="9462b-151">角度の既定のバインド構文は、常に要素のプロパティを設定します。</span><span class="sxs-lookup"><span data-stu-id="9462b-151">Angular's default binding syntax will always set properties on an element.</span></span> <span data-ttu-id="9462b-152">これは、オブジェクトや配列などの豊富なデータに適しています。また、プリミティブ値にも適しています。</span><span class="sxs-lookup"><span data-stu-id="9462b-152">This works well for rich data, like objects and arrays, and also works well for primitive values.</span></span>

<span data-ttu-id="9462b-153">カスタム要素を使用するには、まず、 `app.module.ts` `CUSTOM_ELEMENT_SCHEMA`を`@NgModule() decorator`に追加して、でカスタム要素を有効にします。次に例を示します。</span><span class="sxs-lookup"><span data-stu-id="9462b-153">To use custom elements, first, enable custom elements in your `app.module.ts` by adding the `CUSTOM_ELEMENT_SCHEMA` to the `@NgModule() decorator`, as shown in the following example.</span></span>

```ts
import { BrowserModule } from '@angular/platform-browser';
import { NgModule, CUSTOM_ELEMENTS_SCHEMA } from '@angular/core';

import { AppComponent } from './app.component';

@NgModule({
  declarations: [AppComponent],
  imports: [BrowserModule],
  schemas: [CUSTOM_ELEMENTS_SCHEMA],
  providers: [],
  bootstrap: [AppComponent]
})
export class AppModule {}
```

<span data-ttu-id="9462b-154">その後、コンポーネント\*の ts ファイルで使用するコンポーネントをインポートできます。</span><span class="sxs-lookup"><span data-stu-id="9462b-154">You can then import the component you'd like to use in your component \*.ts file.</span></span>

```ts
import { Component } from '@angular/core';
import '@microsoft/mgt/dist/es6/components/mgt-person/mgt-person';

@Component({
  selector: 'app-root',
  templateUrl: './app.component.html',
  styleUrls: ['./app.component.css']
})
export class AppComponent {
  person = {
    displayName: 'Nikola Metulev'
  };
}
```

<span data-ttu-id="9462b-155">最後に、テンプレート内の通常のようにコンポーネントを使用します。</span><span class="sxs-lookup"><span data-stu-id="9462b-155">Finally, use the component as you normally would in your template.</span></span>

```html
<mgt-person [personDetails]="person" show-name></mgt-person>
```
