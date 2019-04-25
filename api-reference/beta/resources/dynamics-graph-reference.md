---
title: Microsoft Graph で Dynamics 365 Business Central API を使用する
description: Microsoft Graph との統合のための API ドキュメント
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: ee67d28a90732bdc1d804da41994de32bf0a7f4f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543080"
---
# <a name="working-with-the-dynamics-365-business-central-api-in-microsoft-graph"></a><span data-ttu-id="d2b54-103">Microsoft Graph で Dynamics 365 Business Central API を使用する</span><span class="sxs-lookup"><span data-stu-id="d2b54-103">Working with the Dynamics 365 Business Central API in Microsoft Graph</span></span>
<span data-ttu-id="d2b54-104">microsoft Graph を使用して、microsoft Dynamics 365 Business Central と web サービスまたは SaaS ソリューションとの接続と統合を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="d2b54-104">You can use Microsoft Graph to connect and integrate your web service or SaaS solution with Microsoft Dynamics 365 Business Central.</span></span> <span data-ttu-id="d2b54-105">microsoft Graph を使用すると、microsoft Dynamics 365 Business Central data へのアクセスを許可し、シームレスに統合するアプリを作成できます。</span><span class="sxs-lookup"><span data-stu-id="d2b54-105">With Microsoft Graph, you can build apps that get authorized access to and integrate seamlessly with Microsoft Dynamics 365 Business Central data.</span></span>

## <a name="authorization"></a><span data-ttu-id="d2b54-106">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2b54-106">Authorization</span></span>
<span data-ttu-id="d2b54-107">Azure AD v2.0 エンドポイントを使用して、Dynamics 365 Business Central api を認証します。</span><span class="sxs-lookup"><span data-stu-id="d2b54-107">Use the Azure AD v2.0 endpoint to authenticate Dynamics 365 Business Central APIs.</span></span> <span data-ttu-id="d2b54-108">すべての api に`Authorization: Bearer {access-token}`は、要求ヘッダーが必要です。</span><span class="sxs-lookup"><span data-stu-id="d2b54-108">All APIs require the `Authorization: Bearer {access-token}` request header.</span></span> <span data-ttu-id="d2b54-109">承認の詳細については、「 [Microsoft Graph を呼び出せるようにアクセストークンを取得する](https://developer.microsoft.com/graph/docs/concepts/auth_overview)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d2b54-109">For more information about authorization, see [Get access tokens to call Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview).</span></span>

## <a name="common-dynamics-365-business-central-scenarios"></a><span data-ttu-id="d2b54-110">一般的な Dynamics 365 ビジネス中央シナリオ</span><span class="sxs-lookup"><span data-stu-id="d2b54-110">Common Dynamics 365 Business Central scenarios</span></span>
<span data-ttu-id="d2b54-111">Dynamics 365 Business Central API を使用すると、1つのエンドポイントを介して接続および統合されたアプリを使用して、ビジネスデータの読み取りと変更を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="d2b54-111">The Dynamics 365 Business Central API allows you to read and modify business data through apps that are connected and integrated through a single endpoint.</span></span> <span data-ttu-id="d2b54-112">たとえば、API を使用して[顧客](../resources/dynamics-customer.md)や[ベンダー](../resources/dynamics-vendor.md)の情報にアクセスしたり、[支払いの延滞を表示](../resources/dynamics-agedaccountspayable.md)したりします。</span><span class="sxs-lookup"><span data-stu-id="d2b54-112">Use the API to, for example, get access to [customer](../resources/dynamics-customer.md) and [vendor](../resources/dynamics-vendor.md) information, or [view overdue payments](../resources/dynamics-agedaccountspayable.md).</span></span>

## <a name="next-steps"></a><span data-ttu-id="d2b54-113">次の手順</span><span class="sxs-lookup"><span data-stu-id="d2b54-113">Next steps</span></span>
<span data-ttu-id="d2b54-114">Dynamics 365 Business Central API は、ユーザーと連携するための新しい方法を開くことができます。</span><span class="sxs-lookup"><span data-stu-id="d2b54-114">The Dynamics 365 Business Central API can open up new ways for you to engage with users.</span></span> <span data-ttu-id="d2b54-115">詳細については、次のトピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="d2b54-115">To learn more, see the following:</span></span>

+ [<span data-ttu-id="d2b54-116">Dynamics 365 Business Central の概要</span><span class="sxs-lookup"><span data-stu-id="d2b54-116">Dynamics 365 Business Central Overview</span></span>](/graph/dynamics-business-central-concept-overview)
+ <span data-ttu-id="d2b54-117">[Graph エクスプローラー](https://developer.microsoft.com/graph/graph-explorer)をお試しください。</span><span class="sxs-lookup"><span data-stu-id="d2b54-117">Try [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>

<!--
|For Resource Type |See                                                 |
|:-----------------|:---------------------------------------------------|
|account resource type|[account](../resources/dynamics-account.md)|
|aged accounts receivable resource type|[agedAccountsReceivable](../resources/dynamics-agedaccountsreceivable.md)|
|aged accounts payable resource type|[agedAccountsPayable](../resources/dynamics-agedaccountspayable.md)|
|balance sheet resource type|[balanceSheet](../resources/dynamics-balancesheet.md)|
|companies resource type|[companies](../resources/dynamics-companies.md)|
|companyInformation resource type|[companyInformation](../resources/dynamics-companyinformation.md)|
|countriesRegions resource type|[countriesRegions](../resources/dynamics-countriesregions.md)|
|currencies resource type|[currencies](../resources/dynamics-currencies.md)|
|customer resource type|[customer](../resources/dynamics-customer.md)|
|customerPaymentJournal resource type|[customerPaymentsJournal](../resources/dynamics-customerpaymentsjournal.md)|
|customerPayment resource type|[customerPayment](../resources/dynamics-customerpayment.md)|
|dimension resource type|[dimension](../resources/dynamics-dimension.md)|
|dimensionValue resource type|[dimensionValue](../resources/dynamics-dimensionvalue.md)
|employee resource type|[employee](../resources/dynamics-employee.md)|
|generalLedgerEntries resource type|[generalLedgerEntries](../resources/dynamics-generalledgerentries.md)|
|item resource type|[item](../resources/dynamics-item.md)|
|itemCategories resource type|[itemCategories](../resources/dynamics-itemcategories.md)|
|income statement resource type|[incomeStatement](../resources/dynamics-incomestatement.md)|
|IRS1099 resource type|[irs1099](../resources/dynamics-irs1099.md)|
|journal resource type|[journal](../resources/dynamics-journal.md)|
|journalLine resource type|[journalLine](../resources/dynamics-journalline.md)|
|paymentMethods resource type|[paymentMethods](../resources/dynamics-paymentmethods.md)|
|paymentTerms resource type|[paymentTerms](../resources/dynamics-paymentterms.md)|
|retained earnings statement resource type|[retainedEarningsStatement](../resources/dynamics-retainedearningsstatement.md)|
|shipmentMethods resource type|[shipmentMethods](../resources/dynamics-shipmentmethods.md)|
|taxGroups resource type|[taxGroups](../resources/dynamics-taxgroups.md)|
|taxArea resource type|[taxAreas](..resources/dynamics-taxarea.md)|
|trial balance resource type|[trialBalance](../resources/dynamics-trialbalance.md)|
|unitsOfMeasure resource type|[unitsOfMeasure](../resources/dynamics-unitsofmeasure.md)|
|vendor resource type|[vendor](../resources/dynamics-vendor.md)|
-->
