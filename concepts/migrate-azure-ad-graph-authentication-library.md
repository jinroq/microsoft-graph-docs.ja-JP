---
title: アプリ認証ライブラリの変更を確認する
description: Azure Active Directory (Azure AD) API アプリから Microsoft Graph API にアプリを移行するために、認証ライブラリの使用を更新する方法について説明します。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 77604945064565f1387553b22a26a0fa871c998d
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33630266"
---
# <a name="review-app-authentication-library-changes"></a><span data-ttu-id="b1078-103">アプリ認証ライブラリの変更を確認する</span><span class="sxs-lookup"><span data-stu-id="b1078-103">Review app authentication library changes</span></span>

<span data-ttu-id="b1078-104">この記事は、「*手順 3:* アプリ[を移行するプロセス](migrate-azure-ad-graph-planning-checklist.md)の詳細を確認する」に含まれています。</span><span class="sxs-lookup"><span data-stu-id="b1078-104">This article is part of *step 3: review app details* of the [process to migrate apps](migrate-azure-ad-graph-planning-checklist.md).</span></span>

<span data-ttu-id="b1078-105">ほとんどのアプリは、認証ライブラリを使用して、Microsoft Graph を呼び出すためのアクセストークンを要求して管理します。</span><span class="sxs-lookup"><span data-stu-id="b1078-105">Most apps use an authentication library to aquire and manage access tokens to call Microsoft Graph.</span></span>  <span data-ttu-id="b1078-106">Microsoft では、2つの認証ライブラリを提供しています。</span><span class="sxs-lookup"><span data-stu-id="b1078-106">Microsoft offers two authentication libraries:</span></span>

- <span data-ttu-id="b1078-107">[Azure Active Directory 認証ライブラリ](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-libraries)ADAL</span><span class="sxs-lookup"><span data-stu-id="b1078-107">[Azure Active Directory authentication library](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-libraries) (ADAL)</span></span>
- <span data-ttu-id="b1078-108">[Microsoft 認証ライブラリ](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries)MSAL</span><span class="sxs-lookup"><span data-stu-id="b1078-108">[Microsoft authentication library](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) (MSAL)</span></span>

## <a name="updating-adal"></a><span data-ttu-id="b1078-109">ADAL の更新</span><span class="sxs-lookup"><span data-stu-id="b1078-109">Updating ADAL</span></span>

<span data-ttu-id="b1078-110">アプリで現在 ADAL を使用している場合は、2段階の移行アプローチを使用します。</span><span class="sxs-lookup"><span data-stu-id="b1078-110">If your app currently uses ADAL, use a two-stage migration approach:</span></span>

1. <span data-ttu-id="b1078-111">アプリを更新して、Microsoft Graph のアクセストークンを取得します。</span><span class="sxs-lookup"><span data-stu-id="b1078-111">Update your app to acquire access tokens for Microsoft Graph.</span></span> <span data-ttu-id="b1078-112">この手順では、引き続き ADAL を使用します。</span><span class="sxs-lookup"><span data-stu-id="b1078-112">Continue to use ADAL for this step.</span></span> <span data-ttu-id="b1078-113">リソース web API を表す URI を保持する**Resourceurl**を次のように更新します。</span><span class="sxs-lookup"><span data-stu-id="b1078-113">Update the **resourceURL**, which holds the URI representing the resource web API, from:</span></span>

    `https://graph.windows.net`  

    <span data-ttu-id="b1078-114">宛先：</span><span class="sxs-lookup"><span data-stu-id="b1078-114">To:</span></span>  

    `https://graph.microsoft.com`

    <span data-ttu-id="b1078-115">この変更後、新しく取得したトークンのスコープは同じですが、アクセストークンの対象ユーザーは Microsoft Graph になりました。</span><span class="sxs-lookup"><span data-stu-id="b1078-115">Newly acquired tokens have the same scopes after this change, but the audience of the access tokens is now Microsoft Graph.</span></span>  

    <span data-ttu-id="b1078-116">**Resourceurl**および検証された機能を更新したら、暫定的な更新をリリースしてユーザーを runnning します。</span><span class="sxs-lookup"><span data-stu-id="b1078-116">Once you've updated **resourceURL** and verified functionality, release an interim update to get your users up and runnning.</span></span>

