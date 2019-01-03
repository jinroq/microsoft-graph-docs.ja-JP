---
title: androidWorkProfileCrossProfileDataSharingType 列挙型
description: Android の作業プロファイルは、プロファイル データの種類の共有を横断します。
author: tfitzmac
ms.openlocfilehash: 278d9af142128003cf05b69f1cce340eb155f973
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308153"
---
# <a name="androidworkprofilecrossprofiledatasharingtype-enum-type"></a><span data-ttu-id="33d7e-103">androidWorkProfileCrossProfileDataSharingType 列挙型</span><span class="sxs-lookup"><span data-stu-id="33d7e-103">androidWorkProfileCrossProfileDataSharingType enum type</span></span>

> <span data-ttu-id="33d7e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="33d7e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="33d7e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="33d7e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="33d7e-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="33d7e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="33d7e-107">Android の作業プロファイルは、プロファイル データの種類の共有を横断します。</span><span class="sxs-lookup"><span data-stu-id="33d7e-107">Android Work Profile cross profile data sharing type.</span></span>
## <a name="members"></a><span data-ttu-id="33d7e-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="33d7e-108">Members</span></span>
|<span data-ttu-id="33d7e-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="33d7e-109">Member</span></span>|<span data-ttu-id="33d7e-110">値</span><span class="sxs-lookup"><span data-stu-id="33d7e-110">Value</span></span>|<span data-ttu-id="33d7e-111">説明</span><span class="sxs-lookup"><span data-stu-id="33d7e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33d7e-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="33d7e-112">deviceDefault</span></span>|<span data-ttu-id="33d7e-113">0</span><span class="sxs-lookup"><span data-stu-id="33d7e-113">0</span></span>|<span data-ttu-id="33d7e-114">デバイスの既定値でことを目的しません。</span><span class="sxs-lookup"><span data-stu-id="33d7e-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="33d7e-115">preventAny</span><span class="sxs-lookup"><span data-stu-id="33d7e-115">preventAny</span></span>|<span data-ttu-id="33d7e-116">1</span><span class="sxs-lookup"><span data-stu-id="33d7e-116">1</span></span>|<span data-ttu-id="33d7e-117">任意の共有を防止します。</span><span class="sxs-lookup"><span data-stu-id="33d7e-117">Prevent any sharing.</span></span>|
|<span data-ttu-id="33d7e-118">allowPersonalToWork</span><span class="sxs-lookup"><span data-stu-id="33d7e-118">allowPersonalToWork</span></span>|<span data-ttu-id="33d7e-119">2</span><span class="sxs-lookup"><span data-stu-id="33d7e-119">2</span></span>|<span data-ttu-id="33d7e-120">データ共有プロファイルを使用する個人のプロファイルからの要求を許可します。</span><span class="sxs-lookup"><span data-stu-id="33d7e-120">Allow data sharing request from personal profile to work profile.</span></span>|
|<span data-ttu-id="33d7e-121">noRestrictions</span><span class="sxs-lookup"><span data-stu-id="33d7e-121">noRestrictions</span></span>|<span data-ttu-id="33d7e-122">3</span><span class="sxs-lookup"><span data-stu-id="33d7e-122">3</span></span>|<span data-ttu-id="33d7e-123">共有の制限はありません。</span><span class="sxs-lookup"><span data-stu-id="33d7e-123">No restrictions on sharing.</span></span>|




