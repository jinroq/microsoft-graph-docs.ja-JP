---
title: defenderAttackSurfaceType 列挙型
description: Defender 攻撃面の削減ルールで使用できる値
ms.openlocfilehash: 224ff03ce41d459a2bb33dae082bf945beddbfd8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067097"
---
# <a name="defenderattacksurfacetype-enum-type"></a><span data-ttu-id="4f111-103">defenderAttackSurfaceType 列挙型</span><span class="sxs-lookup"><span data-stu-id="4f111-103">defenderAttackSurfaceType enum type</span></span>

> <span data-ttu-id="4f111-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4f111-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4f111-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4f111-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4f111-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4f111-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4f111-107">Defender 攻撃面の削減ルールで使用できる値</span><span class="sxs-lookup"><span data-stu-id="4f111-107">Possible values of Defender Attack Surface Reduction Rules</span></span>
## <a name="members"></a><span data-ttu-id="4f111-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="4f111-108">Members</span></span>
|<span data-ttu-id="4f111-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="4f111-109">Member</span></span>|<span data-ttu-id="4f111-110">値</span><span class="sxs-lookup"><span data-stu-id="4f111-110">Value</span></span>|<span data-ttu-id="4f111-111">説明</span><span class="sxs-lookup"><span data-stu-id="4f111-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f111-112">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="4f111-112">userDefined</span></span>|<span data-ttu-id="4f111-113">0</span><span class="sxs-lookup"><span data-stu-id="4f111-113">0</span></span>|<span data-ttu-id="4f111-114">デバイスの既定値でことを目的しません。</span><span class="sxs-lookup"><span data-stu-id="4f111-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="4f111-115">ブロック</span><span class="sxs-lookup"><span data-stu-id="4f111-115">block</span></span>|<span data-ttu-id="4f111-116">1</span><span class="sxs-lookup"><span data-stu-id="4f111-116">1</span></span>|<span data-ttu-id="4f111-117">機能をブロックします。</span><span class="sxs-lookup"><span data-stu-id="4f111-117">Block functionality.</span></span>|
|<span data-ttu-id="4f111-118">auditMode</span><span class="sxs-lookup"><span data-stu-id="4f111-118">auditMode</span></span>|<span data-ttu-id="4f111-119">2</span><span class="sxs-lookup"><span data-stu-id="4f111-119">2</span></span>|<span data-ttu-id="4f111-120">機能は変更されませんが、ログを生成します。</span><span class="sxs-lookup"><span data-stu-id="4f111-120">Does not change functionality but generate logs.</span></span>|





