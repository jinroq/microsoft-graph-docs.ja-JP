---
title: defenderAttackSurfaceType 列挙型
description: Defender 攻撃面の削減ルールで使用できる値
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3535169fde0206ee2a441551f1816b20f6caf7de
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924259"
---
# <a name="defenderattacksurfacetype-enum-type"></a><span data-ttu-id="086ed-103">defenderAttackSurfaceType 列挙型</span><span class="sxs-lookup"><span data-stu-id="086ed-103">defenderAttackSurfaceType enum type</span></span>

> <span data-ttu-id="086ed-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="086ed-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="086ed-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="086ed-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="086ed-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="086ed-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="086ed-107">Defender 攻撃面の削減ルールで使用できる値</span><span class="sxs-lookup"><span data-stu-id="086ed-107">Possible values of Defender Attack Surface Reduction Rules</span></span>
## <a name="members"></a><span data-ttu-id="086ed-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="086ed-108">Members</span></span>
|<span data-ttu-id="086ed-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="086ed-109">Member</span></span>|<span data-ttu-id="086ed-110">値</span><span class="sxs-lookup"><span data-stu-id="086ed-110">Value</span></span>|<span data-ttu-id="086ed-111">説明</span><span class="sxs-lookup"><span data-stu-id="086ed-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="086ed-112">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="086ed-112">userDefined</span></span>|<span data-ttu-id="086ed-113">0</span><span class="sxs-lookup"><span data-stu-id="086ed-113">0</span></span>|<span data-ttu-id="086ed-114">デバイスの既定値でことを目的しません。</span><span class="sxs-lookup"><span data-stu-id="086ed-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="086ed-115">ブロック</span><span class="sxs-lookup"><span data-stu-id="086ed-115">block</span></span>|<span data-ttu-id="086ed-116">1</span><span class="sxs-lookup"><span data-stu-id="086ed-116">1</span></span>|<span data-ttu-id="086ed-117">機能をブロックします。</span><span class="sxs-lookup"><span data-stu-id="086ed-117">Block functionality.</span></span>|
|<span data-ttu-id="086ed-118">auditMode</span><span class="sxs-lookup"><span data-stu-id="086ed-118">auditMode</span></span>|<span data-ttu-id="086ed-119">2</span><span class="sxs-lookup"><span data-stu-id="086ed-119">2</span></span>|<span data-ttu-id="086ed-120">機能は変更されませんが、ログを生成します。</span><span class="sxs-lookup"><span data-stu-id="086ed-120">Does not change functionality but generate logs.</span></span>|





