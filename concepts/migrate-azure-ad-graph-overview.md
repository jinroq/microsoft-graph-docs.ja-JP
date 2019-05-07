---
title: Azure AD Graph アプリを Microsoft Graph に移行する
description: Azure Active Directory (Azure AD) API アプリを Microsoft Graph API に移行する方法について説明します。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 348bc7632c2e2e158d41bb1cc2da9fa3ea755ca6
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33630231"
---
# <a name="migrate-azure-ad-graph-apps-to-microsoft-graph"></a><span data-ttu-id="b13d9-103">Azure AD Graph アプリを Microsoft Graph に移行する</span><span class="sxs-lookup"><span data-stu-id="b13d9-103">Migrate Azure AD Graph apps to Microsoft Graph</span></span>

<span data-ttu-id="b13d9-104">Microsoft Graph は Azure Active Directory (Azure AD) のグラフを完全に置き換えます。</span><span class="sxs-lookup"><span data-stu-id="b13d9-104">Microsoft Graph is fully replacing Azure Active Directory (Azure AD) Graph.</span></span> <span data-ttu-id="b13d9-105">ほとんどの運用アプリでは、Microsoft Graph は既に Azure AD シナリオを完全にサポートしています。</span><span class="sxs-lookup"><span data-stu-id="b13d9-105">For most production apps, Microsoft Graph can already fully support Azure AD scenarios.</span></span> <span data-ttu-id="b13d9-106">Azure AD Graph アプリを Microsoft Graph に移行し始める必要があります。</span><span class="sxs-lookup"><span data-stu-id="b13d9-106">You should start moving your Azure AD Graph apps to Microsoft Graph now.</span></span>

<span data-ttu-id="b13d9-107">さらに、Microsoft Graph では、Azure AD Graph では利用できない多くの新しい Azure AD データセットと機能をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="b13d9-107">In addition, Microsoft Graph supports many new Azure AD datasets and features that are not available in Azure AD Graph.</span></span> <span data-ttu-id="b13d9-108">Microsoft Graph に切り替えて、これらの新しい Api をすべて、次の単一のエンドポイントを介して利用できるようにします。</span><span class="sxs-lookup"><span data-stu-id="b13d9-108">Switch to Microsoft Graph to take advantage of these new APIs, all through one single endpoint, including:</span></span>

- [<span data-ttu-id="b13d9-109">Office 365 グループ管理</span><span class="sxs-lookup"><span data-stu-id="b13d9-109">Office 365 group management</span></span>](/graph/office365-groups-concept-overview)
- [<span data-ttu-id="b13d9-110">外部ユーザーの招待</span><span class="sxs-lookup"><span data-stu-id="b13d9-110">External user invitations</span></span>](/graph/api/resources/invitation?view=graph-rest-1.0)
- <span data-ttu-id="b13d9-111">削除した後、[ユーザーおよび Office 365 グループを復元](/graph/api/resources/directory?view=graph-rest-1.0)する機能</span><span class="sxs-lookup"><span data-stu-id="b13d9-111">The ability to [restore users and Office 365 groups](/graph/api/resources/directory?view=graph-rest-1.0) after they've been deleted</span></span>
- [<span data-ttu-id="b13d9-112">ユーザーとグループの Webhook 通知</span><span class="sxs-lookup"><span data-stu-id="b13d9-112">Webhook notifications on users and groups</span></span>](/graph/webhooks?toc=./ref/toc.json&view=graph-rest-1.0)
- <span data-ttu-id="b13d9-113">次のような Id ガバナンス機能</span><span class="sxs-lookup"><span data-stu-id="b13d9-113">Identity governance features such as:</span></span>
  - <span data-ttu-id="b13d9-114">[特権 id の管理](/graph/api/resources/privilegedidentitymanagement-root?view=graph-rest-beta)(PIM) ユーザーを必要なときにのみ特権の役割に昇格させ、期間を限定します。</span><span class="sxs-lookup"><span data-stu-id="b13d9-114">[Privileged identity management](/graph/api/resources/privilegedidentitymanagement-root?view=graph-rest-beta) (PIM) to elevate users to privileged roles only when needed and for a limited time period</span></span>
  - <span data-ttu-id="b13d9-115">ユーザーのアクセス権の構成証明のための1回限りまたは定期的なアクセスレビューのための[アクセスのレビュー](/graph/api/resources/accessreviews-root?view=graph-rest-beta)</span><span class="sxs-lookup"><span data-stu-id="b13d9-115">[Access reviews](/graph/api/resources/accessreviews-root?view=graph-rest-beta) for one-time or recurring access reviews for attestation of user's access rights</span></span>
  - <span data-ttu-id="b13d9-116">法律やコンプライアンスの要件に関する情報を提示することを可能にするための[使用条件](/graph/api/resources/accessreviews-root?view=graph-rest-beta)(免責事項など)</span><span class="sxs-lookup"><span data-stu-id="b13d9-116">[Terms-of-use](/graph/api/resources/accessreviews-root?view=graph-rest-beta) to enable organizations to present information for legal or compliance requirements, like disclaimer notices</span></span>
