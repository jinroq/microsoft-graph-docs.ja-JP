---
title: SharePoint プロバイダー
description: Sharepoint web パーツ内の SharePoint プロバイダーを使用して、Microsoft Graph access でコンポーネントの電源を入れます。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 684214e1490238564065c2ed53588b9700d17dc3
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/26/2019
ms.locfileid: "35243048"
---
# <a name="sharepoint-provider"></a><span data-ttu-id="ff230-103">SharePoint プロバイダー</span><span class="sxs-lookup"><span data-stu-id="ff230-103">SharePoint provider</span></span>

<span data-ttu-id="ff230-104">Sharepoint web パーツ内の SharePoint プロバイダーを使用して、Microsoft Graph access でコンポーネントの電源を入れます。</span><span class="sxs-lookup"><span data-stu-id="ff230-104">Use the SharePoint provider inside your SharePoint web parts to power the components with Microsoft Graph access.</span></span>

<span data-ttu-id="ff230-105">詳細については、「 [providers](../providers.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ff230-105">To learn more, see [providers](../providers.md).</span></span>

## <a name="get-started"></a><span data-ttu-id="ff230-106">作業の開始</span><span class="sxs-lookup"><span data-stu-id="ff230-106">Get started</span></span>

<span data-ttu-id="ff230-107">Web パーツの`onInit()`メソッド内でプロバイダーを初期化します。</span><span class="sxs-lookup"><span data-stu-id="ff230-107">Initialize the provider inside the `onInit()` method of your web part.</span></span>

```ts

// import the providers at the top of the page
import {Providers, SharePointProvider} from '@microsoft/mgt';

// add the onInit() method if not already there in your web part class
protected async onInit() {
    Providers.globalProvider = new SharePointProvider(this.context);
}
```

<span data-ttu-id="ff230-108">これで、 `render()`メソッドにコンポーネントを追加し、SharePoint コンテキストを使用して Microsoft Graph にアクセスすることができます。</span><span class="sxs-lookup"><span data-stu-id="ff230-108">Now you can add any component in your `render()` method and it will use the SharePoint context to access Microsoft Graph.</span></span>

```ts

public render(): void {
    this.domElement.innerHTML = `
      <mgt-agenda></mgt-agenda>
      `;
  }
```

><span data-ttu-id="ff230-109">**注:** Microsoft Graph ツールキットには、Typescript 3 .x が必要です。</span><span class="sxs-lookup"><span data-stu-id="ff230-109">**Note:** The Microsoft Graph Toolkit requires Typescript 3.x.</span></span> <span data-ttu-id="ff230-110">[適切なコンパイラをインストール](https://github.com/SharePoint/sp-dev-docs/wiki/SharePoint-Framework-v1.8-release-notes#support-for-typescript-27-29-and-3x)して、サポートされているバージョンの Typescript を使用していることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="ff230-110">Make sure you're using a supported version of Typescript by [installing the right compiler](https://github.com/SharePoint/sp-dev-docs/wiki/SharePoint-Framework-v1.8-release-notes#support-for-typescript-27-29-and-3x).</span></span>

## <a name="test-in-the-workbench"></a><span data-ttu-id="ff230-111">ワークベンチでテストする</span><span class="sxs-lookup"><span data-stu-id="ff230-111">Test in the workbench</span></span>

<span data-ttu-id="ff230-112">SharePoint web パーツの使用を開始しているばかりの場合は、「[最初の web パーツ](https://docs.microsoft.com/sharepoint/dev/spfx/web-parts/get-started/build-a-hello-world-web-part)のガイダンスを構築する」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ff230-112">If you're just getting started with SharePoint web parts, you can follow the [Build your first web part](https://docs.microsoft.com/sharepoint/dev/spfx/web-parts/get-started/build-a-hello-world-web-part) guidance.</span></span>

<span data-ttu-id="ff230-113">Web パーツを作成した後、コンポーネントを使用する準備ができたら、web パーツが Microsoft Graph にアクセスするための適切なアクセス許可を持っていることを確認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ff230-113">After you've created a web part, and you're ready to use the components, you will need to make sure that your web part has the right permissions to access Microsoft Graph.</span></span> <span data-ttu-id="ff230-114">詳細については、「 [SharePoint Framework で Microsoft Graph を使用する](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/use-aad-tutorial)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ff230-114">For details, see [Consume Microsoft Graph in the SharePoint Framework](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/use-aad-tutorial).</span></span>

<span data-ttu-id="ff230-115">簡単に言えば、に適切なアクセス許可を追加する`package-solution.json`ことが重要です。</span><span class="sxs-lookup"><span data-stu-id="ff230-115">In short, it's important to add the right permission to your `package-solution.json`.</span></span> <span data-ttu-id="ff230-116">Web パーツのパッケージを SharePoint にアップロードし、管理者が要求されたアクセス許可を承認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ff230-116">You will need to upload a package of your web part to SharePoint and have an administrator approve the requested permissions.</span></span>

><span data-ttu-id="ff230-117">**ヒント:** 追加するアクセス許可がわからない場合は、各コンポーネントのドキュメントに必要なすべてのアクセス許可が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ff230-117">**Tip:** if you're not sure what permissions to add, the documentation for each component includes all the permissions it needs.</span></span>
