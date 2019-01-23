---
title: secureAssessmentAccountType 列挙型
description: Windows10SecureAssessment ConfigurationAccount に許可されているアカウントの種類です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2f9e620f87173708b852bd7eac79bee5a45e432c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409882"
---
# <a name="secureassessmentaccounttype-enum-type"></a><span data-ttu-id="c4112-103">secureAssessmentAccountType 列挙型</span><span class="sxs-lookup"><span data-stu-id="c4112-103">secureAssessmentAccountType enum type</span></span>

> <span data-ttu-id="c4112-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c4112-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c4112-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c4112-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c4112-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c4112-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4112-107">Windows10SecureAssessment ConfigurationAccount に許可されているアカウントの種類です。</span><span class="sxs-lookup"><span data-stu-id="c4112-107">Type of accounts that are allowed for Windows10SecureAssessment ConfigurationAccount.</span></span>

## <a name="members"></a><span data-ttu-id="c4112-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="c4112-108">Members</span></span>
|<span data-ttu-id="c4112-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="c4112-109">Member</span></span>|<span data-ttu-id="c4112-110">値</span><span class="sxs-lookup"><span data-stu-id="c4112-110">Value</span></span>|<span data-ttu-id="c4112-111">説明</span><span class="sxs-lookup"><span data-stu-id="c4112-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4112-112">azureADAccount</span><span class="sxs-lookup"><span data-stu-id="c4112-112">azureADAccount</span></span>|<span data-ttu-id="c4112-113">0</span><span class="sxs-lookup"><span data-stu-id="c4112-113">0</span></span>|<span data-ttu-id="c4112-114">AzureAD\ username@tenant.com の形式で、Azure AD アカウントを示します。</span><span class="sxs-lookup"><span data-stu-id="c4112-114">Indicates an Azure AD account in format of AzureAD\username@tenant.com.</span></span>|
|<span data-ttu-id="c4112-115">domainAccount</span><span class="sxs-lookup"><span data-stu-id="c4112-115">domainAccount</span></span>|<span data-ttu-id="c4112-116">1</span><span class="sxs-lookup"><span data-stu-id="c4112-116">1</span></span>|<span data-ttu-id="c4112-117">ドメイン \ ユーザーまたは user@domain.com の形式でドメイン アカウントを示します。</span><span class="sxs-lookup"><span data-stu-id="c4112-117">Indicates a domain account in format of domain\user or user@domain.com.</span></span>|
|<span data-ttu-id="c4112-118">ご覧</span><span class="sxs-lookup"><span data-stu-id="c4112-118">localAccount</span></span>|<span data-ttu-id="c4112-119">2</span><span class="sxs-lookup"><span data-stu-id="c4112-119">2</span></span>|<span data-ttu-id="c4112-120">ユーザー名の形式でローカル アカウントを示します。</span><span class="sxs-lookup"><span data-stu-id="c4112-120">Indicates a local account in format of username.</span></span>|




