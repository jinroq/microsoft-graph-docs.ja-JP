---
title: deviceManagementExchangeAccessLevel 列挙型
description: Exchange のアクセス レベルです。
ms.openlocfilehash: 2d45dab4cecc65fa7514eef178b134da05e466d0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070521"
---
# <a name="devicemanagementexchangeaccesslevel-enum-type"></a><span data-ttu-id="25430-103">deviceManagementExchangeAccessLevel 列挙型</span><span class="sxs-lookup"><span data-stu-id="25430-103">deviceManagementExchangeAccessLevel enum type</span></span>

> <span data-ttu-id="25430-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="25430-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="25430-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="25430-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="25430-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="25430-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="25430-107">Exchange のアクセス レベルです。</span><span class="sxs-lookup"><span data-stu-id="25430-107">Access Level in Exchange.</span></span>
## <a name="members"></a><span data-ttu-id="25430-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="25430-108">Members</span></span>
|<span data-ttu-id="25430-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="25430-109">Member</span></span>|<span data-ttu-id="25430-110">値</span><span class="sxs-lookup"><span data-stu-id="25430-110">Value</span></span>|<span data-ttu-id="25430-111">説明</span><span class="sxs-lookup"><span data-stu-id="25430-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25430-112">none</span><span class="sxs-lookup"><span data-stu-id="25430-112">none</span></span>|<span data-ttu-id="25430-113">0</span><span class="sxs-lookup"><span data-stu-id="25430-113">0</span></span>|<span data-ttu-id="25430-114">Exchange では、デバイス アクセス ルールが構成されていません。</span><span class="sxs-lookup"><span data-stu-id="25430-114">No device access rule has been configured in Exchange.</span></span>|
|<span data-ttu-id="25430-115">許可します。</span><span class="sxs-lookup"><span data-stu-id="25430-115">allow</span></span>|<span data-ttu-id="25430-116">1</span><span class="sxs-lookup"><span data-stu-id="25430-116">1</span></span>|<span data-ttu-id="25430-117">デバイスの Exchange へのアクセスを許可します。</span><span class="sxs-lookup"><span data-stu-id="25430-117">Allow the device access to Exchange.</span></span>|
|<span data-ttu-id="25430-118">ブロック</span><span class="sxs-lookup"><span data-stu-id="25430-118">block</span></span>|<span data-ttu-id="25430-119">2</span><span class="sxs-lookup"><span data-stu-id="25430-119">2</span></span>|<span data-ttu-id="25430-120">デバイスから Exchange へのアクセスをブロックします。</span><span class="sxs-lookup"><span data-stu-id="25430-120">Block the device from accessing Exchange.</span></span>|
|<span data-ttu-id="25430-121">検査</span><span class="sxs-lookup"><span data-stu-id="25430-121">quarantine</span></span>|<span data-ttu-id="25430-122">3</span><span class="sxs-lookup"><span data-stu-id="25430-122">3</span></span>|<span data-ttu-id="25430-123">デバイスを Exchange で隔離します。</span><span class="sxs-lookup"><span data-stu-id="25430-123">Quarantine the device in Exchange.</span></span>|





