---
title: secureAssessmentAccountType 列挙型
description: Windows10SecureAssessment ConfigurationAccount に許可されているアカウントの種類です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9e5ae78b5df3636e738cf21beece269e6fa7b81a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27959259"
---
# <a name="secureassessmentaccounttype-enum-type"></a><span data-ttu-id="247d7-103">secureAssessmentAccountType 列挙型</span><span class="sxs-lookup"><span data-stu-id="247d7-103">secureAssessmentAccountType enum type</span></span>

> <span data-ttu-id="247d7-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="247d7-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="247d7-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="247d7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="247d7-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="247d7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="247d7-107">Windows10SecureAssessment ConfigurationAccount に許可されているアカウントの種類です。</span><span class="sxs-lookup"><span data-stu-id="247d7-107">Type of accounts that are allowed for Windows10SecureAssessment ConfigurationAccount.</span></span>
## <a name="members"></a><span data-ttu-id="247d7-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="247d7-108">Members</span></span>
|<span data-ttu-id="247d7-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="247d7-109">Member</span></span>|<span data-ttu-id="247d7-110">値</span><span class="sxs-lookup"><span data-stu-id="247d7-110">Value</span></span>|<span data-ttu-id="247d7-111">説明</span><span class="sxs-lookup"><span data-stu-id="247d7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="247d7-112">azureADAccount</span><span class="sxs-lookup"><span data-stu-id="247d7-112">azureADAccount</span></span>|<span data-ttu-id="247d7-113">0</span><span class="sxs-lookup"><span data-stu-id="247d7-113">0</span></span>|<span data-ttu-id="247d7-114">AzureAD\ username@tenant.com の形式で、Azure AD アカウントを示します。</span><span class="sxs-lookup"><span data-stu-id="247d7-114">Indicates an Azure AD account in format of AzureAD\username@tenant.com.</span></span>|
|<span data-ttu-id="247d7-115">domainAccount</span><span class="sxs-lookup"><span data-stu-id="247d7-115">domainAccount</span></span>|<span data-ttu-id="247d7-116">1</span><span class="sxs-lookup"><span data-stu-id="247d7-116">1</span></span>|<span data-ttu-id="247d7-117">ドメイン \ ユーザーまたは user@domain.com の形式でドメイン アカウントを示します。</span><span class="sxs-lookup"><span data-stu-id="247d7-117">Indicates a domain account in format of domain\user or user@domain.com.</span></span>|
|<span data-ttu-id="247d7-118">ご覧</span><span class="sxs-lookup"><span data-stu-id="247d7-118">localAccount</span></span>|<span data-ttu-id="247d7-119">2</span><span class="sxs-lookup"><span data-stu-id="247d7-119">2</span></span>|<span data-ttu-id="247d7-120">ユーザー名の形式でローカル アカウントを示します。</span><span class="sxs-lookup"><span data-stu-id="247d7-120">Indicates a local account in format of username.</span></span>|





