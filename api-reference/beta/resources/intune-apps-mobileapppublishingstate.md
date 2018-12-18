---
title: mobileAppPublishingState 列挙型
description: アプリケーションの発行状態を示します。
author: tfitzmac
ms.openlocfilehash: 2415e2ba244d7766cbdc670c303643ec125c1091
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302332"
---
# <a name="mobileapppublishingstate-enum-type"></a><span data-ttu-id="b8ee3-103">mobileAppPublishingState 列挙型</span><span class="sxs-lookup"><span data-stu-id="b8ee3-103">mobileAppPublishingState enum type</span></span>

> <span data-ttu-id="b8ee3-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b8ee3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b8ee3-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b8ee3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b8ee3-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b8ee3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b8ee3-107">アプリケーションの発行状態を示します。</span><span class="sxs-lookup"><span data-stu-id="b8ee3-107">Indicates the publishing state of an app.</span></span>
## <a name="members"></a><span data-ttu-id="b8ee3-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="b8ee3-108">Members</span></span>
|<span data-ttu-id="b8ee3-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="b8ee3-109">Member</span></span>|<span data-ttu-id="b8ee3-110">値</span><span class="sxs-lookup"><span data-stu-id="b8ee3-110">Value</span></span>|<span data-ttu-id="b8ee3-111">説明</span><span class="sxs-lookup"><span data-stu-id="b8ee3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8ee3-112">notPublished</span><span class="sxs-lookup"><span data-stu-id="b8ee3-112">notPublished</span></span>|<span data-ttu-id="b8ee3-113">0</span><span class="sxs-lookup"><span data-stu-id="b8ee3-113">0</span></span>|<span data-ttu-id="b8ee3-114">アプリケーションはまだ公開されていません。</span><span class="sxs-lookup"><span data-stu-id="b8ee3-114">The app is not yet published.</span></span>|
|<span data-ttu-id="b8ee3-115">処理</span><span class="sxs-lookup"><span data-stu-id="b8ee3-115">processing</span></span>|<span data-ttu-id="b8ee3-116">1</span><span class="sxs-lookup"><span data-stu-id="b8ee3-116">1</span></span>|<span data-ttu-id="b8ee3-117">アプリケーションは、サービス側の処理を保留中です。</span><span class="sxs-lookup"><span data-stu-id="b8ee3-117">The app is pending service-side processing.</span></span>|
|<span data-ttu-id="b8ee3-118">公開</span><span class="sxs-lookup"><span data-stu-id="b8ee3-118">published</span></span>|<span data-ttu-id="b8ee3-119">2</span><span class="sxs-lookup"><span data-stu-id="b8ee3-119">2</span></span>|<span data-ttu-id="b8ee3-120">アプリケーションが発行されます。</span><span class="sxs-lookup"><span data-stu-id="b8ee3-120">The app is published.</span></span>|





