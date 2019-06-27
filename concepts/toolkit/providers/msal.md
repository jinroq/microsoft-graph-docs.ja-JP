---
title: MSAL プロバイダ
description: MSAL のプロバイダーは MSAL を使用してユーザーにサインインし、トークンを取得して Microsoft Graph で使用します。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: b66fd9a640c6baa84767e1ab08821b80384a5464
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/26/2019
ms.locfileid: "35243049"
---
# <a name="msal-provider"></a>MSAL プロバイダ

MSAL プロバイダーは、 [msal .js](https://github.com/AzureAD/microsoft-authentication-library-for-js)を使用してユーザーにサインインし、Microsoft Graph で使用するトークンを取得します。

詳細については、「 [providers](../providers.md)」を参照してください。

## <a name="get-started"></a>作業の開始

MSAL プロバイダーは、HTML または JavaScript で初期化できます。

### <a name="initialize-in-your-html-page"></a>HTML ページでの初期化

新しいプロバイダーを作成する最も簡単な方法は、HTML で MSAL プロバイダーを初期化することです。 `mgt-msal-provider`コンポーネントを使用して、**クライアント id**とその他のプロパティを設定します。 これにより、すべて`UserAgentApplication`の認証とトークンの取得で使用される新しいインスタンスが作成されます。

```html
<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"
                   login-type="redirect/popup"
                   authority=""></mgt-msal-provider>
```

>**注:**`login-type` `authority`

### <a name="initialize-in-javascript"></a>JavaScript での初期化

JavaScript でプロバイダーを初期化することで、より多くのオプションを提供できます。

```ts
import {Providers, MsalProvider} from '@microsoft/mgt'
import {UserAgentApplication} from "msal";

Providers.globalProvider = new MsalProvider(config: MsalConfig);
```

MsalConfig は次のとおりです。

```ts
interface MsalConfig {
  clientId: string;
  scopes?: string[];
  authority?: string;
  loginType?: LoginType;
  options?: Configuration; // msal js Configuration object
}
```

を`clientId`指定する必要があります (新しい`UserAgentApplication`を作成する場合)。

詳細については、 [Msal のドキュメント](https://github.com/AzureAD/microsoft-authentication-library-for-js/wiki/MSAL-basics)を参照してください。

## <a name="creating-an-appclient-id"></a>アプリ/クライアント ID の作成

アプリを登録し、クライアント ID を取得する方法の詳細については、「[アプリのクイックスタートを登録](https://docs.microsoft.com/en-us/azure/active-directory/develop/quickstart-register-app)する」を参照してください。

>**注:** MSAL では、OAuth の暗黙的フローのみがサポートされています。 Azure Portal でアプリケーションの暗黙的フローを有効にしてください (既定では有効になっていません)。 [**認証**] で、[**暗黙的な付与**] セクションを見つけて、**アクセストークン**と**ID トークン**のチェックボックスをオンにします。
