---
title: Microsoft Graph で Dynamics 365 Business Central API を使用する
description: Microsoft Graph との統合のための API ドキュメント
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: ee67d28a90732bdc1d804da41994de32bf0a7f4f
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366593"
---
# <a name="working-with-the-dynamics-365-business-central-api-in-microsoft-graph"></a>Microsoft Graph で Dynamics 365 Business Central API を使用する
microsoft Graph を使用して、microsoft Dynamics 365 Business Central と web サービスまたは SaaS ソリューションとの接続と統合を行うことができます。 microsoft Graph を使用すると、microsoft Dynamics 365 Business Central data へのアクセスを許可し、シームレスに統合するアプリを作成できます。

## <a name="authorization"></a>Authorization
Azure AD v2.0 エンドポイントを使用して、Dynamics 365 Business Central api を認証します。 すべての api に`Authorization: Bearer {access-token}`は、要求ヘッダーが必要です。 承認の詳細については、「 [Microsoft Graph を呼び出せるようにアクセストークンを取得する](https://developer.microsoft.com/graph/docs/concepts/auth_overview)」を参照してください。

## <a name="common-dynamics-365-business-central-scenarios"></a>一般的な Dynamics 365 ビジネス中央シナリオ
Dynamics 365 Business Central API を使用すると、1つのエンドポイントを介して接続および統合されたアプリを使用して、ビジネスデータの読み取りと変更を行うことができます。 たとえば、API を使用して[顧客](../resources/dynamics-customer.md)や[ベンダー](../resources/dynamics-vendor.md)の情報にアクセスしたり、[支払いの延滞を表示](../resources/dynamics-agedaccountspayable.md)したりします。

## <a name="next-steps"></a>次の手順
Dynamics 365 Business Central API は、ユーザーと連携するための新しい方法を開くことができます。 詳細については、以下を参照してください。

+ [Dynamics 365 Business Central の概要](/graph/dynamics-business-central-concept-overview)
+ [Graph エクスプローラー](https://developer.microsoft.com/graph/graph-explorer)をお試しください。

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
