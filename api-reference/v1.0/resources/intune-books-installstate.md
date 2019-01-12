---
title: installState 列挙型
description: インストール状態の値です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b50fb44c2af31efff81f2dd7097505f71bc791d5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947551"
---
# <a name="installstate-enum-type"></a><span data-ttu-id="bdb18-103">installState 列挙型</span><span class="sxs-lookup"><span data-stu-id="bdb18-103">installState enum type</span></span>

> <span data-ttu-id="bdb18-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="bdb18-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bdb18-105">インストール状態の値です。</span><span class="sxs-lookup"><span data-stu-id="bdb18-105">Possible values for install state.</span></span>
## <a name="members"></a><span data-ttu-id="bdb18-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="bdb18-106">Members</span></span>
|<span data-ttu-id="bdb18-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="bdb18-107">Member</span></span>|<span data-ttu-id="bdb18-108">値</span><span class="sxs-lookup"><span data-stu-id="bdb18-108">Value</span></span>|<span data-ttu-id="bdb18-109">説明</span><span class="sxs-lookup"><span data-stu-id="bdb18-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bdb18-110">質問表</span><span class="sxs-lookup"><span data-stu-id="bdb18-110">notApplicable</span></span>|<span data-ttu-id="bdb18-111">0</span><span class="sxs-lookup"><span data-stu-id="bdb18-111">0</span></span>|<span data-ttu-id="bdb18-112">適用されません。</span><span class="sxs-lookup"><span data-stu-id="bdb18-112">Not Applicable.</span></span>|
|<span data-ttu-id="bdb18-113">インストールされています。</span><span class="sxs-lookup"><span data-stu-id="bdb18-113">installed</span></span>|<span data-ttu-id="bdb18-114">1</span><span class="sxs-lookup"><span data-stu-id="bdb18-114">1</span></span>|<span data-ttu-id="bdb18-115">インストールされています。</span><span class="sxs-lookup"><span data-stu-id="bdb18-115">Installed.</span></span>|
|<span data-ttu-id="bdb18-116">失敗しました。</span><span class="sxs-lookup"><span data-stu-id="bdb18-116">failed</span></span>|<span data-ttu-id="bdb18-117">2</span><span class="sxs-lookup"><span data-stu-id="bdb18-117">2</span></span>|<span data-ttu-id="bdb18-118">失敗しました。</span><span class="sxs-lookup"><span data-stu-id="bdb18-118">Failed.</span></span>|
|<span data-ttu-id="bdb18-119">notInstalled</span><span class="sxs-lookup"><span data-stu-id="bdb18-119">notInstalled</span></span>|<span data-ttu-id="bdb18-120">3</span><span class="sxs-lookup"><span data-stu-id="bdb18-120">3</span></span>|<span data-ttu-id="bdb18-121">インストールされていません。</span><span class="sxs-lookup"><span data-stu-id="bdb18-121">Not Installed.</span></span>|
|<span data-ttu-id="bdb18-122">uninstallFailed</span><span class="sxs-lookup"><span data-stu-id="bdb18-122">uninstallFailed</span></span>|<span data-ttu-id="bdb18-123">4</span><span class="sxs-lookup"><span data-stu-id="bdb18-123">4</span></span>|<span data-ttu-id="bdb18-124">アンインストールできませんでした。</span><span class="sxs-lookup"><span data-stu-id="bdb18-124">Uninstall Failed.</span></span>|
|<span data-ttu-id="bdb18-125">不明</span><span class="sxs-lookup"><span data-stu-id="bdb18-125">unknown</span></span>|<span data-ttu-id="bdb18-126">5</span><span class="sxs-lookup"><span data-stu-id="bdb18-126">5</span></span>|<span data-ttu-id="bdb18-127">不明。</span><span class="sxs-lookup"><span data-stu-id="bdb18-127">Unknown.</span></span>|



