---
title: subject代替/ベンダー ametype 列挙型
description: サブジェクトの別名オプション。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 89b638a00ca57b497a1447e0a5491563cd228e30
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166396"
---
# <a name="subjectalternativenametype-enum-type"></a><span data-ttu-id="72073-103">subject代替/ベンダー ametype 列挙型</span><span class="sxs-lookup"><span data-stu-id="72073-103">subjectAlternativeNameType enum type</span></span>

> <span data-ttu-id="72073-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="72073-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="72073-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="72073-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72073-106">サブジェクトの別名オプション。</span><span class="sxs-lookup"><span data-stu-id="72073-106">Subject Alternative Name Options.</span></span>

## <a name="members"></a><span data-ttu-id="72073-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="72073-107">Members</span></span>
|<span data-ttu-id="72073-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="72073-108">Member</span></span>|<span data-ttu-id="72073-109">値</span><span class="sxs-lookup"><span data-stu-id="72073-109">Value</span></span>|<span data-ttu-id="72073-110">説明</span><span class="sxs-lookup"><span data-stu-id="72073-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72073-111">none</span><span class="sxs-lookup"><span data-stu-id="72073-111">none</span></span>|<span data-ttu-id="72073-112">.0</span><span class="sxs-lookup"><span data-stu-id="72073-112">0</span></span>|<span data-ttu-id="72073-113">サブジェクトの別名がありません。</span><span class="sxs-lookup"><span data-stu-id="72073-113">No subject alternative name.</span></span>|
|<span data-ttu-id="72073-114">emailAddress</span><span class="sxs-lookup"><span data-stu-id="72073-114">emailAddress</span></span>|<span data-ttu-id="72073-115">1-d</span><span class="sxs-lookup"><span data-stu-id="72073-115">1</span></span>|<span data-ttu-id="72073-116">電子メールアドレス。</span><span class="sxs-lookup"><span data-stu-id="72073-116">Email address.</span></span>|
|<span data-ttu-id="72073-117">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="72073-117">userPrincipalName</span></span>|<span data-ttu-id="72073-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="72073-118">2</span></span>|<span data-ttu-id="72073-119">ユーザー プリンシパル名 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="72073-119">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="72073-120">customAzureADAttribute</span><span class="sxs-lookup"><span data-stu-id="72073-120">customAzureADAttribute</span></span>|<span data-ttu-id="72073-121">2/4</span><span class="sxs-lookup"><span data-stu-id="72073-121">4</span></span>|<span data-ttu-id="72073-122">カスタム Azure AD 属性。</span><span class="sxs-lookup"><span data-stu-id="72073-122">Custom Azure AD Attribute.</span></span>|
|<span data-ttu-id="72073-123">domainnameservice</span><span class="sxs-lookup"><span data-stu-id="72073-123">domainNameService</span></span>|<span data-ttu-id="72073-124">~</span><span class="sxs-lookup"><span data-stu-id="72073-124">8</span></span>|<span data-ttu-id="72073-125">ドメインネームサービス (DNS)。</span><span class="sxs-lookup"><span data-stu-id="72073-125">Domain Name Service (DNS).</span></span>|




