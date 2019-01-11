---
title: win32LobAppRegistryDetectionType 列挙型
description: すべて含まれているレジストリ データの検出の種類をサポートします。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 60e27e01825c54677bfb88727b8dcbc16a808278
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831854"
---
# <a name="win32lobappregistrydetectiontype-enum-type"></a><span data-ttu-id="7cacb-103">win32LobAppRegistryDetectionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="7cacb-103">win32LobAppRegistryDetectionType enum type</span></span>

> <span data-ttu-id="7cacb-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7cacb-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7cacb-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7cacb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7cacb-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7cacb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7cacb-107">すべて含まれているレジストリ データの検出の種類をサポートします。</span><span class="sxs-lookup"><span data-stu-id="7cacb-107">Contains all supported registry data detection type.</span></span>
## <a name="members"></a><span data-ttu-id="7cacb-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="7cacb-108">Members</span></span>
|<span data-ttu-id="7cacb-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="7cacb-109">Member</span></span>|<span data-ttu-id="7cacb-110">値</span><span class="sxs-lookup"><span data-stu-id="7cacb-110">Value</span></span>|<span data-ttu-id="7cacb-111">説明</span><span class="sxs-lookup"><span data-stu-id="7cacb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7cacb-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="7cacb-112">notConfigured</span></span>|<span data-ttu-id="7cacb-113">0</span><span class="sxs-lookup"><span data-stu-id="7cacb-113">0</span></span>|<span data-ttu-id="7cacb-114">構成されていません。</span><span class="sxs-lookup"><span data-stu-id="7cacb-114">Not configured.</span></span>|
|<span data-ttu-id="7cacb-115">存在します。</span><span class="sxs-lookup"><span data-stu-id="7cacb-115">exists</span></span>|<span data-ttu-id="7cacb-116">1</span><span class="sxs-lookup"><span data-stu-id="7cacb-116">1</span></span>|<span data-ttu-id="7cacb-117">指定したレジストリ キーまたは値が存在します。</span><span class="sxs-lookup"><span data-stu-id="7cacb-117">The specified registry key or value exists.</span></span>|
|<span data-ttu-id="7cacb-118">doesNotExist</span><span class="sxs-lookup"><span data-stu-id="7cacb-118">doesNotExist</span></span>|<span data-ttu-id="7cacb-119">2</span><span class="sxs-lookup"><span data-stu-id="7cacb-119">2</span></span>|<span data-ttu-id="7cacb-120">指定したレジストリ キーまたは値が存在しません。</span><span class="sxs-lookup"><span data-stu-id="7cacb-120">The specified registry key or value does not exist.</span></span>|
|<span data-ttu-id="7cacb-121">文字列</span><span class="sxs-lookup"><span data-stu-id="7cacb-121">string</span></span>|<span data-ttu-id="7cacb-122">3</span><span class="sxs-lookup"><span data-stu-id="7cacb-122">3</span></span>|<span data-ttu-id="7cacb-123">値型の文字列を指定します。</span><span class="sxs-lookup"><span data-stu-id="7cacb-123">String value type.</span></span>|
|<span data-ttu-id="7cacb-124">integer</span><span class="sxs-lookup"><span data-stu-id="7cacb-124">integer</span></span>|<span data-ttu-id="7cacb-125">4</span><span class="sxs-lookup"><span data-stu-id="7cacb-125">4</span></span>|<span data-ttu-id="7cacb-126">整数値型。</span><span class="sxs-lookup"><span data-stu-id="7cacb-126">Integer value type.</span></span>|
|<span data-ttu-id="7cacb-127">version</span><span class="sxs-lookup"><span data-stu-id="7cacb-127">version</span></span>|<span data-ttu-id="7cacb-128">5</span><span class="sxs-lookup"><span data-stu-id="7cacb-128">5</span></span>|<span data-ttu-id="7cacb-129">バージョンの値の型。</span><span class="sxs-lookup"><span data-stu-id="7cacb-129">Version value type.</span></span>|





