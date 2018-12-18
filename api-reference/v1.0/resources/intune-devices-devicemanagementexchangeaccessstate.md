---
title: deviceManagementExchangeAccessState 列挙型
description: デバイスの Exchange のアクセスの状態です。
author: tfitzmac
ms.openlocfilehash: 37db054314375411dc237746ca6ca3bdb99e9016
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328722"
---
# <a name="devicemanagementexchangeaccessstate-enum-type"></a><span data-ttu-id="f7063-103">deviceManagementExchangeAccessState 列挙型</span><span class="sxs-lookup"><span data-stu-id="f7063-103">deviceManagementExchangeAccessState enum type</span></span>

> <span data-ttu-id="f7063-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f7063-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f7063-105">デバイスの Exchange のアクセスの状態です。</span><span class="sxs-lookup"><span data-stu-id="f7063-105">Device Exchange Access State.</span></span>
## <a name="members"></a><span data-ttu-id="f7063-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="f7063-106">Members</span></span>
|<span data-ttu-id="f7063-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="f7063-107">Member</span></span>|<span data-ttu-id="f7063-108">値</span><span class="sxs-lookup"><span data-stu-id="f7063-108">Value</span></span>|<span data-ttu-id="f7063-109">説明</span><span class="sxs-lookup"><span data-stu-id="f7063-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7063-110">none</span><span class="sxs-lookup"><span data-stu-id="f7063-110">none</span></span>|<span data-ttu-id="f7063-111">0</span><span class="sxs-lookup"><span data-stu-id="f7063-111">0</span></span>|<span data-ttu-id="f7063-112">Exchange から検出アクセス状態がないです。</span><span class="sxs-lookup"><span data-stu-id="f7063-112">No access state discovered from Exchange</span></span>|
|<span data-ttu-id="f7063-113">不明</span><span class="sxs-lookup"><span data-stu-id="f7063-113">unknown</span></span>|<span data-ttu-id="f7063-114">1</span><span class="sxs-lookup"><span data-stu-id="f7063-114">1</span></span>|<span data-ttu-id="f7063-115">Exchange へのデバイスのアクセス状態は不明です。</span><span class="sxs-lookup"><span data-stu-id="f7063-115">Device access state to Exchange is unknown</span></span>|
|<span data-ttu-id="f7063-116">許可</span><span class="sxs-lookup"><span data-stu-id="f7063-116">allowed</span></span>|<span data-ttu-id="f7063-117">2</span><span class="sxs-lookup"><span data-stu-id="f7063-117">2</span></span>|<span data-ttu-id="f7063-118">デバイスが Exchange へのアクセス権を持つ</span><span class="sxs-lookup"><span data-stu-id="f7063-118">Device has access to Exchange</span></span>|
|<span data-ttu-id="f7063-119">ブロック</span><span class="sxs-lookup"><span data-stu-id="f7063-119">blocked</span></span>|<span data-ttu-id="f7063-120">3</span><span class="sxs-lookup"><span data-stu-id="f7063-120">3</span></span>|<span data-ttu-id="f7063-121">デバイスが Exchange でブロックされています。</span><span class="sxs-lookup"><span data-stu-id="f7063-121">Device is Blocked in Exchange</span></span>|
|<span data-ttu-id="f7063-122">検疫</span><span class="sxs-lookup"><span data-stu-id="f7063-122">quarantined</span></span>|<span data-ttu-id="f7063-123">4</span><span class="sxs-lookup"><span data-stu-id="f7063-123">4</span></span>|<span data-ttu-id="f7063-124">デバイスが Exchange の検疫します。</span><span class="sxs-lookup"><span data-stu-id="f7063-124">Device is Quarantined in Exchange</span></span>|



