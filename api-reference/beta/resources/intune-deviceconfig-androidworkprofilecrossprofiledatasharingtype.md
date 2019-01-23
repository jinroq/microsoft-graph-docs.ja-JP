---
title: androidWorkProfileCrossProfileDataSharingType 列挙型
description: Android の作業プロファイルは、プロファイル データの種類の共有を横断します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 97001dcab56ef23506bee3d29c53757e3705fe04
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395637"
---
# <a name="androidworkprofilecrossprofiledatasharingtype-enum-type"></a><span data-ttu-id="ae7c6-103">androidWorkProfileCrossProfileDataSharingType 列挙型</span><span class="sxs-lookup"><span data-stu-id="ae7c6-103">androidWorkProfileCrossProfileDataSharingType enum type</span></span>

> <span data-ttu-id="ae7c6-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ae7c6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ae7c6-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ae7c6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ae7c6-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ae7c6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae7c6-107">Android の作業プロファイルは、プロファイル データの種類の共有を横断します。</span><span class="sxs-lookup"><span data-stu-id="ae7c6-107">Android Work Profile cross profile data sharing type.</span></span>

## <a name="members"></a><span data-ttu-id="ae7c6-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="ae7c6-108">Members</span></span>
|<span data-ttu-id="ae7c6-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="ae7c6-109">Member</span></span>|<span data-ttu-id="ae7c6-110">値</span><span class="sxs-lookup"><span data-stu-id="ae7c6-110">Value</span></span>|<span data-ttu-id="ae7c6-111">説明</span><span class="sxs-lookup"><span data-stu-id="ae7c6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae7c6-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="ae7c6-112">deviceDefault</span></span>|<span data-ttu-id="ae7c6-113">0</span><span class="sxs-lookup"><span data-stu-id="ae7c6-113">0</span></span>|<span data-ttu-id="ae7c6-114">デバイスの既定値でことを目的しません。</span><span class="sxs-lookup"><span data-stu-id="ae7c6-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="ae7c6-115">preventAny</span><span class="sxs-lookup"><span data-stu-id="ae7c6-115">preventAny</span></span>|<span data-ttu-id="ae7c6-116">1</span><span class="sxs-lookup"><span data-stu-id="ae7c6-116">1</span></span>|<span data-ttu-id="ae7c6-117">任意の共有を防止します。</span><span class="sxs-lookup"><span data-stu-id="ae7c6-117">Prevent any sharing.</span></span>|
|<span data-ttu-id="ae7c6-118">allowPersonalToWork</span><span class="sxs-lookup"><span data-stu-id="ae7c6-118">allowPersonalToWork</span></span>|<span data-ttu-id="ae7c6-119">2</span><span class="sxs-lookup"><span data-stu-id="ae7c6-119">2</span></span>|<span data-ttu-id="ae7c6-120">データ共有プロファイルを使用する個人のプロファイルからの要求を許可します。</span><span class="sxs-lookup"><span data-stu-id="ae7c6-120">Allow data sharing request from personal profile to work profile.</span></span>|
|<span data-ttu-id="ae7c6-121">noRestrictions</span><span class="sxs-lookup"><span data-stu-id="ae7c6-121">noRestrictions</span></span>|<span data-ttu-id="ae7c6-122">3</span><span class="sxs-lookup"><span data-stu-id="ae7c6-122">3</span></span>|<span data-ttu-id="ae7c6-123">共有の制限はありません。</span><span class="sxs-lookup"><span data-stu-id="ae7c6-123">No restrictions on sharing.</span></span>|




