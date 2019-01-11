---
title: adminConsentState 列挙型
description: 管理者の承認の状態です。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 40f2c30327f7e8af3792c4332fb5605159a28628
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876798"
---
# <a name="adminconsentstate-enum-type"></a><span data-ttu-id="1d194-103">adminConsentState 列挙型</span><span class="sxs-lookup"><span data-stu-id="1d194-103">adminConsentState enum type</span></span>

> <span data-ttu-id="1d194-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1d194-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1d194-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1d194-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1d194-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1d194-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1d194-107">管理者の承認の状態です。</span><span class="sxs-lookup"><span data-stu-id="1d194-107">Admin consent state.</span></span>
## <a name="members"></a><span data-ttu-id="1d194-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="1d194-108">Members</span></span>
|<span data-ttu-id="1d194-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="1d194-109">Member</span></span>|<span data-ttu-id="1d194-110">値</span><span class="sxs-lookup"><span data-stu-id="1d194-110">Value</span></span>|<span data-ttu-id="1d194-111">説明</span><span class="sxs-lookup"><span data-stu-id="1d194-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d194-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="1d194-112">notConfigured</span></span>|<span data-ttu-id="1d194-113">0</span><span class="sxs-lookup"><span data-stu-id="1d194-113">0</span></span>|<span data-ttu-id="1d194-114">管理項目の構成されていません。</span><span class="sxs-lookup"><span data-stu-id="1d194-114">Admin did not configure the item</span></span>|
|<span data-ttu-id="1d194-115">付与</span><span class="sxs-lookup"><span data-stu-id="1d194-115">granted</span></span>|<span data-ttu-id="1d194-116">1</span><span class="sxs-lookup"><span data-stu-id="1d194-116">1</span></span>|<span data-ttu-id="1d194-117">管理の項目を与えられます。</span><span class="sxs-lookup"><span data-stu-id="1d194-117">Admin granted item</span></span>|
|<span data-ttu-id="1d194-118">notGranted</span><span class="sxs-lookup"><span data-stu-id="1d194-118">notGranted</span></span>|<span data-ttu-id="1d194-119">2</span><span class="sxs-lookup"><span data-stu-id="1d194-119">2</span></span>|<span data-ttu-id="1d194-120">Deos の管理項目を付与します。</span><span class="sxs-lookup"><span data-stu-id="1d194-120">Admin deos not grant item</span></span>|





