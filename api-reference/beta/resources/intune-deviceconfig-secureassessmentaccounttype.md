---
title: secureAssessmentAccountType 列挙型
description: Windows10SecureAssessment ConfigurationAccount に許可されているアカウントの種類です。
author: tfitzmac
ms.openlocfilehash: faf504410336bdc491c29b676aaa1b57cd0a5ee2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27362224"
---
# <a name="secureassessmentaccounttype-enum-type"></a><span data-ttu-id="817e0-103">secureAssessmentAccountType 列挙型</span><span class="sxs-lookup"><span data-stu-id="817e0-103">secureAssessmentAccountType enum type</span></span>

> <span data-ttu-id="817e0-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="817e0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="817e0-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="817e0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="817e0-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="817e0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="817e0-107">Windows10SecureAssessment ConfigurationAccount に許可されているアカウントの種類です。</span><span class="sxs-lookup"><span data-stu-id="817e0-107">Type of accounts that are allowed for Windows10SecureAssessment ConfigurationAccount.</span></span>
## <a name="members"></a><span data-ttu-id="817e0-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="817e0-108">Members</span></span>
|<span data-ttu-id="817e0-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="817e0-109">Member</span></span>|<span data-ttu-id="817e0-110">値</span><span class="sxs-lookup"><span data-stu-id="817e0-110">Value</span></span>|<span data-ttu-id="817e0-111">説明</span><span class="sxs-lookup"><span data-stu-id="817e0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="817e0-112">azureADAccount</span><span class="sxs-lookup"><span data-stu-id="817e0-112">azureADAccount</span></span>|<span data-ttu-id="817e0-113">0</span><span class="sxs-lookup"><span data-stu-id="817e0-113">0</span></span>|<span data-ttu-id="817e0-114">AzureAD\ username@tenant.com の形式で、Azure AD アカウントを示します。</span><span class="sxs-lookup"><span data-stu-id="817e0-114">Indicates an Azure AD account in format of AzureAD\username@tenant.com.</span></span>|
|<span data-ttu-id="817e0-115">domainAccount</span><span class="sxs-lookup"><span data-stu-id="817e0-115">domainAccount</span></span>|<span data-ttu-id="817e0-116">1</span><span class="sxs-lookup"><span data-stu-id="817e0-116">1</span></span>|<span data-ttu-id="817e0-117">ドメイン \ ユーザーまたは user@domain.com の形式でドメイン アカウントを示します。</span><span class="sxs-lookup"><span data-stu-id="817e0-117">Indicates a domain account in format of domain\user or user@domain.com.</span></span>|
|<span data-ttu-id="817e0-118">ご覧</span><span class="sxs-lookup"><span data-stu-id="817e0-118">localAccount</span></span>|<span data-ttu-id="817e0-119">2</span><span class="sxs-lookup"><span data-stu-id="817e0-119">2</span></span>|<span data-ttu-id="817e0-120">ユーザー名の形式でローカル アカウントを示します。</span><span class="sxs-lookup"><span data-stu-id="817e0-120">Indicates a local account in format of username.</span></span>|





