---
title: REST API を使用して Exchange ハイブリッド展開のメールボックスにアクセスする (プレビュー)
description: Office 365 の一部として、Microsoft Graph は、Exchange Online のクラウドにある顧客メールボックスへのアクセスを常に提供してきました。
localization_priority: Priority
ms.openlocfilehash: 5dab9fea5a9d9c9177befc90ccb64b3bb03b6b33
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864352"
---
# <a name="use-rest-apis-to-access-mailboxes-in-exchange-hybrid-deployments-preview"></a><span data-ttu-id="6a4cf-103">REST API を使用して Exchange ハイブリッド展開のメールボックスにアクセスする (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="6a4cf-103">Use REST APIs to access mailboxes in Exchange hybrid deployments (preview)</span></span>

<span data-ttu-id="6a4cf-104">Microsoft Graph では、Office 365 の一部としての Exchange Online で、クラウドにある顧客メールボックスへのアクセスをずっと提供してきました。</span><span class="sxs-lookup"><span data-stu-id="6a4cf-104">Microsoft Graph has always provided access to customer mailboxes in the cloud on Exchange Online as part of Office 365.</span></span>
<span data-ttu-id="6a4cf-105">2016 年 9 月にリリースされた Exchange On-Premises サーバー用の Exchange 2016 Cumulative Update 3 (CU3) では、Office 365 との REST API の統合のサポートが追加されています。</span><span class="sxs-lookup"><span data-stu-id="6a4cf-105">Exchange 2016 Cumulative Update 3 (CU3), released in September 2016 for Exchange on-premises servers, adds support for REST API integration with Office 365.</span></span> <span data-ttu-id="6a4cf-106">アプリで v1.0 の[メール](/graph/api/resources/message?view=graph-rest-1.0)、[カレンダー](/graph/api/resources/calendar?view=graph-rest-1.0)、[連絡先](/graph/api/resources/contact?view=graph-rest-1.0) API を使用している場合、_ハイブリッド_展開で認証やアプリケーションのエクスペリエンスがシームレスとなり、展開が特定の[要件](#requirements-for-the-rest-api-to-work-in-hybrid-deployments)を満たしていれば、メールボックスがオンプレミスとクラウドのどちらにあろうと関係なくなりました。</span><span class="sxs-lookup"><span data-stu-id="6a4cf-106">If your app uses v1.0 of the [Mail](/graph/api/resources/message?view=graph-rest-1.0), [Calendar](/graph/api/resources/calendar?view=graph-rest-1.0), or [Contacts](/graph/api/resources/contact?view=graph-rest-1.0) API, you will now also find a seamless authentication and application experience in _hybrid_ deployments, regardless of whether the mailbox is on-premises or in the cloud, provided that the deployment meets specific [requirements](#requirements-for-the-rest-api-to-work-in-hybrid-deployments).</span></span> 


<span data-ttu-id="6a4cf-p102">舞台裏では、ハイブリッド展開のオンプレミスのメールボックスに REST API 呼び出しがアクセスしようとしていることを Microsoft Graph が識別すると、Microsoft Graph は REST 要求をオンプレミスの REST エンドポイントに送り、エンドポイントがその要求を処理します。この検出により、REST API へのアクセスが可能になります。</span><span class="sxs-lookup"><span data-stu-id="6a4cf-p102">Behind the scenes, when Microsoft Graph identifies that a REST API call is attempting to access an on-premises mailbox in a hybrid deployment, it proxies the REST request to an on-premises REST endpoint which then processes the request. This discovery makes accessing the REST API possible.</span></span>

><span data-ttu-id="6a4cf-109">**注:** ハイブリッド展開でこれらの REST API を使用する機能は、現在プレビュー段階です。</span><span class="sxs-lookup"><span data-stu-id="6a4cf-109">**Note:** The ability to use these REST APIs in hybrid deployments is currently in preview.</span></span>

><span data-ttu-id="6a4cf-p103">ハイブリッド展開のメールボックスでは、v1.0 のメール、予定表、連絡先 API のみを使用できます。[グループ](/graph/api/resources/group?view=graph-rest-1.0) API など、他の v1.0 API セットや、他のバージョンの API は使用できません。ハイブリッド展開でサポートされているセットに属さない API を使用しようとすると、次のエラー メッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="6a4cf-p103">Only v1.0 of the Mail, Calendar and Contacts API are available for mailboxes in hybrid deployments. Other v1.0 API sets, such as the [Groups](/graph/api/resources/group?view=graph-rest-1.0) API, or APIs in other versions, are not. If you attempt to use an API that is not part of the supported set in a hybrid deployment, you will get the following error message:</span></span>

><span data-ttu-id="6a4cf-113">"このメールボックスの REST API は現在プレビュー段階です。</span><span class="sxs-lookup"><span data-stu-id="6a4cf-113">"REST APIs for this mailbox are currently in preview.</span></span> <span data-ttu-id="6a4cf-114">REST API (プレビュー) の詳細については、https://dev.outlook.com をご覧ください。"</span><span class="sxs-lookup"><span data-stu-id="6a4cf-114">You can find more information about the preview REST APIs at https://dev.outlook.com."</span></span>

## <a name="requirements-for-the-rest-api-to-work-in-hybrid-deployments"></a><span data-ttu-id="6a4cf-115">ハイブリッド展開で REST API が作動する要件</span><span class="sxs-lookup"><span data-stu-id="6a4cf-115">Requirements for the REST API to work in hybrid deployments</span></span>

<span data-ttu-id="6a4cf-116">Microsoft Graph はオープンネス (JSON、OAUTH、ODATA といったオープンな標準をサポートし、最も人気のあるプラットフォームから接続可能)、および柔軟性 (ユーザー データにアクセスするための段階的で、厳格に範囲指定されたアクセス許可) を提供します。</span><span class="sxs-lookup"><span data-stu-id="6a4cf-116">Microsoft Graph provides openness (open standards support like JSON, OAUTH and ODATA, connecting from most popular platforms) and flexibility (granular, tightly scoped permissions to access user data).</span></span> <span data-ttu-id="6a4cf-117">組織が Microsoft Graph アプリ開発の有効化に興味があり、現在、ハイブリッド展開を実装している、または実装を検討している場合、次の展開要件に注意してください。</span><span class="sxs-lookup"><span data-stu-id="6a4cf-117">If your organization is interested in enabling Microsoft Graph app development and is currently in or considering a hybrid deployment, be aware of the following deployment requirements:</span></span>

- <span data-ttu-id="6a4cf-118">メールボックスの要件</span><span class="sxs-lookup"><span data-stu-id="6a4cf-118">Mailbox requirements</span></span>

  - <span data-ttu-id="6a4cf-119">REST API を使用するオンプレミスのメールボックスはすべて Exchange 2016 CU3 サーバー上のデータベースに配置される必要があります。</span><span class="sxs-lookup"><span data-stu-id="6a4cf-119">All on-premises mailboxes that will use the REST APIs must be located on databases located on Exchange 2016 CU3 servers.</span></span> 

- <span data-ttu-id="6a4cf-120">インフラストラクチャの要件</span><span class="sxs-lookup"><span data-stu-id="6a4cf-120">Infrastructure requirements</span></span>

  - <span data-ttu-id="6a4cf-121">すべての Exchange 2016 サーバーを CU3 以降にアップグレードする必要があります。</span><span class="sxs-lookup"><span data-stu-id="6a4cf-121">All Exchange 2016 servers must be upgraded to CU3 or later.</span></span>  
  - <span data-ttu-id="6a4cf-122">オンプレミスの Active Directory を Azure Active Directory と同期させる必要があります。</span><span class="sxs-lookup"><span data-stu-id="6a4cf-122">On-premises Active Directory must synchronize with Azure Active Directory.</span></span>
  - <span data-ttu-id="6a4cf-123">Exchange 2016 サーバーと同じ負荷分散アレイにおいて共存するすべての Exchange 2013 サーバーを、アレイから削除する必要があります。</span><span class="sxs-lookup"><span data-stu-id="6a4cf-123">Any Exchange 2013 servers coexisting in the same load-balanced array with Exchange 2016 servers must be removed from the array.</span></span>

- <span data-ttu-id="6a4cf-124">ネットワークの要件</span><span class="sxs-lookup"><span data-stu-id="6a4cf-124">Networking requirements</span></span>

  - <span data-ttu-id="6a4cf-125">DNS の観点から、自動検出の名前空間およびオンプレミスのクライアント名前空間には、インターネットの DNS レコードが含まれている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6a4cf-125">From a DNS perspective, the Autodiscover namespace and on-premises client namespace must have Internet DNS records.</span></span> 
  - <span data-ttu-id="6a4cf-126">アクセスを検査および制限するファイアウォールまたはアプリケーション ゲートウェイがある場合は、適切な設定を更新して、検出およびアクセスを許可します。</span><span class="sxs-lookup"><span data-stu-id="6a4cf-126">If you have a firewall or application gateway that inspects and restricts access, update the appropriate settings to allow discovery and access.</span></span>


<span data-ttu-id="6a4cf-127">IT 管理者は、次のリソースで詳細情報を確認できます。</span><span class="sxs-lookup"><span data-stu-id="6a4cf-127">IT administrators can find more information in the following resources:</span></span>

- <span data-ttu-id="6a4cf-128">
  [Exchange Server のハイブリッド展開](https://technet.microsoft.com/en-us/library/jj200581(v=exchg.150).aspx)</span><span class="sxs-lookup"><span data-stu-id="6a4cf-128">[Exchange Server Hybrid Deployments](https://technet.microsoft.com/en-us/library/jj200581(v=exchg.150).aspx)</span></span>
- [<span data-ttu-id="6a4cf-129">2016 年 9 月の Cumulative Update リリース</span><span class="sxs-lookup"><span data-stu-id="6a4cf-129">September 2016 Cumulative Update Release</span></span>](https://blogs.technet.microsoft.com/exchange/2016/09/20/released-september-2016-quarterly-exchange-updates/) 
- [<span data-ttu-id="6a4cf-130">REST API のオンプレミス アーキテクチャ要件</span><span class="sxs-lookup"><span data-stu-id="6a4cf-130">On-Premises Architectural Requirements for the REST API</span></span>](https://blogs.technet.microsoft.com/exchange/2016/09/26/on-premises-architectural-requirements-for-the-rest-api/)
