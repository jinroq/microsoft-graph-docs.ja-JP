---
title: androidForWorkCrossProfileDataSharingType 列挙型
description: Android の作業では、プロファイル データの種類の共有を横断します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6e2c407698807eda4fefa9d4ccc403380c3005f2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27942144"
---
# <a name="androidforworkcrossprofiledatasharingtype-enum-type"></a><span data-ttu-id="e9a75-103">androidForWorkCrossProfileDataSharingType 列挙型</span><span class="sxs-lookup"><span data-stu-id="e9a75-103">androidForWorkCrossProfileDataSharingType enum type</span></span>

> <span data-ttu-id="e9a75-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e9a75-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e9a75-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e9a75-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e9a75-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e9a75-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e9a75-107">Android の作業では、プロファイル データの種類の共有を横断します。</span><span class="sxs-lookup"><span data-stu-id="e9a75-107">Android For Work cross profile data sharing type.</span></span>
## <a name="members"></a><span data-ttu-id="e9a75-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="e9a75-108">Members</span></span>
|<span data-ttu-id="e9a75-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="e9a75-109">Member</span></span>|<span data-ttu-id="e9a75-110">値</span><span class="sxs-lookup"><span data-stu-id="e9a75-110">Value</span></span>|<span data-ttu-id="e9a75-111">説明</span><span class="sxs-lookup"><span data-stu-id="e9a75-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9a75-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="e9a75-112">deviceDefault</span></span>|<span data-ttu-id="e9a75-113">0</span><span class="sxs-lookup"><span data-stu-id="e9a75-113">0</span></span>|<span data-ttu-id="e9a75-114">デバイスの既定値でことを目的しません。</span><span class="sxs-lookup"><span data-stu-id="e9a75-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="e9a75-115">preventAny</span><span class="sxs-lookup"><span data-stu-id="e9a75-115">preventAny</span></span>|<span data-ttu-id="e9a75-116">1</span><span class="sxs-lookup"><span data-stu-id="e9a75-116">1</span></span>|<span data-ttu-id="e9a75-117">任意の共有を防止します。</span><span class="sxs-lookup"><span data-stu-id="e9a75-117">Prevent any sharing.</span></span>|
|<span data-ttu-id="e9a75-118">allowPersonalToWork</span><span class="sxs-lookup"><span data-stu-id="e9a75-118">allowPersonalToWork</span></span>|<span data-ttu-id="e9a75-119">2</span><span class="sxs-lookup"><span data-stu-id="e9a75-119">2</span></span>|<span data-ttu-id="e9a75-120">データ共有プロファイルを使用する個人のプロファイルからの要求を許可します。</span><span class="sxs-lookup"><span data-stu-id="e9a75-120">Allow data sharing request from personal profile to work profile.</span></span>|
|<span data-ttu-id="e9a75-121">noRestrictions</span><span class="sxs-lookup"><span data-stu-id="e9a75-121">noRestrictions</span></span>|<span data-ttu-id="e9a75-122">3</span><span class="sxs-lookup"><span data-stu-id="e9a75-122">3</span></span>|<span data-ttu-id="e9a75-123">共有の制限はありません。</span><span class="sxs-lookup"><span data-stu-id="e9a75-123">No restrictions on sharing.</span></span>|





