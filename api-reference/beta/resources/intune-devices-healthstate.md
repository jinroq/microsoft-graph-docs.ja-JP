---
title: healthState 列挙型
description: Windows 管理アプリケーションの稼働状態を示します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 4b50023a71aaf33e2febf43e3ce96a1223eaa2ed
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878779"
---
# <a name="healthstate-enum-type"></a><span data-ttu-id="81176-103">healthState 列挙型</span><span class="sxs-lookup"><span data-stu-id="81176-103">healthState enum type</span></span>

> <span data-ttu-id="81176-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="81176-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="81176-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="81176-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="81176-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="81176-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="81176-107">Windows 管理アプリケーションの稼働状態を示します。</span><span class="sxs-lookup"><span data-stu-id="81176-107">Indicates health state of the Windows management app.</span></span>
## <a name="members"></a><span data-ttu-id="81176-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="81176-108">Members</span></span>
|<span data-ttu-id="81176-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="81176-109">Member</span></span>|<span data-ttu-id="81176-110">値</span><span class="sxs-lookup"><span data-stu-id="81176-110">Value</span></span>|<span data-ttu-id="81176-111">説明</span><span class="sxs-lookup"><span data-stu-id="81176-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81176-112">不明</span><span class="sxs-lookup"><span data-stu-id="81176-112">unknown</span></span>|<span data-ttu-id="81176-113">0</span><span class="sxs-lookup"><span data-stu-id="81176-113">0</span></span>|<span data-ttu-id="81176-114">不明な状態です。</span><span class="sxs-lookup"><span data-stu-id="81176-114">Unknown state.</span></span>|
|<span data-ttu-id="81176-115">正常な状態</span><span class="sxs-lookup"><span data-stu-id="81176-115">healthy</span></span>|<span data-ttu-id="81176-116">1</span><span class="sxs-lookup"><span data-stu-id="81176-116">1</span></span>|<span data-ttu-id="81176-117">正常な状態です。</span><span class="sxs-lookup"><span data-stu-id="81176-117">Healthy state.</span></span>|
|<span data-ttu-id="81176-118">問題があります。</span><span class="sxs-lookup"><span data-stu-id="81176-118">unhealthy</span></span>|<span data-ttu-id="81176-119">2</span><span class="sxs-lookup"><span data-stu-id="81176-119">2</span></span>|<span data-ttu-id="81176-120">異常な状態です。</span><span class="sxs-lookup"><span data-stu-id="81176-120">Unhealthy state.</span></span>|





