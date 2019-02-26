---
title: mobileAppPublishingState 列挙型
description: アプリの発行状態を示します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0b0823576dd1792b01193d600cdebbe171b47052
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30263393"
---
# <a name="mobileapppublishingstate-enum-type"></a><span data-ttu-id="4a128-103">mobileAppPublishingState 列挙型</span><span class="sxs-lookup"><span data-stu-id="4a128-103">mobileAppPublishingState enum type</span></span>

> <span data-ttu-id="4a128-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4a128-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a128-105">アプリの発行状態を示します。</span><span class="sxs-lookup"><span data-stu-id="4a128-105">Indicates the publishing state of an app.</span></span>

## <a name="members"></a><span data-ttu-id="4a128-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="4a128-106">Members</span></span>
|<span data-ttu-id="4a128-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="4a128-107">Member</span></span>|<span data-ttu-id="4a128-108">値</span><span class="sxs-lookup"><span data-stu-id="4a128-108">Value</span></span>|<span data-ttu-id="4a128-109">説明</span><span class="sxs-lookup"><span data-stu-id="4a128-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a128-110">notpublished</span><span class="sxs-lookup"><span data-stu-id="4a128-110">notPublished</span></span>|<span data-ttu-id="4a128-111">.0</span><span class="sxs-lookup"><span data-stu-id="4a128-111">0</span></span>|<span data-ttu-id="4a128-112">アプリはまだ公開されていません。</span><span class="sxs-lookup"><span data-stu-id="4a128-112">The app is not yet published.</span></span>|
|<span data-ttu-id="4a128-113">処理</span><span class="sxs-lookup"><span data-stu-id="4a128-113">processing</span></span>|<span data-ttu-id="4a128-114">1-d</span><span class="sxs-lookup"><span data-stu-id="4a128-114">1</span></span>|<span data-ttu-id="4a128-115">アプリは、サービス側の処理を保留しています。</span><span class="sxs-lookup"><span data-stu-id="4a128-115">The app is pending service-side processing.</span></span>|
|<span data-ttu-id="4a128-116">公開</span><span class="sxs-lookup"><span data-stu-id="4a128-116">published</span></span>|<span data-ttu-id="4a128-117">pbm-2</span><span class="sxs-lookup"><span data-stu-id="4a128-117">2</span></span>|<span data-ttu-id="4a128-118">アプリが発行されます。</span><span class="sxs-lookup"><span data-stu-id="4a128-118">The app is published.</span></span>|



