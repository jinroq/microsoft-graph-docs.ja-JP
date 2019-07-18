---
title: Microsoft Graph 通知のためのアプリの登録と API アクセス許可を管理する
description: Microsoft Graph 経由で送信される通知を受信するためには、最初に、Microsoft Azure portal でアプリケーションを登録する必要があります。
localization_priority: Priority
ms.prod: notifications
ms.openlocfilehash: dc102f451b3f206bbfefe1d3c38c3995041f04fa
ms.sourcegitcommit: 9cee9d8229fc84dd7ef97670ff27c145e1a78408
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/18/2019
ms.locfileid: "35778636"
---
# <a name="manage-app-registration-and-api-permission-for-microsoft-graph-notifications"></a><span data-ttu-id="4f5ad-103">Microsoft Graph 通知のためのアプリの登録と API アクセス許可を管理する</span><span class="sxs-lookup"><span data-stu-id="4f5ad-103">Manage app registration and API permission for Microsoft Graph notifications</span></span>

<span data-ttu-id="4f5ad-104">Microsoft Graph 通知と統合するアプリケーション サービスのためには、Microsoft アカウントあるいは職場や学校のアカウントをサポートする Microsoft ID プラットフォームでアプリを登録する必要があり、必要な API アクセス許可を宣言する必要があります。</span><span class="sxs-lookup"><span data-stu-id="4f5ad-104">In order for your application service to integrate with Microsoft Graph notifications, you need to register your app with the Microsoft identity platform to support Microsoft accounts or work or school accounts, and declare the API permissions that are required.</span></span>

## <a name="register-your-app-to-support-microsoft-accounts-or-work-or-school-accounts"></a><span data-ttu-id="4f5ad-105">Microsoft アカウントあるいは職場や学校のアカウントをサポートするアプリを登録します。</span><span class="sxs-lookup"><span data-stu-id="4f5ad-105">Register your app to support Microsoft accounts or work or school accounts</span></span>

