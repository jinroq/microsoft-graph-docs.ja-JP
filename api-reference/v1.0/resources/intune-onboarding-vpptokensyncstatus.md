---
title: vppTokenSyncStatus 列挙型
description: Apple ボリューム購入プログラム、トークンに関連付けられている可能性のある同期のステータス。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: db458423a00fd7b38bddea1b1954cda1ec6ec83b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888684"
---
# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="9d697-103">vppTokenSyncStatus 列挙型</span><span class="sxs-lookup"><span data-stu-id="9d697-103">vppTokenSyncStatus enum type</span></span>

> <span data-ttu-id="9d697-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9d697-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9d697-105">Apple ボリューム購入プログラム、トークンに関連付けられている可能性のある同期のステータス。</span><span class="sxs-lookup"><span data-stu-id="9d697-105">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>
## <a name="members"></a><span data-ttu-id="9d697-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="9d697-106">Members</span></span>
|<span data-ttu-id="9d697-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="9d697-107">Member</span></span>|<span data-ttu-id="9d697-108">値</span><span class="sxs-lookup"><span data-stu-id="9d697-108">Value</span></span>|<span data-ttu-id="9d697-109">説明</span><span class="sxs-lookup"><span data-stu-id="9d697-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d697-110">none</span><span class="sxs-lookup"><span data-stu-id="9d697-110">none</span></span>|<span data-ttu-id="9d697-111">0</span><span class="sxs-lookup"><span data-stu-id="9d697-111">0</span></span>|<span data-ttu-id="9d697-112">既定の状態です。</span><span class="sxs-lookup"><span data-stu-id="9d697-112">Default status.</span></span>|
|<span data-ttu-id="9d697-113">inProgress</span><span class="sxs-lookup"><span data-stu-id="9d697-113">inProgress</span></span>|<span data-ttu-id="9d697-114">1</span><span class="sxs-lookup"><span data-stu-id="9d697-114">1</span></span>|<span data-ttu-id="9d697-115">進行中の最後の同期します。</span><span class="sxs-lookup"><span data-stu-id="9d697-115">Last Sync in progress.</span></span>|
|<span data-ttu-id="9d697-116">完了</span><span class="sxs-lookup"><span data-stu-id="9d697-116">completed</span></span>|<span data-ttu-id="9d697-117">2</span><span class="sxs-lookup"><span data-stu-id="9d697-117">2</span></span>|<span data-ttu-id="9d697-118">前回の同期が正常に完了しました。</span><span class="sxs-lookup"><span data-stu-id="9d697-118">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="9d697-119">失敗しました。</span><span class="sxs-lookup"><span data-stu-id="9d697-119">failed</span></span>|<span data-ttu-id="9d697-120">3</span><span class="sxs-lookup"><span data-stu-id="9d697-120">3</span></span>|<span data-ttu-id="9d697-121">前回の同期が失敗しました。</span><span class="sxs-lookup"><span data-stu-id="9d697-121">Last Sync failed.</span></span>|



