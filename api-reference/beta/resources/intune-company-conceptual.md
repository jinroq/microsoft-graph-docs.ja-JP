---
title: Microsoft Intune の会社の使用条件
description: Intune の使用条件をユーザー グループに展開して、登録、作業リソースへのアクセス、ポータル サイト アプリがデバイスやユーザーにどのように影響するかを説明することができます。 ポータル サイトを使用して自分の仕事に登録してアクセスするには、ユーザーはまず使用条件に同意する必要があります。
ms.openlocfilehash: 39f73700fd84537566454c9dcb3bc9fd17523c43
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073024"
---
# <a name="company-terms-and-conditions-in-microsoft-intune"></a><span data-ttu-id="0c1de-104">Microsoft Intune の会社の使用条件</span><span class="sxs-lookup"><span data-stu-id="0c1de-104">Company terms and conditions in Microsoft Intune</span></span>

> <span data-ttu-id="0c1de-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0c1de-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0c1de-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0c1de-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0c1de-107">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0c1de-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="0c1de-108">Intune の使用条件をユーザー グループに展開して、登録、作業リソースへのアクセス、ポータル サイト アプリがデバイスやユーザーにどのように影響するかを説明することができます。</span><span class="sxs-lookup"><span data-stu-id="0c1de-108">You can deploy Intune terms and conditions to user groups to explain how enrollment, access to work resources, and the Company Portal app affect devices and users.</span></span> <span data-ttu-id="0c1de-109">ポータル サイトを使用して自分の仕事に登録してアクセスするには、ユーザーはまず使用条件に同意する必要があります。</span><span class="sxs-lookup"><span data-stu-id="0c1de-109">Users must accept the terms and conditions before they can use the Company Portal to enroll and access their work.</span></span>

<span data-ttu-id="0c1de-110">さまざまな使用条件を含む複数のポリシーを作成して展開することができます。</span><span class="sxs-lookup"><span data-stu-id="0c1de-110">You can create and deploy multiple policies containing different terms and conditions.</span></span> <span data-ttu-id="0c1de-111">同じ使用条件のバージョンを異なる言語で作成し、それぞれ適切なグループに展開することもできます。</span><span class="sxs-lookup"><span data-stu-id="0c1de-111">You can also produce versions of the same terms and conditions in different languages and then deploy these to their appropriate groups.</span></span>

<span data-ttu-id="0c1de-112">次の Graph リソースを使用して、Intune での会社の使用条件を管理できます。</span><span class="sxs-lookup"><span data-stu-id="0c1de-112">The following Graph resources are available to manage company terms and conditions in Intune:</span></span>

- [<span data-ttu-id="0c1de-113">使用条件</span><span class="sxs-lookup"><span data-stu-id="0c1de-113">Terms and conditions</span></span>](intune-companyterms-termsandconditions.md)
- [<span data-ttu-id="0c1de-114">使用条件の承認状態</span><span class="sxs-lookup"><span data-stu-id="0c1de-114">Terms and conditions acceptance status</span></span>](intune-companyterms-termsandconditionsacceptancestatus.md)
- [<span data-ttu-id="0c1de-115">使用条件の割り当て</span><span class="sxs-lookup"><span data-stu-id="0c1de-115">Terms and conditions assignment</span></span>](intune-companyterms-termsandconditionsassignment.md)
- [<span data-ttu-id="0c1de-116">条項および条件は、割り当てをグループ化します。</span><span class="sxs-lookup"><span data-stu-id="0c1de-116">Terms and conditions group assignment</span></span>](intune-companyterms-termsandconditionsgroupassignment.md)
