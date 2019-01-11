---
title: runState 列挙型
description: デバイスの管理スクリプトの実行ステータスの種類を示します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 38831625e5f3fc5f3e05b599054c738482b0a6cb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845004"
---
# <a name="runstate-enum-type"></a><span data-ttu-id="0f624-103">runState 列挙型</span><span class="sxs-lookup"><span data-stu-id="0f624-103">runState enum type</span></span>

> <span data-ttu-id="0f624-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0f624-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0f624-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0f624-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0f624-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0f624-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0f624-107">デバイスの管理スクリプトの実行ステータスの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="0f624-107">Indicates the type of execution status of the device management script.</span></span>
## <a name="members"></a><span data-ttu-id="0f624-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="0f624-108">Members</span></span>
|<span data-ttu-id="0f624-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="0f624-109">Member</span></span>|<span data-ttu-id="0f624-110">値</span><span class="sxs-lookup"><span data-stu-id="0f624-110">Value</span></span>|<span data-ttu-id="0f624-111">説明</span><span class="sxs-lookup"><span data-stu-id="0f624-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f624-112">不明</span><span class="sxs-lookup"><span data-stu-id="0f624-112">unknown</span></span>|<span data-ttu-id="0f624-113">0</span><span class="sxs-lookup"><span data-stu-id="0f624-113">0</span></span>|<span data-ttu-id="0f624-114">不明な結果です。</span><span class="sxs-lookup"><span data-stu-id="0f624-114">Unknown result.</span></span>|
|<span data-ttu-id="0f624-115">success</span><span class="sxs-lookup"><span data-stu-id="0f624-115">success</span></span>|<span data-ttu-id="0f624-116">1</span><span class="sxs-lookup"><span data-stu-id="0f624-116">1</span></span>|<span data-ttu-id="0f624-117">スクリプトが正常に実行します。</span><span class="sxs-lookup"><span data-stu-id="0f624-117">Script is run successfully.</span></span>|
|<span data-ttu-id="0f624-118">失敗します。</span><span class="sxs-lookup"><span data-stu-id="0f624-118">fail</span></span>|<span data-ttu-id="0f624-119">2</span><span class="sxs-lookup"><span data-stu-id="0f624-119">2</span></span>|<span data-ttu-id="0f624-120">スクリプトを実行できませんでした。</span><span class="sxs-lookup"><span data-stu-id="0f624-120">Script failed to run.</span></span>|





