---
title: sharedPCAllowedAccountType 列挙型
description: PC の共有を許可するアカウントの種類です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1f3948cd149e8779cc06d2d24bfaa6119fcb08ae
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399305"
---
# <a name="sharedpcallowedaccounttype-enum-type"></a><span data-ttu-id="c7967-103">sharedPCAllowedAccountType 列挙型</span><span class="sxs-lookup"><span data-stu-id="c7967-103">sharedPCAllowedAccountType enum type</span></span>

> <span data-ttu-id="c7967-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c7967-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c7967-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c7967-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c7967-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c7967-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7967-107">PC の共有を許可するアカウントの種類です。</span><span class="sxs-lookup"><span data-stu-id="c7967-107">Type of accounts that are allowed to share the PC.</span></span>

## <a name="members"></a><span data-ttu-id="c7967-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="c7967-108">Members</span></span>
|<span data-ttu-id="c7967-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="c7967-109">Member</span></span>|<span data-ttu-id="c7967-110">値</span><span class="sxs-lookup"><span data-stu-id="c7967-110">Value</span></span>|<span data-ttu-id="c7967-111">説明</span><span class="sxs-lookup"><span data-stu-id="c7967-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7967-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="c7967-112">notConfigured</span></span>|<span data-ttu-id="c7967-113">0</span><span class="sxs-lookup"><span data-stu-id="c7967-113">0</span></span>|<span data-ttu-id="c7967-114">構成されていません。</span><span class="sxs-lookup"><span data-stu-id="c7967-114">Not configured.</span></span> <span data-ttu-id="c7967-115">既定値です。</span><span class="sxs-lookup"><span data-stu-id="c7967-115">Default value.</span></span>|
|<span data-ttu-id="c7967-116">ゲスト</span><span class="sxs-lookup"><span data-stu-id="c7967-116">guest</span></span>|<span data-ttu-id="c7967-117">1</span><span class="sxs-lookup"><span data-stu-id="c7967-117">1</span></span>|<span data-ttu-id="c7967-118">Guest アカウントだけです。</span><span class="sxs-lookup"><span data-stu-id="c7967-118">Only guest accounts.</span></span>|
|<span data-ttu-id="c7967-119">domain</span><span class="sxs-lookup"><span data-stu-id="c7967-119">domain</span></span>|<span data-ttu-id="c7967-120">2</span><span class="sxs-lookup"><span data-stu-id="c7967-120">2</span></span>|<span data-ttu-id="c7967-121">ドメインに参加しているアカウントだけです。</span><span class="sxs-lookup"><span data-stu-id="c7967-121">Only domain-joined accounts.</span></span>|




