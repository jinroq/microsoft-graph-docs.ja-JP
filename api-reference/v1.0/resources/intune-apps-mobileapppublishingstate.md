---
title: mobileAppPublishingState 列挙型
description: アプリケーションの発行状態を示します。
ms.openlocfilehash: 458c38f6e53bc5590d4414d8c288cdd88739bcc1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023093"
---
# <a name="mobileapppublishingstate-enum-type"></a><span data-ttu-id="6b33e-103">mobileAppPublishingState 列挙型</span><span class="sxs-lookup"><span data-stu-id="6b33e-103">mobileAppPublishingState enum type</span></span>

> <span data-ttu-id="6b33e-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6b33e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6b33e-105">アプリケーションの発行状態を示します。</span><span class="sxs-lookup"><span data-stu-id="6b33e-105">Indicates the publishing state of an app.</span></span>
## <a name="members"></a><span data-ttu-id="6b33e-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="6b33e-106">Members</span></span>
|<span data-ttu-id="6b33e-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="6b33e-107">Member</span></span>|<span data-ttu-id="6b33e-108">値</span><span class="sxs-lookup"><span data-stu-id="6b33e-108">Value</span></span>|<span data-ttu-id="6b33e-109">説明</span><span class="sxs-lookup"><span data-stu-id="6b33e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b33e-110">notPublished</span><span class="sxs-lookup"><span data-stu-id="6b33e-110">notPublished</span></span>|<span data-ttu-id="6b33e-111">0</span><span class="sxs-lookup"><span data-stu-id="6b33e-111">0</span></span>|<span data-ttu-id="6b33e-112">アプリケーションはまだ公開されていません。</span><span class="sxs-lookup"><span data-stu-id="6b33e-112">The app is not yet published.</span></span>|
|<span data-ttu-id="6b33e-113">処理</span><span class="sxs-lookup"><span data-stu-id="6b33e-113">processing</span></span>|<span data-ttu-id="6b33e-114">1</span><span class="sxs-lookup"><span data-stu-id="6b33e-114">1</span></span>|<span data-ttu-id="6b33e-115">アプリケーションは、サービス側の処理を保留中です。</span><span class="sxs-lookup"><span data-stu-id="6b33e-115">The app is pending service-side processing.</span></span>|
|<span data-ttu-id="6b33e-116">公開</span><span class="sxs-lookup"><span data-stu-id="6b33e-116">published</span></span>|<span data-ttu-id="6b33e-117">2</span><span class="sxs-lookup"><span data-stu-id="6b33e-117">2</span></span>|<span data-ttu-id="6b33e-118">アプリケーションが発行されます。</span><span class="sxs-lookup"><span data-stu-id="6b33e-118">The app is published.</span></span>|



