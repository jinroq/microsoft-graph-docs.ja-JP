---
title: secureAssessmentAccountType 列挙型
description: Windows10SecureAssessment ConfigurationAccount で許可されているアカウントの種類。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8ff967766321b5e7be5dd33944a02e4ed2bdc280
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34986649"
---
# <a name="secureassessmentaccounttype-enum-type"></a><span data-ttu-id="89729-103">secureAssessmentAccountType 列挙型</span><span class="sxs-lookup"><span data-stu-id="89729-103">secureAssessmentAccountType enum type</span></span>

> <span data-ttu-id="89729-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="89729-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="89729-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="89729-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89729-106">Windows10SecureAssessment ConfigurationAccount で許可されているアカウントの種類。</span><span class="sxs-lookup"><span data-stu-id="89729-106">Type of accounts that are allowed for Windows10SecureAssessment ConfigurationAccount.</span></span>

## <a name="members"></a><span data-ttu-id="89729-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="89729-107">Members</span></span>
|<span data-ttu-id="89729-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="89729-108">Member</span></span>|<span data-ttu-id="89729-109">値</span><span class="sxs-lookup"><span data-stu-id="89729-109">Value</span></span>|<span data-ttu-id="89729-110">説明</span><span class="sxs-lookup"><span data-stu-id="89729-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89729-111">azureADAccount</span><span class="sxs-lookup"><span data-stu-id="89729-111">azureADAccount</span></span>|<span data-ttu-id="89729-112">.0</span><span class="sxs-lookup"><span data-stu-id="89729-112">0</span></span>|<span data-ttu-id="89729-113">Azure AD アカウントが AzureAD\username@tenant.com の形式であることを示します。</span><span class="sxs-lookup"><span data-stu-id="89729-113">Indicates an Azure AD account in format of AzureAD\username@tenant.com.</span></span>|
|<span data-ttu-id="89729-114">domainAccount</span><span class="sxs-lookup"><span data-stu-id="89729-114">domainAccount</span></span>|<span data-ttu-id="89729-115">1-d</span><span class="sxs-lookup"><span data-stu-id="89729-115">1</span></span>|<span data-ttu-id="89729-116">ドメインアカウントが domain\user または user@domain.com の形式であることを示します。</span><span class="sxs-lookup"><span data-stu-id="89729-116">Indicates a domain account in format of domain\user or user@domain.com.</span></span>|
|<span data-ttu-id="89729-117">localAccount</span><span class="sxs-lookup"><span data-stu-id="89729-117">localAccount</span></span>|<span data-ttu-id="89729-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="89729-118">2</span></span>|<span data-ttu-id="89729-119">ユーザー名の形式でローカルアカウントを示します。</span><span class="sxs-lookup"><span data-stu-id="89729-119">Indicates a local account in format of username.</span></span>|





