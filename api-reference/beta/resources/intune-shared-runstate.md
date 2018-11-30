---
title: runState 列挙型
description: デバイスの管理スクリプトの実行ステータスの種類を示します。
ms.openlocfilehash: 74802b347d83db0785c5c132315071024d944ddc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066258"
---
# <a name="runstate-enum-type"></a><span data-ttu-id="44d17-103">runState 列挙型</span><span class="sxs-lookup"><span data-stu-id="44d17-103">runState enum type</span></span>

> <span data-ttu-id="44d17-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="44d17-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="44d17-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="44d17-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="44d17-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="44d17-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="44d17-107">デバイスの管理スクリプトの実行ステータスの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="44d17-107">Indicates the type of execution status of the device management script.</span></span>
## <a name="members"></a><span data-ttu-id="44d17-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="44d17-108">Members</span></span>
|<span data-ttu-id="44d17-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="44d17-109">Member</span></span>|<span data-ttu-id="44d17-110">値</span><span class="sxs-lookup"><span data-stu-id="44d17-110">Value</span></span>|<span data-ttu-id="44d17-111">説明</span><span class="sxs-lookup"><span data-stu-id="44d17-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44d17-112">不明</span><span class="sxs-lookup"><span data-stu-id="44d17-112">unknown</span></span>|<span data-ttu-id="44d17-113">0</span><span class="sxs-lookup"><span data-stu-id="44d17-113">0</span></span>|<span data-ttu-id="44d17-114">不明な結果です。</span><span class="sxs-lookup"><span data-stu-id="44d17-114">Unknown result.</span></span>|
|<span data-ttu-id="44d17-115">success</span><span class="sxs-lookup"><span data-stu-id="44d17-115">success</span></span>|<span data-ttu-id="44d17-116">1</span><span class="sxs-lookup"><span data-stu-id="44d17-116">1</span></span>|<span data-ttu-id="44d17-117">スクリプトが正常に実行します。</span><span class="sxs-lookup"><span data-stu-id="44d17-117">Script is run successfully.</span></span>|
|<span data-ttu-id="44d17-118">失敗します。</span><span class="sxs-lookup"><span data-stu-id="44d17-118">fail</span></span>|<span data-ttu-id="44d17-119">2</span><span class="sxs-lookup"><span data-stu-id="44d17-119">2</span></span>|<span data-ttu-id="44d17-120">スクリプトを実行できませんでした。</span><span class="sxs-lookup"><span data-stu-id="44d17-120">Script failed to run.</span></span>|





