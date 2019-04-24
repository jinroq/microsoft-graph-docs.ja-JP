---
title: sharedpcallowedaccounttype 列挙型
description: PC の共有が許可されているアカウントの種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8c450f09a89602493582db5585fe1e565716a4ff
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32464576"
---
# <a name="sharedpcallowedaccounttype-enum-type"></a><span data-ttu-id="b6ece-103">sharedpcallowedaccounttype 列挙型</span><span class="sxs-lookup"><span data-stu-id="b6ece-103">sharedPCAllowedAccountType enum type</span></span>

> <span data-ttu-id="b6ece-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b6ece-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b6ece-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b6ece-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6ece-106">PC の共有が許可されているアカウントの種類。</span><span class="sxs-lookup"><span data-stu-id="b6ece-106">Type of accounts that are allowed to share the PC.</span></span>

## <a name="members"></a><span data-ttu-id="b6ece-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="b6ece-107">Members</span></span>
|<span data-ttu-id="b6ece-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="b6ece-108">Member</span></span>|<span data-ttu-id="b6ece-109">値</span><span class="sxs-lookup"><span data-stu-id="b6ece-109">Value</span></span>|<span data-ttu-id="b6ece-110">説明</span><span class="sxs-lookup"><span data-stu-id="b6ece-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6ece-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="b6ece-111">notConfigured</span></span>|<span data-ttu-id="b6ece-112">.0</span><span class="sxs-lookup"><span data-stu-id="b6ece-112">0</span></span>|<span data-ttu-id="b6ece-113">構成されていません。</span><span class="sxs-lookup"><span data-stu-id="b6ece-113">Not configured.</span></span> <span data-ttu-id="b6ece-114">既定値です。</span><span class="sxs-lookup"><span data-stu-id="b6ece-114">Default value.</span></span>|
|<span data-ttu-id="b6ece-115">しあわせ</span><span class="sxs-lookup"><span data-stu-id="b6ece-115">guest</span></span>|<span data-ttu-id="b6ece-116">1-d</span><span class="sxs-lookup"><span data-stu-id="b6ece-116">1</span></span>|<span data-ttu-id="b6ece-117">guest アカウントのみ。</span><span class="sxs-lookup"><span data-stu-id="b6ece-117">Only guest accounts.</span></span>|
|<span data-ttu-id="b6ece-118">domain</span><span class="sxs-lookup"><span data-stu-id="b6ece-118">domain</span></span>|<span data-ttu-id="b6ece-119">pbm-2</span><span class="sxs-lookup"><span data-stu-id="b6ece-119">2</span></span>|<span data-ttu-id="b6ece-120">ドメインに参加しているアカウントのみ</span><span class="sxs-lookup"><span data-stu-id="b6ece-120">Only domain-joined accounts.</span></span>|





