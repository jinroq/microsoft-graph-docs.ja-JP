---
title: microsoft Intune での会社の使用条件-microsoft Graph API
description: テナント組織の使用条件を定義する Intune エンドポイント (REST) の Microsoft Graph API を一覧表示します。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 1277a6893ddd306b7050fafc70b815217d376b14
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172283"
---
# <a name="company-terms-and-conditions-in-microsoft-intune"></a><span data-ttu-id="d5247-103">Microsoft Intune の会社の使用条件</span><span class="sxs-lookup"><span data-stu-id="d5247-103">Company terms and conditions in Microsoft Intune</span></span>

> <span data-ttu-id="d5247-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d5247-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d5247-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d5247-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d5247-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d5247-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="d5247-107">Intune の使用条件をユーザー グループに展開して、登録、作業リソースへのアクセス、ポータル サイト アプリがデバイスやユーザーにどのように影響するかを説明することができます。</span><span class="sxs-lookup"><span data-stu-id="d5247-107">You can deploy Intune terms and conditions to user groups to explain how enrollment, access to work resources, and the Company Portal app affect devices and users.</span></span> <span data-ttu-id="d5247-108">ポータル サイトを使用して自分の仕事に登録してアクセスするには、ユーザーはまず使用条件に同意する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d5247-108">Users must accept the terms and conditions before they can use the Company Portal to enroll and access their work.</span></span>

<span data-ttu-id="d5247-109">さまざまな使用条件を含む複数のポリシーを作成して展開することができます。</span><span class="sxs-lookup"><span data-stu-id="d5247-109">You can create and deploy multiple policies containing different terms and conditions.</span></span> <span data-ttu-id="d5247-110">同じ使用条件のバージョンを異なる言語で作成し、それぞれ適切なグループに展開することもできます。</span><span class="sxs-lookup"><span data-stu-id="d5247-110">You can also produce versions of the same terms and conditions in different languages and then deploy these to their appropriate groups.</span></span>

<span data-ttu-id="d5247-111">次の Graph リソースを使用して、Intune での会社の使用条件を管理できます。</span><span class="sxs-lookup"><span data-stu-id="d5247-111">The following Graph resources are available to manage company terms and conditions in Intune:</span></span>

- [<span data-ttu-id="d5247-112">使用条件</span><span class="sxs-lookup"><span data-stu-id="d5247-112">Terms and conditions</span></span>](intune-companyterms-termsandconditions.md)
- [<span data-ttu-id="d5247-113">使用条件の承認状態</span><span class="sxs-lookup"><span data-stu-id="d5247-113">Terms and conditions acceptance status</span></span>](intune-companyterms-termsandconditionsacceptancestatus.md)
- [<span data-ttu-id="d5247-114">使用条件の割り当て</span><span class="sxs-lookup"><span data-stu-id="d5247-114">Terms and conditions assignment</span></span>](intune-companyterms-termsandconditionsassignment.md)
- [<span data-ttu-id="d5247-115">条項および条件のグループの割り当て</span><span class="sxs-lookup"><span data-stu-id="d5247-115">Terms and conditions group assignment</span></span>](intune-companyterms-termsandconditionsgroupassignment.md)
