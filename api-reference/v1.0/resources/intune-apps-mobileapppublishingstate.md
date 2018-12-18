---
title: mobileAppPublishingState 列挙型
description: アプリケーションの発行状態を示します。
author: tfitzmac
ms.openlocfilehash: c1c89bc67a6f5c9732089b5f85ded77986b16689
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27329555"
---
# <a name="mobileapppublishingstate-enum-type"></a><span data-ttu-id="98015-103">mobileAppPublishingState 列挙型</span><span class="sxs-lookup"><span data-stu-id="98015-103">mobileAppPublishingState enum type</span></span>

> <span data-ttu-id="98015-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="98015-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="98015-105">アプリケーションの発行状態を示します。</span><span class="sxs-lookup"><span data-stu-id="98015-105">Indicates the publishing state of an app.</span></span>
## <a name="members"></a><span data-ttu-id="98015-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="98015-106">Members</span></span>
|<span data-ttu-id="98015-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="98015-107">Member</span></span>|<span data-ttu-id="98015-108">値</span><span class="sxs-lookup"><span data-stu-id="98015-108">Value</span></span>|<span data-ttu-id="98015-109">説明</span><span class="sxs-lookup"><span data-stu-id="98015-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98015-110">notPublished</span><span class="sxs-lookup"><span data-stu-id="98015-110">notPublished</span></span>|<span data-ttu-id="98015-111">0</span><span class="sxs-lookup"><span data-stu-id="98015-111">0</span></span>|<span data-ttu-id="98015-112">アプリケーションはまだ公開されていません。</span><span class="sxs-lookup"><span data-stu-id="98015-112">The app is not yet published.</span></span>|
|<span data-ttu-id="98015-113">処理</span><span class="sxs-lookup"><span data-stu-id="98015-113">processing</span></span>|<span data-ttu-id="98015-114">1</span><span class="sxs-lookup"><span data-stu-id="98015-114">1</span></span>|<span data-ttu-id="98015-115">アプリケーションは、サービス側の処理を保留中です。</span><span class="sxs-lookup"><span data-stu-id="98015-115">The app is pending service-side processing.</span></span>|
|<span data-ttu-id="98015-116">公開</span><span class="sxs-lookup"><span data-stu-id="98015-116">published</span></span>|<span data-ttu-id="98015-117">2</span><span class="sxs-lookup"><span data-stu-id="98015-117">2</span></span>|<span data-ttu-id="98015-118">アプリケーションが発行されます。</span><span class="sxs-lookup"><span data-stu-id="98015-118">The app is published.</span></span>|



