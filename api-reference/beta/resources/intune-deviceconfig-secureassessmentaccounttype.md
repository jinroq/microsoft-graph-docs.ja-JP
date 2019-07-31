---
title: secureAssessmentAccountType 列挙型
description: Windows10SecureAssessment ConfigurationAccount で許可されているアカウントの種類。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: f1f7e2b6b9cbc32ee41840d96b706322660fd2b2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36000558"
---
# <a name="secureassessmentaccounttype-enum-type"></a><span data-ttu-id="0737c-103">secureAssessmentAccountType 列挙型</span><span class="sxs-lookup"><span data-stu-id="0737c-103">secureAssessmentAccountType enum type</span></span>

> <span data-ttu-id="0737c-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0737c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0737c-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0737c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0737c-106">Windows10SecureAssessment ConfigurationAccount で許可されているアカウントの種類。</span><span class="sxs-lookup"><span data-stu-id="0737c-106">Type of accounts that are allowed for Windows10SecureAssessment ConfigurationAccount.</span></span>

## <a name="members"></a><span data-ttu-id="0737c-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="0737c-107">Members</span></span>
|<span data-ttu-id="0737c-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="0737c-108">Member</span></span>|<span data-ttu-id="0737c-109">値</span><span class="sxs-lookup"><span data-stu-id="0737c-109">Value</span></span>|<span data-ttu-id="0737c-110">説明</span><span class="sxs-lookup"><span data-stu-id="0737c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0737c-111">azureADAccount</span><span class="sxs-lookup"><span data-stu-id="0737c-111">azureADAccount</span></span>|<span data-ttu-id="0737c-112">.0</span><span class="sxs-lookup"><span data-stu-id="0737c-112">0</span></span>|<span data-ttu-id="0737c-113">Azure AD アカウントが AzureAD\username@tenant.com の形式であることを示します。</span><span class="sxs-lookup"><span data-stu-id="0737c-113">Indicates an Azure AD account in format of AzureAD\username@tenant.com.</span></span>|
|<span data-ttu-id="0737c-114">domainAccount</span><span class="sxs-lookup"><span data-stu-id="0737c-114">domainAccount</span></span>|<span data-ttu-id="0737c-115">1-d</span><span class="sxs-lookup"><span data-stu-id="0737c-115">1</span></span>|<span data-ttu-id="0737c-116">ドメインアカウントが domain\user または user@domain.com の形式であることを示します。</span><span class="sxs-lookup"><span data-stu-id="0737c-116">Indicates a domain account in format of domain\user or user@domain.com.</span></span>|
|<span data-ttu-id="0737c-117">localAccount</span><span class="sxs-lookup"><span data-stu-id="0737c-117">localAccount</span></span>|<span data-ttu-id="0737c-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="0737c-118">2</span></span>|<span data-ttu-id="0737c-119">ユーザー名の形式でローカルアカウントを示します。</span><span class="sxs-lookup"><span data-stu-id="0737c-119">Indicates a local account in format of username.</span></span>|
|<span data-ttu-id="0737c-120">localGuestAccount</span><span class="sxs-lookup"><span data-stu-id="0737c-120">localGuestAccount</span></span>|<span data-ttu-id="0737c-121">1/3</span><span class="sxs-lookup"><span data-stu-id="0737c-121">3</span></span>|<span data-ttu-id="0737c-122">テスト名の形式でローカルのゲストアカウントを示します。</span><span class="sxs-lookup"><span data-stu-id="0737c-122">Indicates a local guest account in format of test name.</span></span>|





