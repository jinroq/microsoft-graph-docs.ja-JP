---
title: mobileAppPublishingState 列挙型
description: アプリの発行状態を示します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6ae8cdb97afb0b44acf268381c3cb128aaff9b7d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160166"
---
# <a name="mobileapppublishingstate-enum-type"></a><span data-ttu-id="d99e5-103">mobileAppPublishingState 列挙型</span><span class="sxs-lookup"><span data-stu-id="d99e5-103">mobileAppPublishingState enum type</span></span>

> <span data-ttu-id="d99e5-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d99e5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d99e5-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d99e5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d99e5-106">アプリの発行状態を示します。</span><span class="sxs-lookup"><span data-stu-id="d99e5-106">Indicates the publishing state of an app.</span></span>

## <a name="members"></a><span data-ttu-id="d99e5-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="d99e5-107">Members</span></span>
|<span data-ttu-id="d99e5-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="d99e5-108">Member</span></span>|<span data-ttu-id="d99e5-109">値</span><span class="sxs-lookup"><span data-stu-id="d99e5-109">Value</span></span>|<span data-ttu-id="d99e5-110">説明</span><span class="sxs-lookup"><span data-stu-id="d99e5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d99e5-111">notpublished</span><span class="sxs-lookup"><span data-stu-id="d99e5-111">notPublished</span></span>|<span data-ttu-id="d99e5-112">.0</span><span class="sxs-lookup"><span data-stu-id="d99e5-112">0</span></span>|<span data-ttu-id="d99e5-113">アプリはまだ公開されていません。</span><span class="sxs-lookup"><span data-stu-id="d99e5-113">The app is not yet published.</span></span>|
|<span data-ttu-id="d99e5-114">処理</span><span class="sxs-lookup"><span data-stu-id="d99e5-114">processing</span></span>|<span data-ttu-id="d99e5-115">1-d</span><span class="sxs-lookup"><span data-stu-id="d99e5-115">1</span></span>|<span data-ttu-id="d99e5-116">アプリは、サービス側の処理を保留しています。</span><span class="sxs-lookup"><span data-stu-id="d99e5-116">The app is pending service-side processing.</span></span>|
|<span data-ttu-id="d99e5-117">公開</span><span class="sxs-lookup"><span data-stu-id="d99e5-117">published</span></span>|<span data-ttu-id="d99e5-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="d99e5-118">2</span></span>|<span data-ttu-id="d99e5-119">アプリが発行されます。</span><span class="sxs-lookup"><span data-stu-id="d99e5-119">The app is published.</span></span>|




