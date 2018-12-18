---
title: runState 列挙型
description: デバイスの管理スクリプトの実行ステータスの種類を示します。
author: tfitzmac
ms.openlocfilehash: 87c845c02bd5a1571ab2f6382acbcc92cf81170d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349274"
---
# <a name="runstate-enum-type"></a><span data-ttu-id="e3415-103">runState 列挙型</span><span class="sxs-lookup"><span data-stu-id="e3415-103">runState enum type</span></span>

> <span data-ttu-id="e3415-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e3415-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e3415-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e3415-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e3415-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e3415-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e3415-107">デバイスの管理スクリプトの実行ステータスの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="e3415-107">Indicates the type of execution status of the device management script.</span></span>
## <a name="members"></a><span data-ttu-id="e3415-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="e3415-108">Members</span></span>
|<span data-ttu-id="e3415-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="e3415-109">Member</span></span>|<span data-ttu-id="e3415-110">値</span><span class="sxs-lookup"><span data-stu-id="e3415-110">Value</span></span>|<span data-ttu-id="e3415-111">説明</span><span class="sxs-lookup"><span data-stu-id="e3415-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3415-112">不明</span><span class="sxs-lookup"><span data-stu-id="e3415-112">unknown</span></span>|<span data-ttu-id="e3415-113">0</span><span class="sxs-lookup"><span data-stu-id="e3415-113">0</span></span>|<span data-ttu-id="e3415-114">不明な結果です。</span><span class="sxs-lookup"><span data-stu-id="e3415-114">Unknown result.</span></span>|
|<span data-ttu-id="e3415-115">success</span><span class="sxs-lookup"><span data-stu-id="e3415-115">success</span></span>|<span data-ttu-id="e3415-116">1</span><span class="sxs-lookup"><span data-stu-id="e3415-116">1</span></span>|<span data-ttu-id="e3415-117">スクリプトが正常に実行します。</span><span class="sxs-lookup"><span data-stu-id="e3415-117">Script is run successfully.</span></span>|
|<span data-ttu-id="e3415-118">失敗します。</span><span class="sxs-lookup"><span data-stu-id="e3415-118">fail</span></span>|<span data-ttu-id="e3415-119">2</span><span class="sxs-lookup"><span data-stu-id="e3415-119">2</span></span>|<span data-ttu-id="e3415-120">スクリプトを実行できませんでした。</span><span class="sxs-lookup"><span data-stu-id="e3415-120">Script failed to run.</span></span>|





