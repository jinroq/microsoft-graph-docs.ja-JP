---
title: androidWorkProfileCrossProfileDataSharingType 列挙型
description: Android の作業プロファイルは、プロファイル データの種類の共有を横断します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 138834bcfa9bfd4f64f3eb9e801c975eb16b38c2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871961"
---
# <a name="androidworkprofilecrossprofiledatasharingtype-enum-type"></a><span data-ttu-id="b67c4-103">androidWorkProfileCrossProfileDataSharingType 列挙型</span><span class="sxs-lookup"><span data-stu-id="b67c4-103">androidWorkProfileCrossProfileDataSharingType enum type</span></span>

> <span data-ttu-id="b67c4-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b67c4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b67c4-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b67c4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b67c4-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b67c4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b67c4-107">Android の作業プロファイルは、プロファイル データの種類の共有を横断します。</span><span class="sxs-lookup"><span data-stu-id="b67c4-107">Android Work Profile cross profile data sharing type.</span></span>
## <a name="members"></a><span data-ttu-id="b67c4-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="b67c4-108">Members</span></span>
|<span data-ttu-id="b67c4-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="b67c4-109">Member</span></span>|<span data-ttu-id="b67c4-110">値</span><span class="sxs-lookup"><span data-stu-id="b67c4-110">Value</span></span>|<span data-ttu-id="b67c4-111">説明</span><span class="sxs-lookup"><span data-stu-id="b67c4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b67c4-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="b67c4-112">deviceDefault</span></span>|<span data-ttu-id="b67c4-113">0</span><span class="sxs-lookup"><span data-stu-id="b67c4-113">0</span></span>|<span data-ttu-id="b67c4-114">デバイスの既定値でことを目的しません。</span><span class="sxs-lookup"><span data-stu-id="b67c4-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="b67c4-115">preventAny</span><span class="sxs-lookup"><span data-stu-id="b67c4-115">preventAny</span></span>|<span data-ttu-id="b67c4-116">1</span><span class="sxs-lookup"><span data-stu-id="b67c4-116">1</span></span>|<span data-ttu-id="b67c4-117">任意の共有を防止します。</span><span class="sxs-lookup"><span data-stu-id="b67c4-117">Prevent any sharing.</span></span>|
|<span data-ttu-id="b67c4-118">allowPersonalToWork</span><span class="sxs-lookup"><span data-stu-id="b67c4-118">allowPersonalToWork</span></span>|<span data-ttu-id="b67c4-119">2</span><span class="sxs-lookup"><span data-stu-id="b67c4-119">2</span></span>|<span data-ttu-id="b67c4-120">データ共有プロファイルを使用する個人のプロファイルからの要求を許可します。</span><span class="sxs-lookup"><span data-stu-id="b67c4-120">Allow data sharing request from personal profile to work profile.</span></span>|
|<span data-ttu-id="b67c4-121">noRestrictions</span><span class="sxs-lookup"><span data-stu-id="b67c4-121">noRestrictions</span></span>|<span data-ttu-id="b67c4-122">3</span><span class="sxs-lookup"><span data-stu-id="b67c4-122">3</span></span>|<span data-ttu-id="b67c4-123">共有の制限はありません。</span><span class="sxs-lookup"><span data-stu-id="b67c4-123">No restrictions on sharing.</span></span>|





