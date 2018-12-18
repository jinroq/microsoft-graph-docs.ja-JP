---
title: vppTokenSyncStatus 列挙型
description: Apple ボリューム購入プログラム、トークンに関連付けられている可能性のある同期のステータス。
author: tfitzmac
ms.openlocfilehash: 18a0fcf9f4d22d7904cb76d1fc45d80b14dfc7d9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344241"
---
# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="11354-103">vppTokenSyncStatus 列挙型</span><span class="sxs-lookup"><span data-stu-id="11354-103">vppTokenSyncStatus enum type</span></span>

> <span data-ttu-id="11354-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="11354-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="11354-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="11354-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="11354-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="11354-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="11354-107">Apple ボリューム購入プログラム、トークンに関連付けられている可能性のある同期のステータス。</span><span class="sxs-lookup"><span data-stu-id="11354-107">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>
## <a name="members"></a><span data-ttu-id="11354-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="11354-108">Members</span></span>
|<span data-ttu-id="11354-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="11354-109">Member</span></span>|<span data-ttu-id="11354-110">値</span><span class="sxs-lookup"><span data-stu-id="11354-110">Value</span></span>|<span data-ttu-id="11354-111">説明</span><span class="sxs-lookup"><span data-stu-id="11354-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11354-112">none</span><span class="sxs-lookup"><span data-stu-id="11354-112">none</span></span>|<span data-ttu-id="11354-113">0</span><span class="sxs-lookup"><span data-stu-id="11354-113">0</span></span>|<span data-ttu-id="11354-114">既定の状態です。</span><span class="sxs-lookup"><span data-stu-id="11354-114">Default status.</span></span>|
|<span data-ttu-id="11354-115">inProgress</span><span class="sxs-lookup"><span data-stu-id="11354-115">inProgress</span></span>|<span data-ttu-id="11354-116">1</span><span class="sxs-lookup"><span data-stu-id="11354-116">1</span></span>|<span data-ttu-id="11354-117">進行中の最後の同期します。</span><span class="sxs-lookup"><span data-stu-id="11354-117">Last Sync in progress.</span></span>|
|<span data-ttu-id="11354-118">完了</span><span class="sxs-lookup"><span data-stu-id="11354-118">completed</span></span>|<span data-ttu-id="11354-119">2</span><span class="sxs-lookup"><span data-stu-id="11354-119">2</span></span>|<span data-ttu-id="11354-120">前回の同期が正常に完了しました。</span><span class="sxs-lookup"><span data-stu-id="11354-120">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="11354-121">失敗しました。</span><span class="sxs-lookup"><span data-stu-id="11354-121">failed</span></span>|<span data-ttu-id="11354-122">3</span><span class="sxs-lookup"><span data-stu-id="11354-122">3</span></span>|<span data-ttu-id="11354-123">前回の同期が失敗しました。</span><span class="sxs-lookup"><span data-stu-id="11354-123">Last Sync failed.</span></span>|





