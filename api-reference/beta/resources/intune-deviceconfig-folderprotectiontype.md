---
title: folderProtectionType 列挙型
description: フォルダーの保護の使用可能な値
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 435f3ea01f5a8ffc3c4cb54034d415d54732db5d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826132"
---
# <a name="folderprotectiontype-enum-type"></a><span data-ttu-id="313fa-103">folderProtectionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="313fa-103">folderProtectionType enum type</span></span>

> <span data-ttu-id="313fa-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="313fa-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="313fa-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="313fa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="313fa-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="313fa-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="313fa-107">フォルダーの保護の使用可能な値</span><span class="sxs-lookup"><span data-stu-id="313fa-107">Possible values of Folder Protection</span></span>
## <a name="members"></a><span data-ttu-id="313fa-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="313fa-108">Members</span></span>
|<span data-ttu-id="313fa-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="313fa-109">Member</span></span>|<span data-ttu-id="313fa-110">値</span><span class="sxs-lookup"><span data-stu-id="313fa-110">Value</span></span>|<span data-ttu-id="313fa-111">説明</span><span class="sxs-lookup"><span data-stu-id="313fa-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="313fa-112">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="313fa-112">userDefined</span></span>|<span data-ttu-id="313fa-113">0</span><span class="sxs-lookup"><span data-stu-id="313fa-113">0</span></span>|<span data-ttu-id="313fa-114">デバイスの既定値でことを目的しません。</span><span class="sxs-lookup"><span data-stu-id="313fa-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="313fa-115">有効にします。</span><span class="sxs-lookup"><span data-stu-id="313fa-115">enable</span></span>|<span data-ttu-id="313fa-116">1</span><span class="sxs-lookup"><span data-stu-id="313fa-116">1</span></span>|<span data-ttu-id="313fa-117">機能をブロックします。</span><span class="sxs-lookup"><span data-stu-id="313fa-117">Block functionality.</span></span>|
|<span data-ttu-id="313fa-118">auditMode</span><span class="sxs-lookup"><span data-stu-id="313fa-118">auditMode</span></span>|<span data-ttu-id="313fa-119">2</span><span class="sxs-lookup"><span data-stu-id="313fa-119">2</span></span>|<span data-ttu-id="313fa-120">機能を許可するが、ログを生成します。</span><span class="sxs-lookup"><span data-stu-id="313fa-120">Allow functionality but generate logs.</span></span>|
|<span data-ttu-id="313fa-121">blockDiskModification</span><span class="sxs-lookup"><span data-stu-id="313fa-121">blockDiskModification</span></span>|<span data-ttu-id="313fa-122">3</span><span class="sxs-lookup"><span data-stu-id="313fa-122">3</span></span>|<span data-ttu-id="313fa-123">ディスク ・ セクターへの書き込みから信頼されていないアプリケーションをブロックします。</span><span class="sxs-lookup"><span data-stu-id="313fa-123">Block untrusted apps from writing to disk sectors.</span></span>|
|<span data-ttu-id="313fa-124">auditDiskModification</span><span class="sxs-lookup"><span data-stu-id="313fa-124">auditDiskModification</span></span>|<span data-ttu-id="313fa-125">4</span><span class="sxs-lookup"><span data-stu-id="313fa-125">4</span></span>|<span data-ttu-id="313fa-126">信頼されていないアプリケーションがディスクのセクターに書き込むときは、ログを生成します。</span><span class="sxs-lookup"><span data-stu-id="313fa-126">Generate logs when untrusted apps write to disk sectors.</span></span>|





