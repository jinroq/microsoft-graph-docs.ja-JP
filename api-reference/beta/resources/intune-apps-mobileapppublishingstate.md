---
title: mobileAppPublishingState 列挙型
description: アプリケーションの発行状態を示します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 24a17e63570d46a1fd1771bf25e5bd0d397f9088
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27890987"
---
# <a name="mobileapppublishingstate-enum-type"></a><span data-ttu-id="4eea2-103">mobileAppPublishingState 列挙型</span><span class="sxs-lookup"><span data-stu-id="4eea2-103">mobileAppPublishingState enum type</span></span>

> <span data-ttu-id="4eea2-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4eea2-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4eea2-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4eea2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4eea2-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4eea2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4eea2-107">アプリケーションの発行状態を示します。</span><span class="sxs-lookup"><span data-stu-id="4eea2-107">Indicates the publishing state of an app.</span></span>
## <a name="members"></a><span data-ttu-id="4eea2-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="4eea2-108">Members</span></span>
|<span data-ttu-id="4eea2-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="4eea2-109">Member</span></span>|<span data-ttu-id="4eea2-110">値</span><span class="sxs-lookup"><span data-stu-id="4eea2-110">Value</span></span>|<span data-ttu-id="4eea2-111">説明</span><span class="sxs-lookup"><span data-stu-id="4eea2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4eea2-112">notPublished</span><span class="sxs-lookup"><span data-stu-id="4eea2-112">notPublished</span></span>|<span data-ttu-id="4eea2-113">0</span><span class="sxs-lookup"><span data-stu-id="4eea2-113">0</span></span>|<span data-ttu-id="4eea2-114">アプリケーションはまだ公開されていません。</span><span class="sxs-lookup"><span data-stu-id="4eea2-114">The app is not yet published.</span></span>|
|<span data-ttu-id="4eea2-115">処理</span><span class="sxs-lookup"><span data-stu-id="4eea2-115">processing</span></span>|<span data-ttu-id="4eea2-116">1</span><span class="sxs-lookup"><span data-stu-id="4eea2-116">1</span></span>|<span data-ttu-id="4eea2-117">アプリケーションは、サービス側の処理を保留中です。</span><span class="sxs-lookup"><span data-stu-id="4eea2-117">The app is pending service-side processing.</span></span>|
|<span data-ttu-id="4eea2-118">公開</span><span class="sxs-lookup"><span data-stu-id="4eea2-118">published</span></span>|<span data-ttu-id="4eea2-119">2</span><span class="sxs-lookup"><span data-stu-id="4eea2-119">2</span></span>|<span data-ttu-id="4eea2-120">アプリケーションが発行されます。</span><span class="sxs-lookup"><span data-stu-id="4eea2-120">The app is published.</span></span>|