1.  <span data-ttu-id="b1078-117">次に、MSAL を使用するようにアプリを移行する作業を開始します。これは、移動を使用するためにサポートされているライブラリです。</span><span class="sxs-lookup"><span data-stu-id="b1078-117">Next, begin work migrating your app to use MSAL, which is the supported library to use moving forward.</span></span>

## <a name="migrating-to-msal"></a><span data-ttu-id="b1078-118">MSAL への移行</span><span class="sxs-lookup"><span data-stu-id="b1078-118">Migrating to MSAL</span></span>

<span data-ttu-id="b1078-119">MSAL は、追加の同意、豊富なシングルサインオンエクスペリエンス、個人の Microsoft アカウントのサポート、標準ベースのプロトコルの使用などを含む、ADAL に対して複数の利点を提供します。</span><span class="sxs-lookup"><span data-stu-id="b1078-119">MSAL provides multiple benefits over ADAL, including incremental consent, richer single sign-on experiences, support for personal Microsoft accounts, use of standards-based protocols and so on.</span></span>  

<span data-ttu-id="b1078-120">アプリを MSAL に切り替えるときには、次のようにいくつかの変更を行う必要があります。これには、トークン acquistion 要求の**範囲**パラメーターの設定などが含まれます。</span><span class="sxs-lookup"><span data-stu-id="b1078-120">When you switch your app over to MSAL, you'll need to make a few changes, including setting the **scopes** parameter in the token acquistion request:</span></span>

``` csharp
var scopes = new string[] { "https://graph.microsoft.com/.default" };
```

<span data-ttu-id="b1078-121">上記の式では、アクセス許可スコープ要求が、Azure Portal のアプリケーション登録時に構成されたものに制限され、既存のユーザーがアプリに再び同意する必要がなくなります。</span><span class="sxs-lookup"><span data-stu-id="b1078-121">The expression above limits the permission scopes request to those configured during application registration in the Azure Portal, and saves your existing users from having to consent to your app again.</span></span>

<span data-ttu-id="b1078-122">一般的なエラーに関するトラブルシューティングやヘルプを含む、プロセスに関する直接の広範なヘルプについては、「 [ADAL を MSAL に移行する](https://aka.ms/adal-net-to-msal-net)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b1078-122">See [Migrating ADAL to MSAL](https://aka.ms/adal-net-to-msal-net) for direct and extensive help with the process, including troubleshooting and help with common errors.</span></span>

<span data-ttu-id="b1078-123">MSAL に移行した後は、追加のスコープを動的に要求することができます。ユーザーは、次回アプリを使用するときに、増分の同意を提供するように求められます。</span><span class="sxs-lookup"><span data-stu-id="b1078-123">Once you've migrated to MSAL, you can request additional scopes dynamically, and users are prompted to provide incremental consent the next time they use your app.</span></span>

## <a name="next-steps"></a><span data-ttu-id="b1078-124">次のステップ</span><span class="sxs-lookup"><span data-stu-id="b1078-124">Next Steps</span></span>

- <span data-ttu-id="b1078-125">Azure AD Graph と Microsoft Graph の間の[.net クライアントライブラリ](migrate-azure-ad-graph-client-libraries.md)の違いについて説明します。</span><span class="sxs-lookup"><span data-stu-id="b1078-125">Learn [.NET client library](migrate-azure-ad-graph-client-libraries.md) differences between Azure AD Graph and Microsoft Graph.</span></span>
- <span data-ttu-id="b1078-126">MSAL への移行に関する詳細なヘルプについては、「 [ADAL を MSAL に移行する](https://aka.ms/adal-net-to-msal-net)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b1078-126">Explore [Migrating ADAL to MSAL](https://aka.ms/adal-net-to-msal-net) for more in-depth help on migrating to MSAL.</span></span>
- <span data-ttu-id="b1078-127">[Microsoft Graph](/graph/overview)の概念とプラクティスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="b1078-127">Explore [Microsoft Graph](/graph/overview) concepts and practices.</span></span>
- <span data-ttu-id="b1078-128">[Graph エクスプローラー](https://aka.ms/ge)を使用して、Microsoft graph を試してみてください。</span><span class="sxs-lookup"><span data-stu-id="b1078-128">Use [Graph Explorer](https://aka.ms/ge) to experiment with Microsoft Graph.</span></span>
