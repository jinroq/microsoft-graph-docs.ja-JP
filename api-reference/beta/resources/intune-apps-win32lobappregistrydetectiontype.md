---
title: win32LobAppRegistryDetectionType 列挙型
description: すべて含まれているレジストリ データの検出の種類をサポートします。
author: tfitzmac
ms.openlocfilehash: d47d13c01d282d73d65f559e016bde5f74248158
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27362490"
---
# <a name="win32lobappregistrydetectiontype-enum-type"></a><span data-ttu-id="d7187-103">win32LobAppRegistryDetectionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="d7187-103">win32LobAppRegistryDetectionType enum type</span></span>

> <span data-ttu-id="d7187-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d7187-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d7187-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d7187-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d7187-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d7187-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d7187-107">すべて含まれているレジストリ データの検出の種類をサポートします。</span><span class="sxs-lookup"><span data-stu-id="d7187-107">Contains all supported registry data detection type.</span></span>
## <a name="members"></a><span data-ttu-id="d7187-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="d7187-108">Members</span></span>
|<span data-ttu-id="d7187-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="d7187-109">Member</span></span>|<span data-ttu-id="d7187-110">値</span><span class="sxs-lookup"><span data-stu-id="d7187-110">Value</span></span>|<span data-ttu-id="d7187-111">説明</span><span class="sxs-lookup"><span data-stu-id="d7187-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7187-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="d7187-112">notConfigured</span></span>|<span data-ttu-id="d7187-113">0</span><span class="sxs-lookup"><span data-stu-id="d7187-113">0</span></span>|<span data-ttu-id="d7187-114">構成されていません。</span><span class="sxs-lookup"><span data-stu-id="d7187-114">Not configured.</span></span>|
|<span data-ttu-id="d7187-115">存在します。</span><span class="sxs-lookup"><span data-stu-id="d7187-115">exists</span></span>|<span data-ttu-id="d7187-116">1</span><span class="sxs-lookup"><span data-stu-id="d7187-116">1</span></span>|<span data-ttu-id="d7187-117">指定したレジストリ キーまたは値が存在します。</span><span class="sxs-lookup"><span data-stu-id="d7187-117">The specified registry key or value exists.</span></span>|
|<span data-ttu-id="d7187-118">doesNotExist</span><span class="sxs-lookup"><span data-stu-id="d7187-118">doesNotExist</span></span>|<span data-ttu-id="d7187-119">2</span><span class="sxs-lookup"><span data-stu-id="d7187-119">2</span></span>|<span data-ttu-id="d7187-120">指定したレジストリ キーまたは値が存在しません。</span><span class="sxs-lookup"><span data-stu-id="d7187-120">The specified registry key or value does not exist.</span></span>|
|<span data-ttu-id="d7187-121">string</span><span class="sxs-lookup"><span data-stu-id="d7187-121">string</span></span>|<span data-ttu-id="d7187-122">3</span><span class="sxs-lookup"><span data-stu-id="d7187-122">3</span></span>|<span data-ttu-id="d7187-123">値型の文字列を指定します。</span><span class="sxs-lookup"><span data-stu-id="d7187-123">String value type.</span></span>|
|<span data-ttu-id="d7187-124">integer</span><span class="sxs-lookup"><span data-stu-id="d7187-124">integer</span></span>|<span data-ttu-id="d7187-125">4</span><span class="sxs-lookup"><span data-stu-id="d7187-125">4</span></span>|<span data-ttu-id="d7187-126">整数値型。</span><span class="sxs-lookup"><span data-stu-id="d7187-126">Integer value type.</span></span>|
|<span data-ttu-id="d7187-127">version</span><span class="sxs-lookup"><span data-stu-id="d7187-127">version</span></span>|<span data-ttu-id="d7187-128">5</span><span class="sxs-lookup"><span data-stu-id="d7187-128">5</span></span>|<span data-ttu-id="d7187-129">バージョンの値の型。</span><span class="sxs-lookup"><span data-stu-id="d7187-129">Version value type.</span></span>|





