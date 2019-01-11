---
title: installState 列挙型
description: インストール状態の値です。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 6898a95b014a3b79db8a38b9a1007bc36ba2f6bd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27877239"
---
# <a name="installstate-enum-type"></a><span data-ttu-id="55e94-103">installState 列挙型</span><span class="sxs-lookup"><span data-stu-id="55e94-103">installState enum type</span></span>

> <span data-ttu-id="55e94-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="55e94-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="55e94-105">インストール状態の値です。</span><span class="sxs-lookup"><span data-stu-id="55e94-105">Possible values for install state.</span></span>
## <a name="members"></a><span data-ttu-id="55e94-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="55e94-106">Members</span></span>
|<span data-ttu-id="55e94-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="55e94-107">Member</span></span>|<span data-ttu-id="55e94-108">値</span><span class="sxs-lookup"><span data-stu-id="55e94-108">Value</span></span>|<span data-ttu-id="55e94-109">説明</span><span class="sxs-lookup"><span data-stu-id="55e94-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55e94-110">質問表</span><span class="sxs-lookup"><span data-stu-id="55e94-110">notApplicable</span></span>|<span data-ttu-id="55e94-111">0</span><span class="sxs-lookup"><span data-stu-id="55e94-111">0</span></span>|<span data-ttu-id="55e94-112">適用されません。</span><span class="sxs-lookup"><span data-stu-id="55e94-112">Not Applicable.</span></span>|
|<span data-ttu-id="55e94-113">インストールされています。</span><span class="sxs-lookup"><span data-stu-id="55e94-113">installed</span></span>|<span data-ttu-id="55e94-114">1</span><span class="sxs-lookup"><span data-stu-id="55e94-114">1</span></span>|<span data-ttu-id="55e94-115">インストールされています。</span><span class="sxs-lookup"><span data-stu-id="55e94-115">Installed.</span></span>|
|<span data-ttu-id="55e94-116">失敗しました。</span><span class="sxs-lookup"><span data-stu-id="55e94-116">failed</span></span>|<span data-ttu-id="55e94-117">2</span><span class="sxs-lookup"><span data-stu-id="55e94-117">2</span></span>|<span data-ttu-id="55e94-118">失敗しました。</span><span class="sxs-lookup"><span data-stu-id="55e94-118">Failed.</span></span>|
|<span data-ttu-id="55e94-119">notInstalled</span><span class="sxs-lookup"><span data-stu-id="55e94-119">notInstalled</span></span>|<span data-ttu-id="55e94-120">3</span><span class="sxs-lookup"><span data-stu-id="55e94-120">3</span></span>|<span data-ttu-id="55e94-121">インストールされていません。</span><span class="sxs-lookup"><span data-stu-id="55e94-121">Not Installed.</span></span>|
|<span data-ttu-id="55e94-122">uninstallFailed</span><span class="sxs-lookup"><span data-stu-id="55e94-122">uninstallFailed</span></span>|<span data-ttu-id="55e94-123">4</span><span class="sxs-lookup"><span data-stu-id="55e94-123">4</span></span>|<span data-ttu-id="55e94-124">アンインストールできませんでした。</span><span class="sxs-lookup"><span data-stu-id="55e94-124">Uninstall Failed.</span></span>|
|<span data-ttu-id="55e94-125">不明</span><span class="sxs-lookup"><span data-stu-id="55e94-125">unknown</span></span>|<span data-ttu-id="55e94-126">5</span><span class="sxs-lookup"><span data-stu-id="55e94-126">5</span></span>|<span data-ttu-id="55e94-127">不明。</span><span class="sxs-lookup"><span data-stu-id="55e94-127">Unknown.</span></span>|



