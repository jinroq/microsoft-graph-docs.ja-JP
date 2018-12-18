---
title: folderProtectionType 列挙型
description: フォルダーの保護の使用可能な値
author: tfitzmac
ms.openlocfilehash: 93df62da9bb5d849cba86b52384f45bfe7bd760f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350604"
---
# <a name="folderprotectiontype-enum-type"></a><span data-ttu-id="cddf5-103">folderProtectionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="cddf5-103">folderProtectionType enum type</span></span>

> <span data-ttu-id="cddf5-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="cddf5-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cddf5-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cddf5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cddf5-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="cddf5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cddf5-107">フォルダーの保護の使用可能な値</span><span class="sxs-lookup"><span data-stu-id="cddf5-107">Possible values of Folder Protection</span></span>
## <a name="members"></a><span data-ttu-id="cddf5-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="cddf5-108">Members</span></span>
|<span data-ttu-id="cddf5-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="cddf5-109">Member</span></span>|<span data-ttu-id="cddf5-110">値</span><span class="sxs-lookup"><span data-stu-id="cddf5-110">Value</span></span>|<span data-ttu-id="cddf5-111">説明</span><span class="sxs-lookup"><span data-stu-id="cddf5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cddf5-112">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="cddf5-112">userDefined</span></span>|<span data-ttu-id="cddf5-113">0</span><span class="sxs-lookup"><span data-stu-id="cddf5-113">0</span></span>|<span data-ttu-id="cddf5-114">デバイスの既定値でことを目的しません。</span><span class="sxs-lookup"><span data-stu-id="cddf5-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="cddf5-115">有効にします。</span><span class="sxs-lookup"><span data-stu-id="cddf5-115">enable</span></span>|<span data-ttu-id="cddf5-116">1</span><span class="sxs-lookup"><span data-stu-id="cddf5-116">1</span></span>|<span data-ttu-id="cddf5-117">機能をブロックします。</span><span class="sxs-lookup"><span data-stu-id="cddf5-117">Block functionality.</span></span>|
|<span data-ttu-id="cddf5-118">auditMode</span><span class="sxs-lookup"><span data-stu-id="cddf5-118">auditMode</span></span>|<span data-ttu-id="cddf5-119">2</span><span class="sxs-lookup"><span data-stu-id="cddf5-119">2</span></span>|<span data-ttu-id="cddf5-120">機能を許可するが、ログを生成します。</span><span class="sxs-lookup"><span data-stu-id="cddf5-120">Allow functionality but generate logs.</span></span>|
|<span data-ttu-id="cddf5-121">blockDiskModification</span><span class="sxs-lookup"><span data-stu-id="cddf5-121">blockDiskModification</span></span>|<span data-ttu-id="cddf5-122">3</span><span class="sxs-lookup"><span data-stu-id="cddf5-122">3</span></span>|<span data-ttu-id="cddf5-123">ディスク ・ セクターへの書き込みから信頼されていないアプリケーションをブロックします。</span><span class="sxs-lookup"><span data-stu-id="cddf5-123">Block untrusted apps from writing to disk sectors.</span></span>|
|<span data-ttu-id="cddf5-124">auditDiskModification</span><span class="sxs-lookup"><span data-stu-id="cddf5-124">auditDiskModification</span></span>|<span data-ttu-id="cddf5-125">4</span><span class="sxs-lookup"><span data-stu-id="cddf5-125">4</span></span>|<span data-ttu-id="cddf5-126">信頼されていないアプリケーションがディスクのセクターに書き込むときは、ログを生成します。</span><span class="sxs-lookup"><span data-stu-id="cddf5-126">Generate logs when untrusted apps write to disk sectors.</span></span>|





