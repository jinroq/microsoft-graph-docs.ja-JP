---
title: mobileAppPublishingState 列挙型
description: アプリケーションの発行状態を示します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 270dd416422c0f0b4dfc320937c749f4fe13c766
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937762"
---
# <a name="mobileapppublishingstate-enum-type"></a><span data-ttu-id="f7399-103">mobileAppPublishingState 列挙型</span><span class="sxs-lookup"><span data-stu-id="f7399-103">mobileAppPublishingState enum type</span></span>

> <span data-ttu-id="f7399-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f7399-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f7399-105">アプリケーションの発行状態を示します。</span><span class="sxs-lookup"><span data-stu-id="f7399-105">Indicates the publishing state of an app.</span></span>
## <a name="members"></a><span data-ttu-id="f7399-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="f7399-106">Members</span></span>
|<span data-ttu-id="f7399-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="f7399-107">Member</span></span>|<span data-ttu-id="f7399-108">値</span><span class="sxs-lookup"><span data-stu-id="f7399-108">Value</span></span>|<span data-ttu-id="f7399-109">説明</span><span class="sxs-lookup"><span data-stu-id="f7399-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7399-110">notPublished</span><span class="sxs-lookup"><span data-stu-id="f7399-110">notPublished</span></span>|<span data-ttu-id="f7399-111">0</span><span class="sxs-lookup"><span data-stu-id="f7399-111">0</span></span>|<span data-ttu-id="f7399-112">アプリケーションはまだ公開されていません。</span><span class="sxs-lookup"><span data-stu-id="f7399-112">The app is not yet published.</span></span>|
|<span data-ttu-id="f7399-113">処理</span><span class="sxs-lookup"><span data-stu-id="f7399-113">processing</span></span>|<span data-ttu-id="f7399-114">1</span><span class="sxs-lookup"><span data-stu-id="f7399-114">1</span></span>|<span data-ttu-id="f7399-115">アプリケーションは、サービス側の処理を保留中です。</span><span class="sxs-lookup"><span data-stu-id="f7399-115">The app is pending service-side processing.</span></span>|
|<span data-ttu-id="f7399-116">公開</span><span class="sxs-lookup"><span data-stu-id="f7399-116">published</span></span>|<span data-ttu-id="f7399-117">2</span><span class="sxs-lookup"><span data-stu-id="f7399-117">2</span></span>|<span data-ttu-id="f7399-118">アプリケーションが発行されます。</span><span class="sxs-lookup"><span data-stu-id="f7399-118">The app is published.</span></span>|



