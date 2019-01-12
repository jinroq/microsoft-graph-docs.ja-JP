---
title: installState 列挙型
description: インストール状態の値です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 92fa9887760835a02c26858fb11503a0841d912e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985383"
---
# <a name="installstate-enum-type"></a><span data-ttu-id="068be-103">installState 列挙型</span><span class="sxs-lookup"><span data-stu-id="068be-103">installState enum type</span></span>

> <span data-ttu-id="068be-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="068be-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="068be-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="068be-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="068be-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="068be-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="068be-107">インストール状態の値です。</span><span class="sxs-lookup"><span data-stu-id="068be-107">Possible values for install state.</span></span>
## <a name="members"></a><span data-ttu-id="068be-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="068be-108">Members</span></span>
|<span data-ttu-id="068be-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="068be-109">Member</span></span>|<span data-ttu-id="068be-110">値</span><span class="sxs-lookup"><span data-stu-id="068be-110">Value</span></span>|<span data-ttu-id="068be-111">説明</span><span class="sxs-lookup"><span data-stu-id="068be-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="068be-112">質問表</span><span class="sxs-lookup"><span data-stu-id="068be-112">notApplicable</span></span>|<span data-ttu-id="068be-113">0</span><span class="sxs-lookup"><span data-stu-id="068be-113">0</span></span>|<span data-ttu-id="068be-114">適用されません。</span><span class="sxs-lookup"><span data-stu-id="068be-114">Not Applicable.</span></span>|
|<span data-ttu-id="068be-115">インストールされています。</span><span class="sxs-lookup"><span data-stu-id="068be-115">installed</span></span>|<span data-ttu-id="068be-116">1</span><span class="sxs-lookup"><span data-stu-id="068be-116">1</span></span>|<span data-ttu-id="068be-117">インストールされています。</span><span class="sxs-lookup"><span data-stu-id="068be-117">Installed.</span></span>|
|<span data-ttu-id="068be-118">失敗しました。</span><span class="sxs-lookup"><span data-stu-id="068be-118">failed</span></span>|<span data-ttu-id="068be-119">2</span><span class="sxs-lookup"><span data-stu-id="068be-119">2</span></span>|<span data-ttu-id="068be-120">失敗しました。</span><span class="sxs-lookup"><span data-stu-id="068be-120">Failed.</span></span>|
|<span data-ttu-id="068be-121">notInstalled</span><span class="sxs-lookup"><span data-stu-id="068be-121">notInstalled</span></span>|<span data-ttu-id="068be-122">3</span><span class="sxs-lookup"><span data-stu-id="068be-122">3</span></span>|<span data-ttu-id="068be-123">インストールされていません。</span><span class="sxs-lookup"><span data-stu-id="068be-123">Not Installed.</span></span>|
|<span data-ttu-id="068be-124">uninstallFailed</span><span class="sxs-lookup"><span data-stu-id="068be-124">uninstallFailed</span></span>|<span data-ttu-id="068be-125">4</span><span class="sxs-lookup"><span data-stu-id="068be-125">4</span></span>|<span data-ttu-id="068be-126">アンインストールできませんでした。</span><span class="sxs-lookup"><span data-stu-id="068be-126">Uninstall Failed.</span></span>|
|<span data-ttu-id="068be-127">不明</span><span class="sxs-lookup"><span data-stu-id="068be-127">unknown</span></span>|<span data-ttu-id="068be-128">5</span><span class="sxs-lookup"><span data-stu-id="068be-128">5</span></span>|<span data-ttu-id="068be-129">不明。</span><span class="sxs-lookup"><span data-stu-id="068be-129">Unknown.</span></span>|





