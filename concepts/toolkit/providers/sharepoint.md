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
# <a name="sharepoint-provider"></a>SharePoint プロバイダー

Sharepoint web パーツ内の SharePoint プロバイダーを使用して、Microsoft Graph access でコンポーネントの電源を入れます。

詳細については、「 [providers](../providers.md)」を参照してください。

## <a name="get-started"></a>作業の開始

Web パーツの`onInit()`メソッド内でプロバイダーを初期化します。

```ts

// import the providers at the top of the page
import {Providers, SharePointProvider} from '@microsoft/mgt';

// add the onInit() method if not already there in your web part class
protected async onInit() {
    Providers.globalProvider = new SharePointProvider(this.context);
}
```

これで、 `render()`メソッドにコンポーネントを追加し、SharePoint コンテキストを使用して Microsoft Graph にアクセスすることができます。

```ts

public render(): void {
    this.domElement.innerHTML = `
      <mgt-agenda></mgt-agenda>
      `;
  }
```

>**注:** Microsoft Graph ツールキットには、Typescript 3 .x が必要です。 [適切なコンパイラをインストール](https://github.com/SharePoint/sp-dev-docs/wiki/SharePoint-Framework-v1.8-release-notes#support-for-typescript-27-29-and-3x)して、サポートされているバージョンの Typescript を使用していることを確認してください。

## <a name="test-in-the-workbench"></a>ワークベンチでテストする

SharePoint web パーツの使用を開始しているばかりの場合は、「[最初の web パーツ](https://docs.microsoft.com/sharepoint/dev/spfx/web-parts/get-started/build-a-hello-world-web-part)のガイダンスを構築する」を参照してください。

Web パーツを作成した後、コンポーネントを使用する準備ができたら、web パーツが Microsoft Graph にアクセスするための適切なアクセス許可を持っていることを確認する必要があります。 詳細については、「 [SharePoint Framework で Microsoft Graph を使用する](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/use-aad-tutorial)」を参照してください。

簡単に言えば、に適切なアクセス許可を追加する`package-solution.json`ことが重要です。 Web パーツのパッケージを SharePoint にアップロードし、管理者が要求されたアクセス許可を承認する必要があります。

>**ヒント:** 追加するアクセス許可がわからない場合は、各コンポーネントのドキュメントに必要なすべてのアクセス許可が含まれています。
