---
title: Microsoft Graph を呼び出すためのトークンの取得
description: Microsoft Graph を呼び出すために、アプリは Microsoft のクラウド ID サービス Azure Active Directory (Azure AD) からアクセス トークンを取得する必要があります。
author: jackson-woods
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5438dfd81dddb2089792f37a42f87070d337a6b4
ms.sourcegitcommit: 255061099661a38278140675db4cbadbdca9be7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/07/2019
ms.locfileid: "29760924"
---
# <a name="get-access-tokens-to-call-microsoft-graph"></a>Microsoft Graph を呼び出すためのアクセス トークンの取得

Microsoft Graph を呼び出すために、アプリは Microsoft のクラウド ID サービス Azure Active Directory (Azure AD) からアクセス トークンを取得する必要があります。アクセス トークンには、アプリとアプリに付与されているアクセス許可に関する情報 (要求) が含まれています (このアクセス許可は、Microsoft Graph を通じて利用できるリソースと API に対応するものです)。アクセス トークンを取得するためには、アプリを Azure AD で認証できるようにすることと、そのアプリが必要とする Microsoft Graph リソースへのアクセスをユーザーまたは管理者が承認することが必要です。 

ここでは、アクセス トークンと Azure AD の概要、およびアプリでアクセス トークンを取得する方法について説明します。トークンを取得するためのアプリと Azure AD との統合について既に詳しく理解している場合は、「[次の手順](#next-steps)」までスキップして、Microsoft Graph に固有の情報とサンプルを参照してください。 

> **重要:** 条件付きアクセス ポリシーの Microsoft Graph への適用方法は変更されています。 条件付きアクセス ポリシーが構成されるシナリオを処理するよう、アプリケーションを更新する必要があります。 詳細およびガイダンスについては、「[Azure Active Directory の条件付きアクセスについての開発者ガイド](https://docs.microsoft.com/azure/active-directory/develop/active-directory-conditional-access-developer)」を参照してください。

## <a name="what-is-an-access-token-and-how-do-i-use-it"></a>アクセス トークンの内容と使用方法について

Azure AD から発行されるアクセス トークンは、Base 64 でエンコードされた JSON Web トークン (JWT) です。これに含まれている情報 (要求) は、呼び出し元の検証と、呼び出し元が要求している操作を実行するための適切なアクセス許可が付与されていることの確認のために、Azure AD によって保護されている Web API (Microsoft Graph など) が使用します。Microsoft Graph の呼び出し時には、アクセス トークンを不透明なものとして扱うことができます。アクセス トークンは、常にトランスポート層セキュリティ (HTTPS) などのセキュリティで保護されたチャネルを通じて送信する必要があります。

次に、Azure AD アクセス トークンの例を示します。

`EwAoA8l6BAAU7p9QDpi/D7xJLwsTgCg3TskyTaQAAXu71AU9f4aS4rOK5xoO/SU5HZKSXtCsDe0Pj7uSc5Ug008qTI+a9M1tBeKoTs7tHzhJNSKgk7pm5e8d3oGWXX5shyOG3cKSqgfwuNDnmmPDNDivwmi9kmKqWIC9OQRf8InpYXH7NdUYNwN+jljffvNTewdZz42VPrvqoMH7hSxiG7A1h8leOv4F3Ek/oeJX6U8nnL9nJ5pHLVuPWD0aNnTPTJD8Y4oQTp5zLhDIIfaJCaGcQperULVF7K6yX8MhHxIBwek418rKIp11om0SWBXOYSGOM0rNNN59qNiKwLNK+MPUf7ObcRBN5I5vg8jB7IMoz66jrNmT2uiWCyI8MmYDZgAACPoaZ9REyqke+AE1/x1ZX0w7OamUexKF8YGZiw+cDpT/BP1GsONnwI4a8M7HsBtDgZPRd6/Hfqlq3HE2xLuhYX8bAc1MUr0gP9KuH6HDQNlIV4KaRZWxyRo1wmKHOF5G5wTHrtxg8tnXylMc1PKOtaXIU4JJZ1l4x/7FwhPmg9M86PBPWr5zwUj2CVXC7wWlL/6M89Mlh8yXESMO3AIuAmEMKjqauPrgi9hAdI2oqnLZWCRL9gcHBida1y0DTXQhcwMv1ORrk65VFHtVgYAegrxu3NDoJiDyVaPZxDwTYRGjPII3va8GALAMVy5xou2ikzRvJjW7Gm3XoaqJCTCExN4m5i/Dqc81Gr4uT7OaeypYTUjnwCh7aMhsOTDJehefzjXhlkn//2eik+NivKx/BTJBEdT6MR97Wh/ns/VcK7QTmbjwbU2cwLngT7Ylq+uzhx54R9JMaSLhnw+/nIrcVkG77Hi3neShKeZmnl5DC9PuwIbtNvVge3Q+V0ws2zsL3z7ndz4tTMYFdvR/XbrnbEErTDLWrV6Lc3JHQMs0bYUyTBg5dThwCiuZ1evaT6BlMMLuSCVxdBGzXTBcvGwihFzZbyNoX+52DS5x+RbIEvd6KWOpQ6Ni+1GAawHDdNUiQTQFXRxLSHfc9fh7hE4qcD7PqHGsykYj7A0XqHCjbKKgWSkcAg==`

Microsoft Graph を呼び出す場合は、アクセス トークンをベララー トークンとして HTTP 要求の Authorization ヘッダーに添付します。その例として、サインインしているユーザーのプロファイル情報を返す呼び出しを示します (読みやすくするために、アクセス トークンは切り詰められています)。

```
HTTP/1.1
Authorization: Bearer EwAoA8l6BAAU ... 7PqHGsykYj7A0XqHCjbKKgWSkcAg==
Host: graph.microsoft.com`
GET https://graph.microsoft.com/v1.0/me/
```

## <a name="what-are-microsoft-graph-permissions"></a>Microsoft Graph のアクセス許可とは
Microsoft Graph は、制御対象のリソースに対して、きめ細かい豊富なアクセス許可のセットを公開しています。このアクセス許可は文字列として表現され、アプリに Microsoft Graph のリソース (ユーザー、グループ、ユーザー メールなど) へのアクセスを許可します。次に例を示します。

- _User.Read_ は、サインインしているユーザーのプロファイルをアプリで読み取れるようにします。
- _Mail.Send_ は、サインインしているユーザーの代わりにアプリでメールを送信できるようにします。

アクセス許可には 2 つの種類があります。

- 委任されたアクセス許可は、ユーザーの存在によって実行するアプリに使用します。ユーザーの特権は、ユーザーの代わりに Microsoft Graph を呼び出すアプリに委任されます。このようなアクセス許可の多くはユーザーが同意できますが、管理者の同意が必要になるものもあります。  
- アプリケーションのアクセス許可は、ユーザーなしで実行するアプリに使用します。これに該当するものは、アプリに組織内で広範な特権を付与することが多く、常に管理者の同意が必要になります。

Microsoft Graph のアクセス許可の完全なリスト、および委任されたアクセス許可とアプリケーションのアクセス許可の相違点については、「[アクセス許可のリファレンス](permissions-reference.md)」を参照してください。

## <a name="where-does-my-app-get-an-access-token"></a>アプリのアクセス トークンを取得する場所
アプリは、Microsoft のクラウド ID サービス Azure Active Directory (Azure AD) からアクセス トークンを取得します。アクセス トークンを取得するために、アプリは OAuth 2.0 と OpenID Connect 1.0 の仕様で定義されている業界標準のプロトコルを使用して、HTTP 要求および応答を Azure AD と交換します。このプロトコルにより、Azure AD での安全な認証とアクセス トークンの取得にアプリが使用する Azure AD エンドポイントとエンドポイントとの交換 (認証フロー) 記述します。  

非常に単純なレベルでは、アプリはアクセス トークンを取得するために、次に示すエンドポイントと HTTP 要求を交換します。

- `/authorize` エンドポイントは、Azure AD での認証とアプリが必要とするアクセス許可への同意を得るために、アプリがユーザーを転送できるエンドポイントです。
- `/token` エンドポイントは、ユーザーの同意が得られたアプリがアクセス トークンを取得できるエンドポイントです。

(注 : これらの定義は固定されたものではありません。アプリが使用するプロトコルによって、`/authorize` エンドポイントから直接アクセス トークンを取得することも、`/token` エンドポイントで直接認証することもあります)。 

次に、Azure AD v2.0 で公開されている 1 セットの `/authorize` エンドポイントと `/token` エンドポイントの例を示します。

```
https://login.microsoftonline.com/common/oauth2/v2.0/authorize
https://login.microsoftonline.com/common/oauth2/v2.0/token

```
Azure AD は、Azure AD と Azure AD v2.0 の 2 つのエンドポイントのセットを公開しています。これらの主な相違点は、Azure AD エンドポイントが職場または学校アカウント (Azure AD テナントに関連付けられたアカウント) のみをサポートし、Azure AD v2.0 が Microsoft アカウント (_Live.com_ アカウントや _outlook.com_ アカウントなど) もサポートしていることです。そのため、Azure AD エンドポイントを使用する場合は、アプリの対象が組織のみになりますが、Azure AD v2.0 の場合は対象が消費者と組織の両方になります。 

Azure AD エンドポイントから得られるトークンは、Azure AD v2.0 エンドポイントから得られるトークンとの互換性がありません。そのため、実稼働に向けたアプリの作成を始める前に、どちらかのエンドポイントに決定しておく必要があります。Azure AD v2.0 エンドポイントのほうが新しく、機能の追加が続けられているため、いくつかの重要な制限があります。この制限は、実稼働のアプリに使用するエンドポイントを判断する際に考慮に入れる必要があります。詳細については、「[Azure AD エンドポイントか Azure AD v2.0 エンドポイントかを決定する](#deciding-between-the-azure-ad-and-azure-ad-v20-endpoints)」を参照してください。

## <a name="whats-the-difference-between-oauth-20-and-openid-connect"></a>OAuth 2.0 と OpenID Connect の相違点について

OAuth 2.0 は、認証プロトコルの 1 つです。これにより、アプリがアクセス トークンを取得する方法を定義します。つまり、Azure AD で直接認証してアクセス トークンを取得するか、Azure AD での認証とアプリが要求するアクセス許可の同意を得るためにユーザーをリダイレクトしてアクセス トークンを取得するかを定義します。最初のケースでは、アプリは、それ自体として Microsoft Graph の呼び出しに使用できるアクセス トークンを取得します。2 番目のケースでは、アプリは、ユーザーの代わりに Microsoft Graph の呼び出しに使用できるアクセス トークンを取得します。ただし、OAuth 2.0 の場合、アプリはユーザーに関する情報 (ユーザーがどのように Azure AD で認証されたかに関する情報) を受け取りません。OAuth 2.0 のフローは、多くの場合、既にユーザーの ID がわかっているモバイルやネイティブ アプリで使用されます。または、ユーザーの代わりではなく、アプリ自体の ID で Microsoft Graph を呼び出すバックグラウンド サービスやデーモンなどのアプリで使用されます。

OpenID Connect は、OAuth 2.0 を拡張することで ID 層を提供しています。OpenID Connect の場合、アプリはアクセス トークンに加えて、ID トークンも Azure AD から取得できます。OpenID Connect の ID トークンには、ユーザーの ID と、そのユーザーが認証された方法および認証された場所についての要求が含まれています。OpenID Connect のフローは、通常、シングル ページ アプリ (SPA) を含む Web アプリで使用されます。このようなアプリは、アクセス トークンを要求したユーザーに応じて動作をカスタマイズする際に ID トークンを使用できます。また、多くの場合、Azure AD へのユーザーのサインインを外部に委託してシングル サインオン (SSO) のようなエクスペリエンスを可能にします。

## <a name="what-kind-of-apps-can-i-call-microsoft-graph-from"></a>Microsoft Graph を呼び出せるアプリの種類について
Microsoft Graph は、次に示す種類のアプリから呼び出せます。 

- **ネイティブ アプリ**: デスクトップ、タブレット、携帯電話などのデバイス上で実行するアプリ。こうしたアプリは、ユーザー プレゼンテーションに iOS、Android、Windows などのデバイスにネイティブなオペレーティング システム (OS) を使用し、ユーザーの代わりに Microsoft Graph を呼び出します。
- **Web アプリ**: サーバー上で実行し、ユーザー エージェント (通常は Web ブラウザー) を通じてサインインしているユーザーと対話するアプリ。プレゼンテーション層のほとんどはサーバーで処理され、Microsoft Graph への呼び出しはユーザーの代わりにサーバー側で実行されます。
- **シングル ページ アプリ (SPA)**: ブラウザーのクライアント側スクリプトで大部分のプレゼンテーション層を処理する上質なユーザー エクスペリエンスを備えた Web アプリケーション。Microsoft Graph の呼び出しは、クライアント側のスクリプト (AJAX などのテクノロジと Angular.js などのフレームワークを使用) から実行します。ユーザーの代わりに呼び出しが実行されます。
- **バックグラウンド サービス/デーモン**: ユーザーの存在なしでサーバー上で実行し、独自の ID で Microsoft Graph を呼び出すバックグラウンド サービスとデーモン。
- **Web API**: クライアント アプリは、ユーザーの代わりに Web API (Azure AD でセキュリティ保護された API) を呼び出して、この API が Microsoft Graph を呼び出すます。Azure AD エンドポイントでサポートされています。Azure AD v2.0 エンドポイントについては、クライアントと Web API が同じアプリケーション ID を持つ場合にのみサポートされます (たとえば、Web API バック エンドを呼び出すネイティブ アプリなど)。 

## <a name="how-do-i-get-my-app-talking-to-azure-ad-and-microsoft-graph"></a>アプリで Azure AD および Microsoft Graph と対話する方法
アプリで Azure AD からトークンを取得するには、まず、そのアプリを登録しておく必要があります。Azure AD v2.0 エンドポイントの場合は、アプリの登録に [Microsoft アプリ登録ポータル](https://apps.dev.microsoft.com/)を使用します。Azure AD エンドポイントの場合は、[Azure ポータル](https://portal.azure.com/)を使用します。この登録では、アプリと Azure AD を統合して、アプリがトークンを取得する位置と ID を設定します。その内容は次のとおりです。

- **アプリケーション ID**:Azure AD によって割り当てられる一意識別子。 
- **リダイレクト URI/URL**: アプリが Azure AD からの応答を受け取る 1 つ以上のエンドポイント (ネイティブ アプリとモバイル アプリの場合は、Azure AD によって割り当てられる URI になります)。
- **アプリケーション シークレット**: アプリが Azure AD での認証に使用するパスワードまたは公開鍵/秘密鍵のペア (ネイティブ アプリまたはモバイル アプリの場合は不要です)。

Azure AD エンドポイントを使用するアプリの場合は、Microsoft Graph のアクセス許可を事前構成しておく必要もあります。これは、アプリの登録時に必要になります。Azure AD v2.0 エンドポイントを使用するアプリの場合は、アクセス許可の事前構成が必要なことも不要なこともあります。 

登録時には構成済みのプロパティが通信で使用されます。たとえば、次に示すトークン要求の場合、*client_id* は *アプリケーション ID*、*redirect_uri* はアプリの登録済*リダイレクト URI* の 1 つ、*client_secret* は *アプリケーション シークレット*です。 

```
// Line breaks for legibility only

POST /common/oauth2/v2.0/token HTTP/1.1
Host: https://login.microsoftonline.com
Content-Type: application/x-www-form-urlencoded

client_id=6731de76-14a6-49ae-97bc-6eba6914391e
&scope=user.read%20mail.read
&code=OAAABAAAAiL9Kn2Z27UubvWFPbm0gLWQJVzCTE9UkP3pSx1aXxUjq3n8b2JRLk4OxVXr...
&redirect_uri=http%3A%2F%2Flocalhost%2Fmyapp%2F
&grant_type=authorization_code
&client_secret=JqQX2PNo9bpM0uEihUPzyrh    // NOTE: Only required for web apps
```

## <a name="are-there-authentication-libraries-available"></a>利用可能な認証ライブラリについて
ほとんどの開発者と同じように、Azure AD との対話式操作を管理するために、認証ライブラリを使用することになります。認証ライブラリは、開発者からプロトコルの詳細の多く (検証、Cookie の処理、トークンのキャッシュ、安全な接続の維持など) を取り除き、アプリの開発に集中できるようにします。Microsoft は、Azure AD エンドポイントと Azure AD v2.0 エンドポイントの両方に対応したオープン ソースのクライアント ライブラリとサーバー ミドルウェアを公開しています。 

Azure AD v2.0 エンドポイント:  

- Microsoft Authentication Library (MSAL) クライアント ライブラリは、.NET、JavaScript、Android、および Objective-c で利用できます。すべてのプラットフォームが実稼働対応のプレビューであり、大きな変更が導入されていますが、Microsoft によりアップグレードの経路が保証されています。
- Microsoft のサーバー ミドルウェアは、.NET コアと ASP.NET (OWIN OpenID Connect および OAuth)、および Node.js (Microsoft Azure AD Passport.js) で利用できます。 
- v2.0 エンドポイントには、多数のサード パーティ製認証ライブラリとの互換性があります。

Microsoft クライアント ライブラリ、Microsoft サーバー ミドルウェア、および互換性のあるサード パーティ製ライブラリの完全なリストについては、「[Azure Active Directory v2.0 認証ライブラリ](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-libraries)」を参照してください。

Azure AD エンドポイント: 

- Active Directory Authentication Library (ADAL) クライアント ライブラリは、より多くのプラットフォームで使用できます。 
- Microsoft によるサーバー ミドルウェアは、.NET コアと ASP.NET、および Node.js で使用できます。 

Microsoft クライアント ライブラリとサーバー ミドルウェアの完全なリストについては、「[Azure Active Directory 認証ライブラリ](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-libraries)」を参照してください。

## <a name="deciding-between-the-azure-ad-and-azure-ad-v20-endpoints"></a>Azure AD エンドポイントか Azure AD v2.0 エンドポイントかを決定する

Azure AD は、2 つのエンドポイントのセット Azure AD と Azure AD v2.0 を公開しています。Microsoft Graph を呼び出す際に使用するアクセス トークンは、このエンドポイントで取得できます。それぞれのエンドポイントから受け取ったトークンには、互換性がありません。Microsoft Graph のサンプルを実行する場合や機能を調べる場合には、Azure AD エンドポイントを選択しておけば特に問題はありません。ただし、実稼働アプリの開発を始める場合は、まず、目的のシナリオに最適なエンドポイントがどちらになるかを決定する必要があります。次に、この決定の際に役立つ一般的なガイドラインのいくつかを示しますが、最新の包括的な情報については、Azure Active Directory ドキュメントの「[v2.0 エンドポイントの使用が適しているかどうかを判断するには](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-limitations)」を参照する必要があります。 

Azure AD と Azure AD v2.0 の主な相違点は次のとおりです。

* Azure AD は、職場または学校アカウントのみをサポートします。このアカウントは、Azure AD テナントに関連付けられているものです。これは、アプリの対象が組織のみになることを意味します。
* Azure AD v2.0 は、職場と学校アカウントと、Microsoft  アカウント (_live.com_ アカウントや _outlook.com_ アカウントなど) の両方をサポートします。これは、アプリの対象が v2.0 エンドポイントを使用する消費者と組織の両方になることを意味します。 

Azure AD v2.0 いくつかの追加的な利点があります。次に例を示します。

* アプリでは、複数のプラットフォームに 1 つのアプリケーション ID を使用できます。これにより、開発者と管理者は、アプリの管理が簡単になります。
* [動的同意と増分同意をサポートしています](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-compare#incremental-and-dynamic-consent)。この機能により、アプリは、ユーザーに同意を求める要求とアプリに必要な機能を組み合わせて、実行時に追加のアクセス許可を要求できるようになります。これにより、最初のサインイン時にアクセス許可の長大なリストに同意を求めるものよりも快適なエクスペリエンスをユーザーに提供できます。  

Azure AD v2.0 は Azure AD よりも新しく、機能の追加が続けられているため、v2.0 エンドポイントにはいくつかの制限があります。エンドポイントを決定する際には、この制限を考慮に入れる必要があります。次に例を示します。

* 一部の機能は、まだ v2.0 では完全に実装されていません。たとえば、エンタープライズのお客様がモバイル セキュリティ機能 ([デバイスへの条件付きアクセス](https://azure.microsoft.com/documentation/articles/active-directory-conditional-access-device-policies)など) をオンにすると、アプリが動作しなくなることがあります。
* クラウド ソリューション プロバイダー アプリは呼び出せません。
* [フェデレーション テナントの統合 Windows 認証](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-limitations#limitations)はサポートされていません。このため、フェデレーション Azure AD テナントのユーザーは、オンプレミスの Active Directory インスタンスでの自動認証ができなくなります。ユーザーは、自分の資格情報を再入力する必要があります。

Azure AD v2.0 エンドポイントと Azure AD エンドポイントの相違点の詳細については、「[v2.0 エンドポイントの変更点](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-compare)」を参照してください。

>**重要**
>
>**実稼働用のアプリを開発するときには、使用するエンドポイントを決定する前に、[v2.0 エンドポイントの使用が適しているかどうか](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-limitations)に関する記事を参照してください。**

## <a name="next-steps"></a>次のステップ

アプリの登録が済むと、開始準備は完了です。

- ユーザーの代わりに Microsoft Graph を呼び出すアプリのアクセス トークンを取得する簡単な手順については、「[ユーザーの代わりにアクセスを取得](auth-v2-user.md)」を参照してください。
- ユーザーなしで Microsoft Graph を呼び出すアプリのアクセス トークンを取得する簡単な手順については、「[ユーザーなしでアクセスを取得](auth-v2-service.md)」を参照してください。
- Microsoft Graph で使用可能なアクセス許可を確認する場合は、「[アクセス許可](permissions-reference.md)」を参照してください。
- Microsoft Graph によるパートナー管理型顧客データへのアクセスについて Microsoft クラウド ソリューション プロバイダーに興味がある場合は、「[アプリケーション アクセスの管理 (CSP)](auth-cloudsolutionprovider.md)」を参照してください。


コードの作成準備が整ったら、次に示すリソースを使用できるようになります。これらのリソースは、Azure AD による認証と承認をアプリに実装する際に役立ちます。

### <a name="microsoft-graph-training-and-samples"></a>Microsoft Graph のトレーニングとサンプル
すぐに使い始めることができるように、さまざまなプラットフォーム上で API を認証して使用する方法を示した、一連のトレーニング モジュールとその他のリソースを作成しました。 

- [概要](https://developer.microsoft.com/ja-JP/graph/get-started)のページで、お好みのプラットフォーム向けのライブラリ、サンプル、トレーニング コンテンツなどのリソースを見つけてください。 
- お使いのプラットフォーム向けに構成済みのサンプルをすぐに実行するには、「[Microsoft Graph のクイック スタート](https://developer.microsoft.com/ja-JP/graph/quick-start)」を参照してください。
- GitHub では [Microsoft Graph サンプル](https://github.com/microsoftgraph?utf8=%E2%9C%93&q=sample&type=&language=)を公開しています。


### <a name="azure-active-directory-samples-and-documentation"></a>Azure Active Directory のサンプルとドキュメント 
Azure AD のドキュメントには、特に Azure AD での認証と承認に焦点を合わせた記事とサンプルが含まれています。

Azure AD v2.0 エンドポイント:  

- 最も簡単な開始地点は、[Azure AD v2.0 エンドポイントのドキュメント](https://docs.microsoft.com/azure/active-directory/develop/active-directory-appmodel-v2-overview)です。この記事には、概要、プロトコルに関するドキュメント、および各種プラットフォームに対応している入門記事へのリンクが記載されています。これらすべてのリンクは、開発するアプリの種類ごとに編成されています。 
- クライアントまたはサーバー認証ライブラリごとのサンプルについては、「[Azure Active Directory v2.0 認証ライブラリ](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-libraries)」を参照してください。 
- また、プラットフォームごとの Azure AD サンプルは、「[Azure のコード サンプル](https://azure.microsoft.com/resources/samples/?service=active-directory)」で見つかります。注意: エンドポイントのバージョンを検索条件にすることはできません。 

Azure AD エンドポイント:  

- 最も簡単な開始地点は、「[開発者のための Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-developers-guide)」です。この記事には、概要、プロトコルに関するドキュメント、および各種プラットフォームに対応した入門記事へのリンクが記載されています。これらのリンクは、開発するアプリの種類ごとに編成されています。 
- クライアントまたはサーバーの認証ライブラリごとのサンプルのリストについては、「[Azure Active Directory 認証ライブラリ](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-libraries)」を参照してください。 
- アプリの種類およびプラットフォームごとのサンプルのリストは、「[Azure Active Directory のコード例](https://docs.microsoft.com/azure/active-directory/develop/active-directory-code-samples)」を参照してください。
- また、プラットフォームごとの Azure AD サンプルは、「[Azure のコード サンプル](https://azure.microsoft.com/resources/samples/?service=active-directory)」で見つかります。注意: エンドポイントのバージョンを検索条件にすることはできません。 


## <a name="see-also"></a>関連項目

- [Azure Active Directory エンドポイントに関するドキュメント](https://docs.microsoft.com/azure/active-directory/develop/active-directory-developers-guide)
- [Azure Active Directory v2.0 エンドポイントに関するドキュメント](https://docs.microsoft.com/azure/active-directory/develop/active-directory-appmodel-v2-overview)
