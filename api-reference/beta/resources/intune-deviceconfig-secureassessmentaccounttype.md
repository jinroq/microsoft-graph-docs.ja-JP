---
title: secureAssessmentAccountType 列挙型
description: Windows10SecureAssessment ConfigurationAccount に許可されているアカウントの種類です。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5b1f8a3d03c0e7b9e91c68ff5a87611fcaa6f31e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826055"
---
# <a name="secureassessmentaccounttype-enum-type"></a><span data-ttu-id="286c7-103">secureAssessmentAccountType 列挙型</span><span class="sxs-lookup"><span data-stu-id="286c7-103">secureAssessmentAccountType enum type</span></span>

> <span data-ttu-id="286c7-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="286c7-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="286c7-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="286c7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="286c7-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="286c7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="286c7-107">Windows10SecureAssessment ConfigurationAccount に許可されているアカウントの種類です。</span><span class="sxs-lookup"><span data-stu-id="286c7-107">Type of accounts that are allowed for Windows10SecureAssessment ConfigurationAccount.</span></span>
## <a name="members"></a><span data-ttu-id="286c7-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="286c7-108">Members</span></span>
|<span data-ttu-id="286c7-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="286c7-109">Member</span></span>|<span data-ttu-id="286c7-110">値</span><span class="sxs-lookup"><span data-stu-id="286c7-110">Value</span></span>|<span data-ttu-id="286c7-111">説明</span><span class="sxs-lookup"><span data-stu-id="286c7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="286c7-112">azureADAccount</span><span class="sxs-lookup"><span data-stu-id="286c7-112">azureADAccount</span></span>|<span data-ttu-id="286c7-113">0</span><span class="sxs-lookup"><span data-stu-id="286c7-113">0</span></span>|<span data-ttu-id="286c7-114">AzureAD\ username@tenant.com の形式で、Azure AD アカウントを示します。</span><span class="sxs-lookup"><span data-stu-id="286c7-114">Indicates an Azure AD account in format of AzureAD\username@tenant.com.</span></span>|
|<span data-ttu-id="286c7-115">domainAccount</span><span class="sxs-lookup"><span data-stu-id="286c7-115">domainAccount</span></span>|<span data-ttu-id="286c7-116">1</span><span class="sxs-lookup"><span data-stu-id="286c7-116">1</span></span>|<span data-ttu-id="286c7-117">ドメイン \ ユーザーまたは user@domain.com の形式でドメイン アカウントを示します。</span><span class="sxs-lookup"><span data-stu-id="286c7-117">Indicates a domain account in format of domain\user or user@domain.com.</span></span>|
|<span data-ttu-id="286c7-118">ご覧</span><span class="sxs-lookup"><span data-stu-id="286c7-118">localAccount</span></span>|<span data-ttu-id="286c7-119">2</span><span class="sxs-lookup"><span data-stu-id="286c7-119">2</span></span>|<span data-ttu-id="286c7-120">ユーザー名の形式でローカル アカウントを示します。</span><span class="sxs-lookup"><span data-stu-id="286c7-120">Indicates a local account in format of username.</span></span>|





