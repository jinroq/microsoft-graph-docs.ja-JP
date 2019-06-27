---
title: Microsoft Teams プロバイダ
description: Microsoft Teams タブの内部にある Teams プロバイダーを使用して、認証と Microsoft Graph のすべてのコンポーネントへのアクセスを容易にします。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 348980225f04adfac4ded6f79a72654fbeec81e7
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/26/2019
ms.locfileid: "35243045"
---
# <a name="microsoft-teams-provider"></a>Microsoft Teams プロバイダ

Microsoft Teams タブの内部にある Teams プロバイダーを使用して、認証と Microsoft Graph のすべてのコンポーネントへのアクセスを容易にします。

詳細については、「 [providers](../providers.md)」を参照してください。

## <a name="get-started"></a>作業の開始

Teams プロバイダーを使用する前に、ページで[Microsoft TEAMS SDK](https://docs.microsoft.com/en-us/javascript/api/overview/msteams-client?view=msteams-client-js-latest#using-the-sdk)を参照していることを確認する必要があります。

次の例では、HTML (CDN 経由) でプロバイダーを使用します。

```html
<!-- Microsoft Teams sdk must be referenced before the toolkit -->
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<mgt-teams-provider
  client-id="<YOUR_CLIENT_ID>"
  auth-popup-url="https://<YOUR-DOMAIN>.com/AUTH-PATH"
></mgt-teams-provider>
```

次の例では、(NPM を介して) JS モジュールでプロバイダーを使用しています。

ツールキットと Microsoft Teams SDK の両方がインストールされていることを確認してください。

```bash
npm install @microsoft/mgt @microsoft/teams-js
```

次に、プロバイダーをインポートして使用します。

```ts
import '@microsoft/teams-js';
import {Providers, TeamsProvider} from '@microsoft/mgt'; 
Providers.globalProvider = new TeamsProvider(config);
```

where `config`は

```ts
export interface TeamsConfig {
  clientId: string;
  authPopupUrl: string;
  scopes?: string[];
  msalOptions?: Configuration;
}
```

完全な例については、「 [Microsoft Teams タブのサンプル](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/teams-tab)」を参照してください。

## <a name="configure-your-teams-app"></a>Teams アプリを構成する

Teams アプリの使用を開始するだけの場合は、「 [Microsoft teams アプリにタブを追加する](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/tabs/tabs-overview)」を参照してください。 アプリ[Studio](https://docs.microsoft.com/en-us/microsoftteams/platform/get-started/get-started-app-studio)を使用して、アプリマニフェストをすばやく開発することもできます。

タブを使用してアプリをインストールした後、コンポーネントを使用する準備ができたら、アプリが Microsoft Graph にアクセスするための適切なアクセス許可を持っていることを確認する必要があります。 必要なアクセス許可を使用してアプリを構成するには、次のようにします。

1. [ドメイン名を取得する](https://docs.microsoft.com/en-us/azure/active-directory/identity-protection/graph-get-started#retrieve-your-domain-name)
2. [新しいアプリの登録を作成する](https://docs.microsoft.com/en-us/azure/active-directory/identity-protection/graph-get-started#create-a-new-app-registration)
3. [アプリケーションのアクセス許可を付与する](https://docs.microsoft.com/en-us/azure/active-directory/identity-protection/graph-get-started#grant-your-application-permission-to-use-the-api)

[ **API へのアクセスの追加] ページ**に適切な権限を追加することが重要です。 必要なコンポーネントに応じて、管理者がアクセス許可を追加して承認する必要があります。

>**ヒント:** 追加するアクセス許可がわからない場合は、各コンポーネントのドキュメントを参照してください。

### <a name="enable-implicit-grant-flow"></a>暗黙的な許可フローを有効にする

暗黙的な許可フローを有効にしてください。これは、クライアント側からトークンを要求する web アプリの要件です。 Azure Portal では、アプリの登録を管理するときに、マニフェストを`oauth2AllowImplicitFlow`編集`true`してに変更します。

### <a name="create-the-popup-page"></a>ポップアップページを作成する

Teams の資格情報を使用してサインインするには、Teams アプリがポップアップで開く URL を指定する必要があります。これは、認証フローに従います。 この URL は、ドメイン内に存在する必要があり、 `TeamsProvider.handleAuth();`メソッドを呼び出す必要があります。 このページで実行する必要があるのは、これだけです。 次に例を示します。

```html
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js">

<script>        
  mgt.TeamsProvider.handleAuth();
</script>
```

### <a name="configure-redirect-uris"></a>リダイレクト Uri を構成する

このページを web サイトに公開した後、 `auth-popup-url/authPopupUrl`プロパティで URL を使用する必要があります。 この URL は、Azure AD ポータルのアプリ構成で有効なリダイレクト URI として構成する必要もあります。
