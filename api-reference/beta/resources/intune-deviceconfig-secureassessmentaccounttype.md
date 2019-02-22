---
title: secureAssessmentAccountType 列挙型
description: Windows10SecureAssessment configurationaccount で許可されているアカウントの種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f6698086b3da16466e9069781312e15ccd7c80c3
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30169378"
---
# <a name="secureassessmentaccounttype-enum-type"></a><span data-ttu-id="55028-103">secureAssessmentAccountType 列挙型</span><span class="sxs-lookup"><span data-stu-id="55028-103">secureAssessmentAccountType enum type</span></span>

> <span data-ttu-id="55028-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="55028-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="55028-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="55028-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55028-106">Windows10SecureAssessment configurationaccount で許可されているアカウントの種類。</span><span class="sxs-lookup"><span data-stu-id="55028-106">Type of accounts that are allowed for Windows10SecureAssessment ConfigurationAccount.</span></span>

## <a name="members"></a><span data-ttu-id="55028-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="55028-107">Members</span></span>
|<span data-ttu-id="55028-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="55028-108">Member</span></span>|<span data-ttu-id="55028-109">値</span><span class="sxs-lookup"><span data-stu-id="55028-109">Value</span></span>|<span data-ttu-id="55028-110">説明</span><span class="sxs-lookup"><span data-stu-id="55028-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55028-111">azureADAccount</span><span class="sxs-lookup"><span data-stu-id="55028-111">azureADAccount</span></span>|<span data-ttu-id="55028-112">.0</span><span class="sxs-lookup"><span data-stu-id="55028-112">0</span></span>|<span data-ttu-id="55028-113">Azure AD アカウントが AzureAD\username@tenant.com の形式であることを示します。</span><span class="sxs-lookup"><span data-stu-id="55028-113">Indicates an Azure AD account in format of AzureAD\username@tenant.com.</span></span>|
|<span data-ttu-id="55028-114">domainaccount</span><span class="sxs-lookup"><span data-stu-id="55028-114">domainAccount</span></span>|<span data-ttu-id="55028-115">1-d</span><span class="sxs-lookup"><span data-stu-id="55028-115">1</span></span>|<span data-ttu-id="55028-116">ドメインアカウントが domain\user または user@domain.com の形式であることを示します。</span><span class="sxs-lookup"><span data-stu-id="55028-116">Indicates a domain account in format of domain\user or user@domain.com.</span></span>|
|<span data-ttu-id="55028-117">localaccount</span><span class="sxs-lookup"><span data-stu-id="55028-117">localAccount</span></span>|<span data-ttu-id="55028-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="55028-118">2</span></span>|<span data-ttu-id="55028-119">ユーザー名の形式でローカルアカウントを示します。</span><span class="sxs-lookup"><span data-stu-id="55028-119">Indicates a local account in format of username.</span></span>|




