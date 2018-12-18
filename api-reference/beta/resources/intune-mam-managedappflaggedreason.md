---
title: managedAppFlaggedReason 列挙型
description: ユーザーが設定されている理由
author: tfitzmac
ms.openlocfilehash: 395cd446863b88fade45c7160302cd05132f1d52
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27358423"
---
# <a name="managedappflaggedreason-enum-type"></a><span data-ttu-id="96d6e-103">managedAppFlaggedReason 列挙型</span><span class="sxs-lookup"><span data-stu-id="96d6e-103">managedAppFlaggedReason enum type</span></span>

> <span data-ttu-id="96d6e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="96d6e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="96d6e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="96d6e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="96d6e-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="96d6e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="96d6e-107">ユーザーが設定されている理由</span><span class="sxs-lookup"><span data-stu-id="96d6e-107">The reason for which a user has been flagged</span></span>
## <a name="members"></a><span data-ttu-id="96d6e-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="96d6e-108">Members</span></span>
|<span data-ttu-id="96d6e-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="96d6e-109">Member</span></span>|<span data-ttu-id="96d6e-110">値</span><span class="sxs-lookup"><span data-stu-id="96d6e-110">Value</span></span>|<span data-ttu-id="96d6e-111">説明</span><span class="sxs-lookup"><span data-stu-id="96d6e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96d6e-112">none</span><span class="sxs-lookup"><span data-stu-id="96d6e-112">none</span></span>|<span data-ttu-id="96d6e-113">0</span><span class="sxs-lookup"><span data-stu-id="96d6e-113">0</span></span>|<span data-ttu-id="96d6e-114">問題はありません。</span><span class="sxs-lookup"><span data-stu-id="96d6e-114">No issue.</span></span>|
|<span data-ttu-id="96d6e-115">rootedDevice</span><span class="sxs-lookup"><span data-stu-id="96d6e-115">rootedDevice</span></span>|<span data-ttu-id="96d6e-116">1</span><span class="sxs-lookup"><span data-stu-id="96d6e-116">1</span></span>|<span data-ttu-id="96d6e-117">ルートとロック解除のデバイスでアプリケーションの登録が行われています。</span><span class="sxs-lookup"><span data-stu-id="96d6e-117">The app registration is running on a rooted/unlocked device.</span></span>|





