---
title: managedAppFlaggedReason 列挙型
description: ユーザーが設定されている理由
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 15c4041b4511ab71ac16520297d5c8bb3e63b4e3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888040"
---
# <a name="managedappflaggedreason-enum-type"></a><span data-ttu-id="fad8a-103">managedAppFlaggedReason 列挙型</span><span class="sxs-lookup"><span data-stu-id="fad8a-103">managedAppFlaggedReason enum type</span></span>

> <span data-ttu-id="fad8a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fad8a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fad8a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fad8a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fad8a-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="fad8a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fad8a-107">ユーザーが設定されている理由</span><span class="sxs-lookup"><span data-stu-id="fad8a-107">The reason for which a user has been flagged</span></span>
## <a name="members"></a><span data-ttu-id="fad8a-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="fad8a-108">Members</span></span>
|<span data-ttu-id="fad8a-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="fad8a-109">Member</span></span>|<span data-ttu-id="fad8a-110">値</span><span class="sxs-lookup"><span data-stu-id="fad8a-110">Value</span></span>|<span data-ttu-id="fad8a-111">説明</span><span class="sxs-lookup"><span data-stu-id="fad8a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fad8a-112">none</span><span class="sxs-lookup"><span data-stu-id="fad8a-112">none</span></span>|<span data-ttu-id="fad8a-113">0</span><span class="sxs-lookup"><span data-stu-id="fad8a-113">0</span></span>|<span data-ttu-id="fad8a-114">問題はありません。</span><span class="sxs-lookup"><span data-stu-id="fad8a-114">No issue.</span></span>|
|<span data-ttu-id="fad8a-115">rootedDevice</span><span class="sxs-lookup"><span data-stu-id="fad8a-115">rootedDevice</span></span>|<span data-ttu-id="fad8a-116">1</span><span class="sxs-lookup"><span data-stu-id="fad8a-116">1</span></span>|<span data-ttu-id="fad8a-117">ルートとロック解除のデバイスでアプリケーションの登録が行われています。</span><span class="sxs-lookup"><span data-stu-id="fad8a-117">The app registration is running on a rooted/unlocked device.</span></span>|





