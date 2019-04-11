---
title: secureAssessmentAccountType 列挙型
description: Windows10SecureAssessment configurationaccount で許可されているアカウントの種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4fa14d90465ed9278fd20362800d5d111de62950
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31795010"
---
# <a name="secureassessmentaccounttype-enum-type"></a><span data-ttu-id="51e56-103">secureAssessmentAccountType 列挙型</span><span class="sxs-lookup"><span data-stu-id="51e56-103">secureAssessmentAccountType enum type</span></span>

> <span data-ttu-id="51e56-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="51e56-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="51e56-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="51e56-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51e56-106">Windows10SecureAssessment configurationaccount で許可されているアカウントの種類。</span><span class="sxs-lookup"><span data-stu-id="51e56-106">Type of accounts that are allowed for Windows10SecureAssessment ConfigurationAccount.</span></span>

## <a name="members"></a><span data-ttu-id="51e56-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="51e56-107">Members</span></span>
|<span data-ttu-id="51e56-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="51e56-108">Member</span></span>|<span data-ttu-id="51e56-109">値</span><span class="sxs-lookup"><span data-stu-id="51e56-109">Value</span></span>|<span data-ttu-id="51e56-110">説明</span><span class="sxs-lookup"><span data-stu-id="51e56-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51e56-111">azureADAccount</span><span class="sxs-lookup"><span data-stu-id="51e56-111">azureADAccount</span></span>|<span data-ttu-id="51e56-112">.0</span><span class="sxs-lookup"><span data-stu-id="51e56-112">0</span></span>|<span data-ttu-id="51e56-113">Azure AD アカウントがのAzureAD\username@tenant.com形式であることを示します。</span><span class="sxs-lookup"><span data-stu-id="51e56-113">Indicates an Azure AD account in format of AzureAD\username@tenant.com.</span></span>|
|<span data-ttu-id="51e56-114">domainaccount</span><span class="sxs-lookup"><span data-stu-id="51e56-114">domainAccount</span></span>|<span data-ttu-id="51e56-115">1-d</span><span class="sxs-lookup"><span data-stu-id="51e56-115">1</span></span>|<span data-ttu-id="51e56-116">ドメインアカウントが domain\user またはuser@domain.comの形式であることを示します。</span><span class="sxs-lookup"><span data-stu-id="51e56-116">Indicates a domain account in format of domain\user or user@domain.com.</span></span>|
|<span data-ttu-id="51e56-117">localaccount</span><span class="sxs-lookup"><span data-stu-id="51e56-117">localAccount</span></span>|<span data-ttu-id="51e56-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="51e56-118">2</span></span>|<span data-ttu-id="51e56-119">ユーザー名の形式でローカルアカウントを示します。</span><span class="sxs-lookup"><span data-stu-id="51e56-119">Indicates a local account in format of username.</span></span>|