<span data-ttu-id="4f5ad-106">[Microsoft Azure portal](https://portal.azure.com/#home) で、Microsoft アカウントあるいは職場や学校のアカウントをサポートするアプリを登録します。</span><span class="sxs-lookup"><span data-stu-id="4f5ad-106">Register your application on the [Microsoft Azure portal](https://portal.azure.com/#home) to support Microsoft accounts or work or school accounts.</span></span> <span data-ttu-id="4f5ad-107">[Microsoft アプリケーション ポータル](https://apps.dev.microsoft.com/)で、以前アプリケーションを登録したことがある場合、新機能と改善された機能の Azure portal エクスペリエンスに既存のアプリが表示されます。</span><span class="sxs-lookup"><span data-stu-id="4f5ad-107">If you’ve previously registered your application on the [Microsoft Application Portal](https://apps.dev.microsoft.com/), your existing apps will show up in the new and improved Azure portal experience.</span></span>

<span data-ttu-id="4f5ad-108">アプリの登録の方法については、[Microsoft ID プラットフォームへのアプリケーションの登録](auth-register-app-v2.md)に関するページを参照してください。</span><span class="sxs-lookup"><span data-stu-id="4f5ad-108">For information about how to register your apps, see [Register an application with the Microsoft identity platform](auth-register-app-v2.md).</span></span> 


> [!NOTE]
> <span data-ttu-id="4f5ad-109">Microsoft アカウントを持っていないが使用したい場合には、 [Microsoft アカウント](https://account.microsoft.com/account) ページを参照してください。</span><span class="sxs-lookup"><span data-stu-id="4f5ad-109">If you don't already have a Microsoft account and would like to use one, go to the [Microsoft account](https://account.microsoft.com/account) page.</span></span> <span data-ttu-id="4f5ad-110">職場または学校のアカウントで、認証と ID フレームワークとして Azure AD v1.0 使用する必要があるアプリを作成する場合は、 [Azure Active Directory 認証ライブラリ](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-libraries)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4f5ad-110">If you're writing an app that needs to use Azure AD v1.0 as an authentication and identity framework for work or school accounts, see [Azure Active Directory Authentication Libraries](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-libraries).</span></span> <span data-ttu-id="4f5ad-111">新しく収束された Microsoft ID プラットフォーム (バージョン 2.0) について学んだり利用に関心がある場合は、 [Microsoft アイデンティティ プラットフォームのエンドポイントと Azure AD v1.0 エンドポイントを比較する](https://docs.microsoft.com/ja-JP/azure/active-directory/develop/azure-ad-endpoint-comparison)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4f5ad-111">If you’re interested in learning about or using the new converged Microsoft identity platform (v2.0), see [Comparing the Microsoft identity platform endpoint and Azure AD v1.0 endpoint](https://docs.microsoft.com/en-us/azure/active-directory/develop/azure-ad-endpoint-comparison).</span></span>

<span data-ttu-id="4f5ad-112">アプリを登録すると、アプリケーション ID/ クライアント ID がいろいろと便利になります。</span><span class="sxs-lookup"><span data-stu-id="4f5ad-112">When you register your app, keep the application ID/client ID somewhere handy.</span></span> <span data-ttu-id="4f5ad-113">[Microsoft パートナー センター](https://partner.microsoft.com/)でさまざまなデバイスの操作でのアプリケーションを登録するときに、この ID が後で必要になります。 </span><span class="sxs-lookup"><span data-stu-id="4f5ad-113">You'll need this ID later when you register your application for cross-device experiences in the [Microsoft Partner Center](https://partner.microsoft.com/).</span></span>

## <a name="app-certificates-and-secrets"></a><span data-ttu-id="4f5ad-114">アプリ証明書とシークレット</span><span class="sxs-lookup"><span data-stu-id="4f5ad-114">App certificates and secrets</span></span>

<span data-ttu-id="4f5ad-115">アプリケーションを識別し、認証トークンを取得するときに認証を有効にするには、独自の証明書をアップロードしたり、Azure portal の**証明書とシークレット**に移動して新しいクライアント シークレットを作成することもできます。</span><span class="sxs-lookup"><span data-stu-id="4f5ad-115">To enable your application to identify and authenticate itself when obtaining auth tokens, you can either upload your own certificate or create a new client secret by going to **Certificates & secrets** in the Azure portal.</span></span>
    
![Azure portal 内のアプリ証明書とシークレットのスクリーン ショット](images/notifications-app-secrets.png)
    
> [!NOTE]
> <span data-ttu-id="4f5ad-117">新しいクライアント シークレットの生成を選択する場合は、必ずをコピーして、安全な場所に保管してください。</span><span class="sxs-lookup"><span data-stu-id="4f5ad-117">If you opt to generate a new client secret, be sure to copy and keep it in a safe place.</span></span> <span data-ttu-id="4f5ad-118">ポータルから脱退したら、もう一度アクセスすることはできません。</span><span class="sxs-lookup"><span data-stu-id="4f5ad-118">You won’t be able to access it again after you leave the portal.</span></span>

## <a name="api-permissions"></a><span data-ttu-id="4f5ad-119">API アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4f5ad-119">Configure API permissions</span></span>

<span data-ttu-id="4f5ad-120">Microsoft Graph の通知を使用するために追加の許可を追加する必要があります。</span><span class="sxs-lookup"><span data-stu-id="4f5ad-120">You'll need to add additional permissions in order to use Microsoft Graph notifications.</span></span> <span data-ttu-id="4f5ad-121">[**アクセス許可を追加**]を選択し、Microsoft Api で [**Microsoft Graph**]を選択してから、[**アクセス許可を委任**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="4f5ad-121">Choose **Add a permission**, and under Microsoft APIs, select **Microsoft Graph**, and then select **Delegated permissions**.</span></span>
    
![Azure portal の API アクセス許可の要求ページのスクリーンショット](images/notifications-api-permissions.png)
    
<span data-ttu-id="4f5ad-123">以下のアクセス許可を追加します。</span><span class="sxs-lookup"><span data-stu-id="4f5ad-123">Add the following permissions:</span></span>

- <span data-ttu-id="4f5ad-124">User.Read - ユーザーにサインインするアプリケーションを許可する</span><span class="sxs-lookup"><span data-stu-id="4f5ad-124">User.Read - allows your application to sign-in your user</span></span>

- <span data-ttu-id="4f5ad-125">Device.Read - デバイスのユーザーの一覧の ID を許可する</span><span class="sxs-lookup"><span data-stu-id="4f5ad-125">Device.Read - allows identification of a user’s list of devices</span></span>

- <span data-ttu-id="4f5ad-126">Device.Command - ユーザーのデバイスとの通信を許可する</span><span class="sxs-lookup"><span data-stu-id="4f5ad-126">Device.Command - allows communication to a user’s device</span></span>

- <span data-ttu-id="4f5ad-127">UserActivity.ReadWrite.CreatedByApp - 通知を取得するためのアプリのサブスクリプションを許可する</span><span class="sxs-lookup"><span data-stu-id="4f5ad-127">UserActivity.ReadWrite.CreatedByApp - allows app subscription for notification retrieval</span></span>

- <span data-ttu-id="4f5ad-128">Notifications.ReadWrite.CreatedByApp - アクセスと配信の通知を許可する</span><span class="sxs-lookup"><span data-stu-id="4f5ad-128">Notifications.ReadWrite.CreatedByApp - allows notification access and delivery</span></span>

- <span data-ttu-id="4f5ad-129">wns.connect - windows の通知サービスへの接続を許可する</span><span class="sxs-lookup"><span data-stu-id="4f5ad-129">wns.connect - allows connecting to windows notification service</span></span>

![Azure portal で通知を行うのための代理アクセス権を示すスクリーン ショット](images/notifications-api-permissions-list.png)

## <a name="next-steps"></a><span data-ttu-id="4f5ad-131">次の手順</span><span class="sxs-lookup"><span data-stu-id="4f5ad-131">Next steps</span></span>

<span data-ttu-id="4f5ad-132">
  [アクセス許可と同意](https://docs.microsoft.com/ja-JP/azure/active-directory/develop/v2-permissions-and-consent)に関する詳細を確認する、または「Microsoft Graph [アクセス許可のリファレンス](https://docs.microsoft.com/ja-JP/graph/permissions-reference)」を参照します。</span><span class="sxs-lookup"><span data-stu-id="4f5ad-132">Learn more about [permissions and consent](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-permissions-and-consent) or view the Microsoft Graph [permissions reference](https://docs.microsoft.com/en-us/graph/permissions-reference).</span></span>

<span data-ttu-id="4f5ad-133">これで、アプリの登録が完了しました。デバイス間の操作性のためのアプリケーションをセットアップし、Microsoft Graph 経由で送信される通知を行うためと、対応するアプリ プラットフォームを対象にするために[パートナー センター](https://partner.microsoft.com/)に移動します。</span><span class="sxs-lookup"><span data-stu-id="4f5ad-133">Now that you’ve registered your app, go to the [Partner Center](https://partner.microsoft.com/) to set up your application for cross-device experiences and to target your corresponding app platforms for notifications sent via Microsoft Graph.</span></span> <span data-ttu-id="4f5ad-134">詳細については、[クロスデバイス エクスペリエンスに参加する](notifications-integration-cross-device-experiences-onboarding.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4f5ad-134">For details, see [Onboarding to cross-device experiences](notifications-integration-cross-device-experiences-onboarding.md).</span></span> 
