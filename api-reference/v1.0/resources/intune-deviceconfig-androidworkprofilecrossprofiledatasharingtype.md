---
title: androidWorkProfileCrossProfileDataSharingType 列挙型
description: Android の作業プロファイルは、プロファイル データの種類の共有を横断します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7aa701f2e19ae008b0306d1d3c52fdcf53cbf33c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967274"
---
# <a name="androidworkprofilecrossprofiledatasharingtype-enum-type"></a><span data-ttu-id="afbd8-103">androidWorkProfileCrossProfileDataSharingType 列挙型</span><span class="sxs-lookup"><span data-stu-id="afbd8-103">androidWorkProfileCrossProfileDataSharingType enum type</span></span>

> <span data-ttu-id="afbd8-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="afbd8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="afbd8-105">Android の作業プロファイルは、プロファイル データの種類の共有を横断します。</span><span class="sxs-lookup"><span data-stu-id="afbd8-105">Android Work Profile cross profile data sharing type.</span></span>
## <a name="members"></a><span data-ttu-id="afbd8-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="afbd8-106">Members</span></span>
|<span data-ttu-id="afbd8-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="afbd8-107">Member</span></span>|<span data-ttu-id="afbd8-108">値</span><span class="sxs-lookup"><span data-stu-id="afbd8-108">Value</span></span>|<span data-ttu-id="afbd8-109">説明</span><span class="sxs-lookup"><span data-stu-id="afbd8-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="afbd8-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="afbd8-110">deviceDefault</span></span>|<span data-ttu-id="afbd8-111">0</span><span class="sxs-lookup"><span data-stu-id="afbd8-111">0</span></span>|<span data-ttu-id="afbd8-112">デバイスの既定値でことを目的しません。</span><span class="sxs-lookup"><span data-stu-id="afbd8-112">Device default value, no intent.</span></span>|
|<span data-ttu-id="afbd8-113">preventAny</span><span class="sxs-lookup"><span data-stu-id="afbd8-113">preventAny</span></span>|<span data-ttu-id="afbd8-114">1</span><span class="sxs-lookup"><span data-stu-id="afbd8-114">1</span></span>|<span data-ttu-id="afbd8-115">任意の共有を防止します。</span><span class="sxs-lookup"><span data-stu-id="afbd8-115">Prevent any sharing.</span></span>|
|<span data-ttu-id="afbd8-116">allowPersonalToWork</span><span class="sxs-lookup"><span data-stu-id="afbd8-116">allowPersonalToWork</span></span>|<span data-ttu-id="afbd8-117">2</span><span class="sxs-lookup"><span data-stu-id="afbd8-117">2</span></span>|<span data-ttu-id="afbd8-118">データ共有プロファイルを使用する個人のプロファイルからの要求を許可します。</span><span class="sxs-lookup"><span data-stu-id="afbd8-118">Allow data sharing request from personal profile to work profile.</span></span>|
|<span data-ttu-id="afbd8-119">noRestrictions</span><span class="sxs-lookup"><span data-stu-id="afbd8-119">noRestrictions</span></span>|<span data-ttu-id="afbd8-120">3</span><span class="sxs-lookup"><span data-stu-id="afbd8-120">3</span></span>|<span data-ttu-id="afbd8-121">共有の制限はありません。</span><span class="sxs-lookup"><span data-stu-id="afbd8-121">No restrictions on sharing.</span></span>|



