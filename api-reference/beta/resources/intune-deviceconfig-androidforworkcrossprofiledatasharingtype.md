---
title: androidForWorkCrossProfileDataSharingType 列挙型
description: Android For Work クロスプロファイルデータ共有タイプ。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ec6c8f9a5300fb15ef8004322e06cc0cc2b28750
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32556320"
---
# <a name="androidforworkcrossprofiledatasharingtype-enum-type"></a><span data-ttu-id="b97bf-103">androidForWorkCrossProfileDataSharingType 列挙型</span><span class="sxs-lookup"><span data-stu-id="b97bf-103">androidForWorkCrossProfileDataSharingType enum type</span></span>

> <span data-ttu-id="b97bf-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b97bf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b97bf-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b97bf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b97bf-106">Android For Work クロスプロファイルデータ共有タイプ。</span><span class="sxs-lookup"><span data-stu-id="b97bf-106">Android For Work cross profile data sharing type.</span></span>

## <a name="members"></a><span data-ttu-id="b97bf-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="b97bf-107">Members</span></span>
|<span data-ttu-id="b97bf-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="b97bf-108">Member</span></span>|<span data-ttu-id="b97bf-109">値</span><span class="sxs-lookup"><span data-stu-id="b97bf-109">Value</span></span>|<span data-ttu-id="b97bf-110">説明</span><span class="sxs-lookup"><span data-stu-id="b97bf-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b97bf-111">devicedefault</span><span class="sxs-lookup"><span data-stu-id="b97bf-111">deviceDefault</span></span>|<span data-ttu-id="b97bf-112">.0</span><span class="sxs-lookup"><span data-stu-id="b97bf-112">0</span></span>|<span data-ttu-id="b97bf-113">デバイスの既定値。意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="b97bf-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="b97bf-114">preventAny</span><span class="sxs-lookup"><span data-stu-id="b97bf-114">preventAny</span></span>|<span data-ttu-id="b97bf-115">1 </span><span class="sxs-lookup"><span data-stu-id="b97bf-115">1</span></span>|<span data-ttu-id="b97bf-116">共有を禁止します。</span><span class="sxs-lookup"><span data-stu-id="b97bf-116">Prevent any sharing.</span></span>|
|<span data-ttu-id="b97bf-117">allowPersonalToWork</span><span class="sxs-lookup"><span data-stu-id="b97bf-117">allowPersonalToWork</span></span>|<span data-ttu-id="b97bf-118">2 </span><span class="sxs-lookup"><span data-stu-id="b97bf-118">2</span></span>|<span data-ttu-id="b97bf-119">個人プロファイルから作業プロファイルへのデータ共有要求を許可します。</span><span class="sxs-lookup"><span data-stu-id="b97bf-119">Allow data sharing request from personal profile to work profile.</span></span>|
|<span data-ttu-id="b97bf-120">noRestrictions</span><span class="sxs-lookup"><span data-stu-id="b97bf-120">noRestrictions</span></span>|<span data-ttu-id="b97bf-121">3 </span><span class="sxs-lookup"><span data-stu-id="b97bf-121">3</span></span>|<span data-ttu-id="b97bf-122">共有の制限はありません。</span><span class="sxs-lookup"><span data-stu-id="b97bf-122">No restrictions on sharing.</span></span>|





