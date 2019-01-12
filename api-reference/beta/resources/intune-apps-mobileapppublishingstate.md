---
title: mobileAppPublishingState 列挙型
description: アプリケーションの発行状態を示します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6b2ae893a0c971bfa0a80a09bb8e7c80b6146555
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932820"
---
# <a name="mobileapppublishingstate-enum-type"></a><span data-ttu-id="79734-103">mobileAppPublishingState 列挙型</span><span class="sxs-lookup"><span data-stu-id="79734-103">mobileAppPublishingState enum type</span></span>

> <span data-ttu-id="79734-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="79734-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="79734-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="79734-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="79734-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="79734-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="79734-107">アプリケーションの発行状態を示します。</span><span class="sxs-lookup"><span data-stu-id="79734-107">Indicates the publishing state of an app.</span></span>
## <a name="members"></a><span data-ttu-id="79734-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="79734-108">Members</span></span>
|<span data-ttu-id="79734-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="79734-109">Member</span></span>|<span data-ttu-id="79734-110">値</span><span class="sxs-lookup"><span data-stu-id="79734-110">Value</span></span>|<span data-ttu-id="79734-111">説明</span><span class="sxs-lookup"><span data-stu-id="79734-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79734-112">notPublished</span><span class="sxs-lookup"><span data-stu-id="79734-112">notPublished</span></span>|<span data-ttu-id="79734-113">0</span><span class="sxs-lookup"><span data-stu-id="79734-113">0</span></span>|<span data-ttu-id="79734-114">アプリケーションはまだ公開されていません。</span><span class="sxs-lookup"><span data-stu-id="79734-114">The app is not yet published.</span></span>|
|<span data-ttu-id="79734-115">処理</span><span class="sxs-lookup"><span data-stu-id="79734-115">processing</span></span>|<span data-ttu-id="79734-116">1</span><span class="sxs-lookup"><span data-stu-id="79734-116">1</span></span>|<span data-ttu-id="79734-117">アプリケーションは、サービス側の処理を保留中です。</span><span class="sxs-lookup"><span data-stu-id="79734-117">The app is pending service-side processing.</span></span>|
|<span data-ttu-id="79734-118">公開</span><span class="sxs-lookup"><span data-stu-id="79734-118">published</span></span>|<span data-ttu-id="79734-119">2</span><span class="sxs-lookup"><span data-stu-id="79734-119">2</span></span>|<span data-ttu-id="79734-120">アプリケーションが発行されます。</span><span class="sxs-lookup"><span data-stu-id="79734-120">The app is published.</span></span>|





