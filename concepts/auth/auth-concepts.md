---
front_matter_title: Basics
description: Microsoft Graph を呼び出すには、アプリが Microsoft ID プラットフォームからアクセス トークンを取得する必要があります。
author: matt-steele
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7e532867c9d92e2c2a7dd27e2e17a51fcbc1d2d4
ms.sourcegitcommit: 118b3cea623d9abec666c9d295a25f18a43a8aee
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/17/2019
ms.locfileid: "35017767"
---
# <a name="authentication-and-authorization-basics-for-microsoft-graph"></a>Microsoft Graph の認証と承認の基本方法

Microsoft Graph を呼び出すには、アプリが Microsoft ID プラットフォームからアクセス トークンを取得する必要があります。 アクセス トークンには、アプリとアプリに付与されているアクセス許可に関する情報が含まれています。このアクセス許可は、Microsoft Graph を通じて利用できるリソースと API に対応するものです。 アクセス トークンを取得するには、アプリを Microsoft ID プラットフォームで登録し、そのアプリが必要とする Microsoft Graph リソースへのアクセスをユーザーまたは管理者が承認する必要があります。 

このトピックでは、アクセス トークンと Microsoft ID プラットフォームの概要、アプリでアクセス トークンを取得する方法について説明します。 トークンを取得するためのアプリと Microsoft ID プラットフォームとの統合について既に詳しく理解している場合は、[[次の手順](#next-steps)] のセクションまでスキップして、Microsoft Graph に固有の情報とサンプルを参照してください。

## <a name="access-tokens"></a>アクセス トークン

Microsoft ID プラットフォームから発行されるアクセス トークンは、Base 64 でエンコードされた JSON Web トークン (JWT) です。 これに含まれている情報 (要求) は、呼び出し元の検証と、呼び出し元が要求している操作を実行するための適切なアクセス許可が付与されていることの確認のために、Microsoft ID プラットフォームによって保護されている Web API (Microsoft Graph など) が使用します。 Microsoft Graph の呼び出し時には、アクセス トークンを不透明なものとして扱うことができます。 アクセス トークンは、常にトランスポート層セキュリティ (HTTPS) などのセキュリティで保護されたチャネルを通じて送信する必要があります。

Microsoft ID プラットフォームのアクセス トークンの例を次のとおりです。

```jwt
EwAoA8l6BAAU7p9QDpi/D7xJLwsTgCg3TskyTaQAAXu71AU9f4aS4rOK5xoO/SU5HZKSXtCsDe0Pj7uSc5Ug008qTI+a9M1tBeKoTs7tHzhJNSKgk7pm5e8d3oGWXX5shyOG3cKSqgfwuNDnmmPDNDivwmi9kmKqWIC9OQRf8InpYXH7NdUYNwN+jljffvNTewdZz42VPrvqoMH7hSxiG7A1h8leOv4F3Ek/oeJX6U8nnL9nJ5pHLVuPWD0aNnTPTJD8Y4oQTp5zLhDIIfaJCaGcQperULVF7K6yX8MhHxIBwek418rKIp11om0SWBXOYSGOM0rNNN59qNiKwLNK+MPUf7ObcRBN5I5vg8jB7IMoz66jrNmT2uiWCyI8MmYDZgAACPoaZ9REyqke+AE1/x1ZX0w7OamUexKF8YGZiw+cDpT/BP1GsONnwI4a8M7HsBtDgZPRd6/Hfqlq3HE2xLuhYX8bAc1MUr0gP9KuH6HDQNlIV4KaRZWxyRo1wmKHOF5G5wTHrtxg8tnXylMc1PKOtaXIU4JJZ1l4x/7FwhPmg9M86PBPWr5zwUj2CVXC7wWlL/6M89Mlh8yXESMO3AIuAmEMKjqauPrgi9hAdI2oqnLZWCRL9gcHBida1y0DTXQhcwMv1ORrk65VFHtVgYAegrxu3NDoJiDyVaPZxDwTYRGjPII3va8GALAMVy5xou2ikzRvJjW7Gm3XoaqJCTCExN4m5i/Dqc81Gr4uT7OaeypYTUjnwCh7aMhsOTDJehefzjXhlkn//2eik+NivKx/BTJBEdT6MR97Wh/ns/VcK7QTmbjwbU2cwLngT7Ylq+uzhx54R9JMaSLhnw+/nIrcVkG77Hi3neShKeZmnl5DC9PuwIbtNvVge3Q+V0ws2zsL3z7ndz4tTMYFdvR/XbrnbEErTDLWrV6Lc3JHQMs0bYUyTBg5dThwCiuZ1evaT6BlMMLuSCVxdBGzXTBcvGwihFzZbyNoX+52DS5x+RbIEvd6KWOpQ6Ni+1GAawHDdNUiQTQFXRxLSHfc9fh7hE4qcD7PqHGsykYj7A0XqHCjbKKgWSkcAg==
```

Microsoft Graph を呼び出す場合は、アクセス トークンをベアラー トークンとして HTTP 要求の Authorization ヘッダーに添付します。 その例として、サインインしているユーザーのプロファイル情報を返す呼び出しを次に示します (読みやすくするために、アクセス トークンは短くされています)。

```http
HTTP/1.1
Authorization: Bearer EwAoA8l6BAAU ... 7PqHGsykYj7A0XqHCjbKKgWSkcAg==
Host: graph.microsoft.com`
GET https://graph.microsoft.com/v1.0/me/
```

## <a name="register-your-app-with-the-microsoft-identity-platform"></a>Microsoft ID プラットフォームにアプリを登録する

アプリが Microsoft ID プラットフォームからトークンを取得する前に、[Azure ポータル](https://portal.azure.com/)に登録する必要があります。 登録によりアプリが Microsoft ID プラットフォームと統合され、次のようなトークンを取得する際に使用する情報を確立します。

- **アプリケーション ID**: Microsoft ID プラットフォームによって割り当てられた一意の識別子。 
- **リダイレクト URI または URL**: アプリが Microsoft ID プラットフォームから応答を受信する 1 つまたは複数のエンドポイント (ネイティブ アプリとモバイル アプリにおいては、Microsoft ID プラットフォームが割り当てた URI です)。
- **アプリケーション シークレット**: アプリが Microsoft ID プラットフォームでの認証に使用するパスワードまたは公開鍵や秘密鍵のペア  (ネイティブ アプリまたはモバイル アプリの場合は不要です)。

登録時には構成済みのプロパティが要求で使用されます。 たとえば、次に示すトークン要求の場合、*client_id* は *アプリケーション ID*、*redirect_uri* はアプリの登録済*リダイレクト URI* の 1 つ、*client_secret* は *アプリケーション シークレット*です。

```http
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

## <a name="microsoft-graph-permissions"></a>Microsoft Graph のアクセス許可

Microsoft Graph はユーザー、グループ、メールなどのリソースに対するアプリのアクセス権を制御する詳細なアクセス許可を公開します。 開発者は Microsoft Graph に要求するアクセス許可を決定します。 アプリにサインインした場合、そのアクセス許可に同意するか否かは、ユーザーか、場合によっては管理者が決定します。 ユーザーが同意すると、アプリは必要なリソースと API にアクセスできるようになります。 サインイン ユーザーを必要としないアプリの場合、アクセス許可は、アプリのインストール時に管理者が事前に同意できます。

Microsoft Graph には次の 2 つの種類のアクセス許可があります。 

- **委任されたアクセス許可**は、サインインしているユーザーが存在するアプリで使用します。 これに該当するアプリの場合は、ユーザーまたは管理者がアプリの要求するアクセス許可に同意します。アプリには、Microsoft Graph の呼び出し時に、サインインしているユーザーとして動作できます。 一部の委任されたアクセス許可は非管理ユーザーの同意によって付与できますが、高度な特権が付与されるアクセス許可には[管理者の同意](https://docs.microsoft.com/ja-JP/azure/active-directory/develop/active-directory-v2-scopes#using-the-admin-consent-endpoint)が必要になります。  

- **アプリケーションのアクセス許可**は、サインインしているユーザーが存在しないアプリで使用します。たとえば、バックグラウンド サービスやデーモンとして実行されるアプリです。 アプリケーションのアクセス許可には、[管理者のみ同意](https://docs.microsoft.com/ja-JP/azure/active-directory/develop/active-directory-v2-scopes#requesting-consent-for-an-entire-tenant)できます。 

_有効なアクセス許可_は、アプリが Microsoft Graph に要求を出すときに付与されるアクセス許可です。アプリに付与される委任されたアクセス許可とアプリケーションのアクセス許可の相違点について理解することに加えて、Microsoft Graph の呼び出し時の有効なアクセス許可についても理解することが重要です。

- 委任されたアクセス許可の場合、アプリの有効なアクセス許可は、アプリに付与されている委任されたアクセス許可 (同意によって付与) と現在サインインしているユーザーの特権が重なる範囲に収まります。 サインインしているユーザーよりも多くの特権がアプリに付与されることはありません。 組織では、サインインしているユーザーの特権は、ポリシーで決まることもあれば、1 つ以上の管理者ロールのメンバーシップで決まることもあります。 管理者ロールに関する詳細については、「[Azure Active Directory での管理者ロールの割り当て](https://docs.microsoft.com/ja-JP/azure/active-directory/active-directory-assign-admin-roles)」を参照してください。<br/><br/>たとえば、委任されたアクセス許可として User.ReadWrite.All がアプリに付与されているとします。 通常、このアクセス許可は、組織内の全ユーザーのプロフィールを読み取り、更新するアクセス許可をアプリに付与します。 サインインしているユーザーが全体管理者の場合、アプリは、組織内のすべてのユーザーのプロファイルを更新できるようになります。 ただし、サインインしているユーザーが管理者ロールに含まれていない場合、アプリは、そのサインインしているユーザーのプロファイルのみを更新できるようになります。 組織にいる他のユーザーのプロフィールは更新できません。アプリが代理するアクセス許可を持つユーザーに、そういった権限が付与されていないためです。
  
- アプリケーションのアクセス許可の場合、アプリの有効なアクセス許可は、そのアクセス許可が暗示する完全なレベルの権限になります。 たとえば、アプリケーションのアクセス許可として User.ReadWrite.All が付与されているアプリは、組織内の全ユーザーのプロフィールを更新できます。

>**注** 既定では、次のデータ セットに対するアプリケーション アクセス許可が与えられているアプリは、組織内のすべてのメールボックスにアクセスできます。

- [予定表](../permissions-reference.md#calendars-permissions)
- [連絡先](../permissions-reference.md#contacts-permissions)
- [メール](../permissions-reference.md#mail-permissions)
- [メールボックス設定](../permissions-reference.md#mail-permissions)

>管理者は[アプリケーション アクセス ポリシー](../auth-limit-mailbox-access.md)を構成して、アプリのアクセスを_特定_のメールボックスに制限することができます。 

Microsoft Graph に委任されたアクセス許可とアプリケーションのアクセス許可の詳細なリスト、管理者の同意が必要なアクセス許可については、「[アクセス許可のリファレンス](../permissions-reference.md)」を参照してください。

## <a name="getting-an-access-token"></a>アクセス トークンの取得

多くの開発者と同じように、認証ライブラリを使用し、Microsoft ID プラットフォームとのトークンの連携を管理することになります。 認証ライブラリは、開発者からプロトコルの詳細の多く (検証、Cookie の処理、トークンのキャッシュ、安全な接続の維持など) を取り去り、アプリの開発に集中できるようにします。 Microsoft はオープン ソース クライアント ライブラリとサーバー ミドルウェアを公開します。

Microsoft ID プラットフォームのエンドポイントの場合:

- Microsoft Authentication Library (MSAL) クライアント ライブラリは、.NET、JavaScript、Android、および Objective-c で利用できます。すべてのプラットフォームが実稼働対応のプレビューであり、大きな変更が導入されていますが、Microsoft によりアップグレードの経路が保証されています。
- Microsoft のサーバー ミドルウェアは .NET コア、ASP.NET (OWIN OpenID Connect および OAuth)、Node.js (Microsoft ID プラットフォーム Passport.js) で利用できます。
- Microsoft ID プラットフォームには、多数のサード パーティ製認証ライブラリとの互換性があります。

Microsoft クライアント ライブラリ、Microsoft サーバー ミドルウェア、および互換性のあるサード パーティ製ライブラリの完全なリストについては、「[Microsoft ID プラットフォームの認証ライブラリ](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-libraries)」を参照してください。

認証ライブラリを使用してアクセス トークンを取得する必要はありません。 認証ライブラリを使わずに Microsoft ID プラットフォームのエンドポイントを直接使用する方法については、「[Microsoft ID プラットフォーム認証](https://docs.microsoft.com/ja-JP/azure/active-directory/develop/authentication-scenarios)」を参照してください。

## <a name="next-steps"></a>次の手順

- Microsoft Graph を読み出すアプリのアクセス トークンの簡単な取得手順については、自分のシナリオに合ったアプリの種類を選びます。
  - [デスクトップ アプリ](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-overview)
  - [モバイル アプリ](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-overview)
  - [Web アプリ](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-call-api-overview)
  - [シングル ページ アプリ](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-overview)
  - [デーモンまたはバックグラウンド サービス](https://docs.microsoft.com/azure/active-directory/develop/scenario-daemon-overview)
- Microsoft Graph で使用可能なアクセス許可を確認する場合は、「[アクセス許可](../permissions-reference.md)」を参照してください。
- Microsoft Graph によるパートナー管理型顧客データへのアクセスについて Microsoft クラウド ソリューション プロバイダーに興味がある場合は、「[アプリケーション アクセスの管理 (CSP)](../auth-cloudsolutionprovider.md)」を参照してください。

コードの作成準備が整ったら、次に示すリソースを使用できるようになります。これらのリソースは、Microsoft ID プラットフォームによる認証と承認をアプリに実装する際に役立ちます。

### <a name="microsoft-graph-training-and-samples"></a>Microsoft Graph のトレーニングとサンプル

すぐに使い始められるように、さまざまなプラットフォームで API を認証し使用する方法を示した、一連のトレーニング モジュールとその他のリソースを作成しました。

- [[概要](https://developer.microsoft.com/ja-JP/graph/get-started)] ページで、お好みのプラットフォーム向けのライブラリ、サンプル、トレーニング コンテンツなどのリソースを見つけてください。
- お使いのプラットフォーム向けに構成済みのサンプルをすぐに実行するには、「[Microsoft Graph のクイック スタート](https://developer.microsoft.com/ja-JP/graph/quick-start)」を参照してください。
- GitHub では [Microsoft Graph サンプル](https://github.com/microsoftgraph?utf8=%E2%9C%93&q=sample&type=&language=)を公開しています。

### <a name="microsoft-identity-platform-samples-and-documentation"></a>Microsoft ID プラットフォーム サンプルとドキュメント 

Microsoft ID プラットフォームのドキュメントには、特に Microsoft ID プラットフォームでの認証と承認に焦点を合わせた記事とサンプルが含まれています。

- 最も簡単な開始地点は、[Microsoft ID プラットフォームのエンドポイントのドキュメント](https://docs.microsoft.com/azure/active-directory/develop/active-directory-appmodel-v2-overview)です。 この記事には、概要、プロトコルに関するドキュメント、各種プラットフォームに対応している入門記事へのリンクが記載されています。このすべてのリンクは、開発しているアプリの種類ごとに編成されています。
- クライアントまたはサーバーの認証ライブラリごとのサンプル リストについては、「[Azure Microsoft ID プラットフォームの認証ライブラリ](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-libraries)」を参照してください。
- [Azure Code ギャラリー](https://azure.microsoft.com/resources/samples/?service=active-directory)のプラットフォームで Microsoft ID プラットフォーム サンプルをご覧ください。

## <a name="see-also"></a>関連項目

- [Microsoft ID プラットフォームのエンドポイントのドキュメント](https://docs.microsoft.com/azure/active-directory/develop/active-directory-appmodel-v2-overview)
