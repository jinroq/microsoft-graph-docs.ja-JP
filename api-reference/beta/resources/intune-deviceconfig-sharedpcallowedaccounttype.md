---
title: sharedPCAllowedAccountType 列挙型
description: PC の共有を許可するアカウントの種類です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ed359399acc1b83c338e509ec3ea35623e0ce9c5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27969416"
---
# <a name="sharedpcallowedaccounttype-enum-type"></a><span data-ttu-id="576eb-103">sharedPCAllowedAccountType 列挙型</span><span class="sxs-lookup"><span data-stu-id="576eb-103">sharedPCAllowedAccountType enum type</span></span>

> <span data-ttu-id="576eb-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="576eb-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="576eb-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="576eb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="576eb-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="576eb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="576eb-107">PC の共有を許可するアカウントの種類です。</span><span class="sxs-lookup"><span data-stu-id="576eb-107">Type of accounts that are allowed to share the PC.</span></span>
## <a name="members"></a><span data-ttu-id="576eb-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="576eb-108">Members</span></span>
|<span data-ttu-id="576eb-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="576eb-109">Member</span></span>|<span data-ttu-id="576eb-110">値</span><span class="sxs-lookup"><span data-stu-id="576eb-110">Value</span></span>|<span data-ttu-id="576eb-111">説明</span><span class="sxs-lookup"><span data-stu-id="576eb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="576eb-112">ゲスト</span><span class="sxs-lookup"><span data-stu-id="576eb-112">guest</span></span>|<span data-ttu-id="576eb-113">1</span><span class="sxs-lookup"><span data-stu-id="576eb-113">1</span></span>|<span data-ttu-id="576eb-114">Guest アカウントだけです。</span><span class="sxs-lookup"><span data-stu-id="576eb-114">Only guest accounts.</span></span> <span data-ttu-id="576eb-115">既定値です。</span><span class="sxs-lookup"><span data-stu-id="576eb-115">Default value.</span></span>|
|<span data-ttu-id="576eb-116">domain</span><span class="sxs-lookup"><span data-stu-id="576eb-116">domain</span></span>|<span data-ttu-id="576eb-117">2</span><span class="sxs-lookup"><span data-stu-id="576eb-117">2</span></span>|<span data-ttu-id="576eb-118">ドメインに参加しているアカウントだけです。</span><span class="sxs-lookup"><span data-stu-id="576eb-118">Only domain-joined accounts.</span></span>|