- <span data-ttu-id="b13d9-117">次のようなセキュリティ機能</span><span class="sxs-lookup"><span data-stu-id="b13d9-117">Security features such as:</span></span>
  - [<span data-ttu-id="b13d9-118">ID リスク イベント</span><span class="sxs-lookup"><span data-stu-id="b13d9-118">Identity risk events</span></span>](/graph/api/resources/identityriskevent?view=graph-rest-beta)
  - [<span data-ttu-id="b13d9-119">リスクの高いユーザー</span><span class="sxs-lookup"><span data-stu-id="b13d9-119">Risky users</span></span>](/graph/api/resources/riskyuser?view=graph-rest-beta)
- <span data-ttu-id="b13d9-120">[クライアントライブラリとサンプル](/graph/)は、多くのプラットフォームと言語で利用できます。</span><span class="sxs-lookup"><span data-stu-id="b13d9-120">[Client libraries and samples](/graph/) available on many more platforms and languages</span></span>

<span data-ttu-id="b13d9-121">Microsoft Graph では、Azure Active Directory だけでなく、多くのサービスにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="b13d9-121">Microsoft Graph offers access to many more services than just Azure Active Directory.</span></span> <span data-ttu-id="b13d9-122">[Microsoft 365 services の API ゲートウェイでも](/graph/)あります。</span><span class="sxs-lookup"><span data-stu-id="b13d9-122">It's the [API gateway to Microsoft 365 services too](/graph/).</span></span>

<span data-ttu-id="b13d9-123">このセクションの残りの記事では、アプリを Azure AD Graph から Microsoft Graph に移行する際に役立つ情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="b13d9-123">The rest of the articles in this section help you move your app from Azure AD Graph to Microsoft Graph.</span></span> <span data-ttu-id="b13d9-124">次のことがわかります。</span><span class="sxs-lookup"><span data-stu-id="b13d9-124">You'll find:</span></span>

- <span data-ttu-id="b13d9-125">計画に役立つチェックリスト。</span><span class="sxs-lookup"><span data-stu-id="b13d9-125">A checklist to help you plan.</span></span>
- <span data-ttu-id="b13d9-126">Api 間の特定の違いを説明するガイダンス。</span><span class="sxs-lookup"><span data-stu-id="b13d9-126">Guidance describing specific differences between the APIs.</span></span>
- <span data-ttu-id="b13d9-127">具体的な違いを説明するために、その他のリソースと例へのリンクがあります。</span><span class="sxs-lookup"><span data-stu-id="b13d9-127">Links to additional resources and examples to illustrate specific differences.</span></span>

## <a name="next-steps"></a><span data-ttu-id="b13d9-128">次のステップ</span><span class="sxs-lookup"><span data-stu-id="b13d9-128">Next Steps</span></span>

- <span data-ttu-id="b13d9-129">移行を計画する際に役立つ、[アプリの移行チェックリスト](migrate-azure-ad-graph-planning-checklist.md)について説明します。</span><span class="sxs-lookup"><span data-stu-id="b13d9-129">Walk through the [app migration checklist](migrate-azure-ad-graph-planning-checklist.md) to help you plan the move.</span></span>
- <span data-ttu-id="b13d9-130">[Microsoft Graph](/graph/overview)の概念とプラクティスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="b13d9-130">Explore [Microsoft Graph](/graph/overview) concepts and practices.</span></span>
- <span data-ttu-id="b13d9-131">[Graph エクスプローラー](https://aka.ms/ge)を使用して、Microsoft graph を試してみてください。</span><span class="sxs-lookup"><span data-stu-id="b13d9-131">Use [Graph Explorer](https://aka.ms/ge) to experiment with Microsoft Graph.</span></span>
- <span data-ttu-id="b13d9-132">進捗状況の更新とタイムラインの詳細については、「 [Microsoft Graph」または「AZURE AD Graph](https://dev.office.com/blogs/microsoft-graph-or-azure-ad-graph) In The Office デベロッパーセンター」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b13d9-132">To learn more about progress updates and timelines, see [Microsoft Graph or the Azure AD Graph](https://dev.office.com/blogs/microsoft-graph-or-azure-ad-graph) in the Office Dev Center.</span></span>
