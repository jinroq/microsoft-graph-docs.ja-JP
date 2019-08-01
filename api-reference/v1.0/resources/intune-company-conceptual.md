---
title: Microsoft Intune での会社の使用条件-Microsoft Graph API
description: 会社の使用条件をサポートする Intune (REST) エンドポイントの Microsoft Graph API を一覧表示します。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: 31178d6acccdae972ead9941feb2a8f98b51a7ba
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028771"
---
# <a name="company-terms-and-conditions-in-microsoft-intune"></a><span data-ttu-id="343b6-103">Microsoft Intune の会社の使用条件</span><span class="sxs-lookup"><span data-stu-id="343b6-103">Company terms and conditions in Microsoft Intune</span></span>

> <span data-ttu-id="343b6-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="343b6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="343b6-105">Intune の使用条件をユーザー グループに展開して、登録、作業リソースへのアクセス、ポータル サイト アプリがデバイスやユーザーにどのように影響するかを説明することができます。</span><span class="sxs-lookup"><span data-stu-id="343b6-105">You can deploy Intune terms and conditions to user groups to explain how enrollment, access to work resources, and the Company Portal app affect devices and users.</span></span> <span data-ttu-id="343b6-106">ポータル サイトを使用して自分の仕事に登録してアクセスするには、ユーザーはまず使用条件に同意する必要があります。</span><span class="sxs-lookup"><span data-stu-id="343b6-106">Users must accept the terms and conditions before they can use the Company Portal to enroll and access their work.</span></span>

<span data-ttu-id="343b6-107">さまざまな使用条件を含む複数のポリシーを作成して展開することができます。</span><span class="sxs-lookup"><span data-stu-id="343b6-107">You can create and deploy multiple policies containing different terms and conditions.</span></span> <span data-ttu-id="343b6-108">同じ使用条件のバージョンを異なる言語で作成し、それぞれ適切なグループに展開することもできます。</span><span class="sxs-lookup"><span data-stu-id="343b6-108">You can also produce versions of the same terms and conditions in different languages and then deploy these to their appropriate groups.</span></span>

<span data-ttu-id="343b6-109">次の Graph リソースを使用して、Intune での会社の使用条件を管理できます。</span><span class="sxs-lookup"><span data-stu-id="343b6-109">The following Graph resources are available to manage company terms and conditions in Intune:</span></span>

- [<span data-ttu-id="343b6-110">使用条件</span><span class="sxs-lookup"><span data-stu-id="343b6-110">Terms and conditions</span></span>](intune-companyterms-termsandconditions.md)
- [<span data-ttu-id="343b6-111">使用条件の承認状態</span><span class="sxs-lookup"><span data-stu-id="343b6-111">Terms and conditions acceptance status</span></span>](intune-companyterms-termsandconditionsacceptancestatus.md)
- [<span data-ttu-id="343b6-112">使用条件の割り当て</span><span class="sxs-lookup"><span data-stu-id="343b6-112">Terms and conditions assignment</span></span>](intune-companyterms-termsandconditionsassignment.md)
