---
title: vppTokenSyncStatus 列挙型
description: Apple ボリューム購入プログラム、トークンに関連付けられている可能性のある同期のステータス。
ms.openlocfilehash: 443eb87299fbb052edf8788d07b029c68d58c2fe
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072614"
---
# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="8ba97-103">vppTokenSyncStatus 列挙型</span><span class="sxs-lookup"><span data-stu-id="8ba97-103">vppTokenSyncStatus enum type</span></span>

> <span data-ttu-id="8ba97-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8ba97-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8ba97-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8ba97-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8ba97-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8ba97-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8ba97-107">Apple ボリューム購入プログラム、トークンに関連付けられている可能性のある同期のステータス。</span><span class="sxs-lookup"><span data-stu-id="8ba97-107">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>
## <a name="members"></a><span data-ttu-id="8ba97-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="8ba97-108">Members</span></span>
|<span data-ttu-id="8ba97-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="8ba97-109">Member</span></span>|<span data-ttu-id="8ba97-110">値</span><span class="sxs-lookup"><span data-stu-id="8ba97-110">Value</span></span>|<span data-ttu-id="8ba97-111">説明</span><span class="sxs-lookup"><span data-stu-id="8ba97-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ba97-112">none</span><span class="sxs-lookup"><span data-stu-id="8ba97-112">none</span></span>|<span data-ttu-id="8ba97-113">0</span><span class="sxs-lookup"><span data-stu-id="8ba97-113">0</span></span>|<span data-ttu-id="8ba97-114">既定の状態です。</span><span class="sxs-lookup"><span data-stu-id="8ba97-114">Default status.</span></span>|
|<span data-ttu-id="8ba97-115">inProgress</span><span class="sxs-lookup"><span data-stu-id="8ba97-115">inProgress</span></span>|<span data-ttu-id="8ba97-116">1</span><span class="sxs-lookup"><span data-stu-id="8ba97-116">1</span></span>|<span data-ttu-id="8ba97-117">進行中の最後の同期します。</span><span class="sxs-lookup"><span data-stu-id="8ba97-117">Last Sync in progress.</span></span>|
|<span data-ttu-id="8ba97-118">完了</span><span class="sxs-lookup"><span data-stu-id="8ba97-118">completed</span></span>|<span data-ttu-id="8ba97-119">2</span><span class="sxs-lookup"><span data-stu-id="8ba97-119">2</span></span>|<span data-ttu-id="8ba97-120">前回の同期が正常に完了しました。</span><span class="sxs-lookup"><span data-stu-id="8ba97-120">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="8ba97-121">失敗しました。</span><span class="sxs-lookup"><span data-stu-id="8ba97-121">failed</span></span>|<span data-ttu-id="8ba97-122">3</span><span class="sxs-lookup"><span data-stu-id="8ba97-122">3</span></span>|<span data-ttu-id="8ba97-123">前回の同期が失敗しました。</span><span class="sxs-lookup"><span data-stu-id="8ba97-123">Last Sync failed.</span></span>|





