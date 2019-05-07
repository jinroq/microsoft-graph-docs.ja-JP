---
title: アプリの登録、アクセス許可、および同意移行の問題を確認する
description: Azure Active Directory (Azure AD) から Microsoft Graph API へのアプリの登録、アクセス許可、および同意の移行について説明します。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 54e187fcf35f030413aa98a6cb0e34649532a8b4
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33630280"
---
# <a name="review-app-registration-permissions-and-consent"></a><span data-ttu-id="6f85d-103">アプリの登録、アクセス許可、同意を確認する</span><span class="sxs-lookup"><span data-stu-id="6f85d-103">Review app registration, permissions, and consent</span></span>

<span data-ttu-id="6f85d-104">この記事は、「*手順 3:* アプリ[を移行するプロセス](migrate-azure-ad-graph-planning-checklist.md)の詳細を確認する」に含まれています。</span><span class="sxs-lookup"><span data-stu-id="6f85d-104">This article is part of *step 3: review app details* of the [process to migrate apps](migrate-azure-ad-graph-planning-checklist.md).</span></span>

<span data-ttu-id="6f85d-105">アプリの更新プログラムには、次の3つの点を考慮する必要があります。</span><span class="sxs-lookup"><span data-stu-id="6f85d-105">For any app update, there are three areas to consider:</span></span>

- <span data-ttu-id="6f85d-106">**アプリの登録**: アプリケーションコードで既存のアプリの登録 (`appId`) を引き続き使用できます。</span><span class="sxs-lookup"><span data-stu-id="6f85d-106">**App registration**: You can continue to use your existing app registration (`appId`) in your application code.</span></span>  

    <span data-ttu-id="6f85d-107">Microsoft Graph に移行するために、アプリを再登録する必要はあり**ません**。</span><span class="sxs-lookup"><span data-stu-id="6f85d-107">You do **not** have to re-register your app to migrate to Microsoft Graph.</span></span> <span data-ttu-id="6f85d-108">コードを更新し、頻繁にテストして、更新プログラムを展開するだけです。</span><span class="sxs-lookup"><span data-stu-id="6f85d-108">Simply update the code, test heavily, and then deploy your update.</span></span>  

- <span data-ttu-id="6f85d-109">**アクセス許可**: アプリに対して構成済みの既存のアクセス許可を引き続き使用できます。</span><span class="sxs-lookup"><span data-stu-id="6f85d-109">**Permissions**: You can continue to use the existing configured permissions for your app.</span></span> <span data-ttu-id="6f85d-110">Azure AD Graph のアクセス許可は Microsoft Graph と共有されるため、新しいアクセス許可を要求する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="6f85d-110">You do not have to request new permissions because Azure AD Graph permissions are shared with Microsoft Graph.</span></span>

    <span data-ttu-id="6f85d-111">たとえば、既存のアプリに_ユーザー_が設定されている場合__ 、そのアクセス許可は、更新された Microsoft Graph のアプリに対して暗黙的に付与されます。</span><span class="sxs-lookup"><span data-stu-id="6f85d-111">For example, if your existing app has _User.Read.All_ and _Group.Read.All_ permissions, those permissions are implicitly granted to your updated app for Microsoft Graph as well.</span></span>

    <span data-ttu-id="6f85d-112">更新プログラムで、Azure AD Graph で利用できない機能の使用が必要になった場合は、これらの新機能に対するアクセス許可を要求する必要があります。</span><span class="sxs-lookup"><span data-stu-id="6f85d-112">If your update also incudes the use of features or capabilities that aren't available to Azure AD Graph, you'll likely need to request permissions for these new features.</span></span> <span data-ttu-id="6f85d-113">その場合は、MSAL と v2 のエンドポイントを使用するようにアプリを切り替え、追加/増分の同意を動的に要求することができます。</span><span class="sxs-lookup"><span data-stu-id="6f85d-113">If that's the case, you can switch your app to use MSAL and the v2 endpoint, and request additional/incremental consent dynamically.</span></span> <span data-ttu-id="6f85d-114">「[アプリ認証ライブラリの変更を確認](/graph/migrate-azure-ad-graph-authentication-library)する」の「msal への切り替えの詳細」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6f85d-114">Find more details about switching to MSAL in [review app authentication library changes](/graph/migrate-azure-ad-graph-authentication-library).</span></span>

- <span data-ttu-id="6f85d-115">**同意**: エンドユーザーは、同意を再度付与するメッセージが表示されることなく、アプリを引き続き使用できます。</span><span class="sxs-lookup"><span data-stu-id="6f85d-115">**Consent**: End-users can continue using your app without being asked to grant consent again.</span></span>

    <span data-ttu-id="6f85d-116">自分のデータにアクセスするためにアプリに同意を付与しているユーザーは、再度同意を求められることなく、Microsoft Graph を使用するように更新された後もアプリを使用し続けることができます。</span><span class="sxs-lookup"><span data-stu-id="6f85d-116">Users who have already granted consent to your app to access their data can continue to use your app after it's been updated to use Microsoft Graph, without being asked to consent again.</span></span>

<span data-ttu-id="6f85d-117">シンプルな移行プロジェクトでは、これらの領域で問題は発生しません。</span><span class="sxs-lookup"><span data-stu-id="6f85d-117">Simple migration projects should experience no issues in these areas.</span></span>

<span data-ttu-id="6f85d-118">ただし、新しい機能、サービス、またはその他の機能を使用する場合は、新しいアクセス許可とエンドユーザーの同意が必要になることがあります。</span><span class="sxs-lookup"><span data-stu-id="6f85d-118">However, if you use new features, services, or add additional capabilities, you may need new permissions and end-user consent may be required.</span></span>  <span data-ttu-id="6f85d-119">このような場合は、トークンの更新時に同意が要求されます。</span><span class="sxs-lookup"><span data-stu-id="6f85d-119">In such cases, consent is requested when tokens are refreshed.</span></span>

## <a name="next-steps"></a><span data-ttu-id="6f85d-120">次のステップ</span><span class="sxs-lookup"><span data-stu-id="6f85d-120">Next Steps</span></span>

- <span data-ttu-id="6f85d-121">Azure AD Graph と Microsoft Graph の[認証ライブラリ](migrate-azure-ad-graph-authentication-library.md)の違いについて説明します。</span><span class="sxs-lookup"><span data-stu-id="6f85d-121">Learn [authentication library](migrate-azure-ad-graph-authentication-library.md) differences between Azure AD Graph and Microsoft Graph.</span></span>
- <span data-ttu-id="6f85d-122">[Microsoft Graph](/graph/overview)の概念とプラクティスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="6f85d-122">Explore [Microsoft Graph](/graph/overview) concepts and practices.</span></span>
- <span data-ttu-id="6f85d-123">[Graph エクスプローラー](https://aka.ms/ge)を使用して、Microsoft graph を試してみてください。</span><span class="sxs-lookup"><span data-stu-id="6f85d-123">Use [Graph Explorer](https://aka.ms/ge) to experiment with Microsoft Graph.</span></span>
