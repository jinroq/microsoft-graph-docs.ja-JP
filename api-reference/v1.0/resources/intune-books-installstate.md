---
title: installState 列挙型
description: インストール状態の値です。
author: tfitzmac
ms.openlocfilehash: f4c721204b0b523e9e3fcadc7ed2c7d06fe7c966
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27325152"
---
# <a name="installstate-enum-type"></a><span data-ttu-id="409b3-103">installState 列挙型</span><span class="sxs-lookup"><span data-stu-id="409b3-103">installState enum type</span></span>

> <span data-ttu-id="409b3-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="409b3-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="409b3-105">インストール状態の値です。</span><span class="sxs-lookup"><span data-stu-id="409b3-105">Possible values for install state.</span></span>
## <a name="members"></a><span data-ttu-id="409b3-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="409b3-106">Members</span></span>
|<span data-ttu-id="409b3-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="409b3-107">Member</span></span>|<span data-ttu-id="409b3-108">値</span><span class="sxs-lookup"><span data-stu-id="409b3-108">Value</span></span>|<span data-ttu-id="409b3-109">説明</span><span class="sxs-lookup"><span data-stu-id="409b3-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="409b3-110">質問表</span><span class="sxs-lookup"><span data-stu-id="409b3-110">notApplicable</span></span>|<span data-ttu-id="409b3-111">0</span><span class="sxs-lookup"><span data-stu-id="409b3-111">0</span></span>|<span data-ttu-id="409b3-112">適用されません。</span><span class="sxs-lookup"><span data-stu-id="409b3-112">Not Applicable.</span></span>|
|<span data-ttu-id="409b3-113">インストールされています。</span><span class="sxs-lookup"><span data-stu-id="409b3-113">installed</span></span>|<span data-ttu-id="409b3-114">1</span><span class="sxs-lookup"><span data-stu-id="409b3-114">1</span></span>|<span data-ttu-id="409b3-115">インストールされています。</span><span class="sxs-lookup"><span data-stu-id="409b3-115">Installed.</span></span>|
|<span data-ttu-id="409b3-116">失敗しました。</span><span class="sxs-lookup"><span data-stu-id="409b3-116">failed</span></span>|<span data-ttu-id="409b3-117">2</span><span class="sxs-lookup"><span data-stu-id="409b3-117">2</span></span>|<span data-ttu-id="409b3-118">失敗しました。</span><span class="sxs-lookup"><span data-stu-id="409b3-118">Failed.</span></span>|
|<span data-ttu-id="409b3-119">notInstalled</span><span class="sxs-lookup"><span data-stu-id="409b3-119">notInstalled</span></span>|<span data-ttu-id="409b3-120">3</span><span class="sxs-lookup"><span data-stu-id="409b3-120">3</span></span>|<span data-ttu-id="409b3-121">インストールされていません。</span><span class="sxs-lookup"><span data-stu-id="409b3-121">Not Installed.</span></span>|
|<span data-ttu-id="409b3-122">uninstallFailed</span><span class="sxs-lookup"><span data-stu-id="409b3-122">uninstallFailed</span></span>|<span data-ttu-id="409b3-123">4</span><span class="sxs-lookup"><span data-stu-id="409b3-123">4</span></span>|<span data-ttu-id="409b3-124">アンインストールできませんでした。</span><span class="sxs-lookup"><span data-stu-id="409b3-124">Uninstall Failed.</span></span>|
|<span data-ttu-id="409b3-125">不明</span><span class="sxs-lookup"><span data-stu-id="409b3-125">unknown</span></span>|<span data-ttu-id="409b3-126">5</span><span class="sxs-lookup"><span data-stu-id="409b3-126">5</span></span>|<span data-ttu-id="409b3-127">不明。</span><span class="sxs-lookup"><span data-stu-id="409b3-127">Unknown.</span></span>|



