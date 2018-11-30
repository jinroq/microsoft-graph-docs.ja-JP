---
title: vppTokenSyncStatus 列挙型
description: Apple ボリューム購入プログラム、トークンに関連付けられている可能性のある同期のステータス。
ms.openlocfilehash: e038f15a3c58928ebb066c0fbf5aac320bf574a9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022829"
---
# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="35d10-103">vppTokenSyncStatus 列挙型</span><span class="sxs-lookup"><span data-stu-id="35d10-103">vppTokenSyncStatus enum type</span></span>

> <span data-ttu-id="35d10-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="35d10-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="35d10-105">Apple ボリューム購入プログラム、トークンに関連付けられている可能性のある同期のステータス。</span><span class="sxs-lookup"><span data-stu-id="35d10-105">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>
## <a name="members"></a><span data-ttu-id="35d10-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="35d10-106">Members</span></span>
|<span data-ttu-id="35d10-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="35d10-107">Member</span></span>|<span data-ttu-id="35d10-108">値</span><span class="sxs-lookup"><span data-stu-id="35d10-108">Value</span></span>|<span data-ttu-id="35d10-109">説明</span><span class="sxs-lookup"><span data-stu-id="35d10-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35d10-110">none</span><span class="sxs-lookup"><span data-stu-id="35d10-110">none</span></span>|<span data-ttu-id="35d10-111">0</span><span class="sxs-lookup"><span data-stu-id="35d10-111">0</span></span>|<span data-ttu-id="35d10-112">既定の状態です。</span><span class="sxs-lookup"><span data-stu-id="35d10-112">Default status.</span></span>|
|<span data-ttu-id="35d10-113">inProgress</span><span class="sxs-lookup"><span data-stu-id="35d10-113">inProgress</span></span>|<span data-ttu-id="35d10-114">1</span><span class="sxs-lookup"><span data-stu-id="35d10-114">1</span></span>|<span data-ttu-id="35d10-115">進行中の最後の同期します。</span><span class="sxs-lookup"><span data-stu-id="35d10-115">Last Sync in progress.</span></span>|
|<span data-ttu-id="35d10-116">完了</span><span class="sxs-lookup"><span data-stu-id="35d10-116">completed</span></span>|<span data-ttu-id="35d10-117">2</span><span class="sxs-lookup"><span data-stu-id="35d10-117">2</span></span>|<span data-ttu-id="35d10-118">前回の同期が正常に完了しました。</span><span class="sxs-lookup"><span data-stu-id="35d10-118">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="35d10-119">失敗しました。</span><span class="sxs-lookup"><span data-stu-id="35d10-119">failed</span></span>|<span data-ttu-id="35d10-120">3</span><span class="sxs-lookup"><span data-stu-id="35d10-120">3</span></span>|<span data-ttu-id="35d10-121">前回の同期が失敗しました。</span><span class="sxs-lookup"><span data-stu-id="35d10-121">Last Sync failed.</span></span>|



