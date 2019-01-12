---
title: managedAppFlaggedReason 列挙型
description: ユーザーが設定されている理由
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: dc4749a1a5b121362c34499511b7e207fb2c4e1e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27961800"
---
# <a name="managedappflaggedreason-enum-type"></a><span data-ttu-id="99d31-103">managedAppFlaggedReason 列挙型</span><span class="sxs-lookup"><span data-stu-id="99d31-103">managedAppFlaggedReason enum type</span></span>

> <span data-ttu-id="99d31-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="99d31-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="99d31-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="99d31-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="99d31-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="99d31-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="99d31-107">ユーザーが設定されている理由</span><span class="sxs-lookup"><span data-stu-id="99d31-107">The reason for which a user has been flagged</span></span>
## <a name="members"></a><span data-ttu-id="99d31-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="99d31-108">Members</span></span>
|<span data-ttu-id="99d31-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="99d31-109">Member</span></span>|<span data-ttu-id="99d31-110">値</span><span class="sxs-lookup"><span data-stu-id="99d31-110">Value</span></span>|<span data-ttu-id="99d31-111">説明</span><span class="sxs-lookup"><span data-stu-id="99d31-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99d31-112">none</span><span class="sxs-lookup"><span data-stu-id="99d31-112">none</span></span>|<span data-ttu-id="99d31-113">0</span><span class="sxs-lookup"><span data-stu-id="99d31-113">0</span></span>|<span data-ttu-id="99d31-114">問題はありません。</span><span class="sxs-lookup"><span data-stu-id="99d31-114">No issue.</span></span>|
|<span data-ttu-id="99d31-115">rootedDevice</span><span class="sxs-lookup"><span data-stu-id="99d31-115">rootedDevice</span></span>|<span data-ttu-id="99d31-116">1</span><span class="sxs-lookup"><span data-stu-id="99d31-116">1</span></span>|<span data-ttu-id="99d31-117">ルートとロック解除のデバイスでアプリケーションの登録が行われています。</span><span class="sxs-lookup"><span data-stu-id="99d31-117">The app registration is running on a rooted/unlocked device.</span></span>|





