---
title: sharedPCAccountDeletionPolicyType 列挙型
description: 共有 PC でアカウントを削除する場合に使用できる値。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 0e9c98a40992bd9404f101f07640014a3f4b6ab5
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36367996"
---
# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a><span data-ttu-id="823bf-103">sharedPCAccountDeletionPolicyType 列挙型</span><span class="sxs-lookup"><span data-stu-id="823bf-103">sharedPCAccountDeletionPolicyType enum type</span></span>

> <span data-ttu-id="823bf-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="823bf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="823bf-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="823bf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="823bf-106">共有 PC でアカウントを削除する場合に使用できる値。</span><span class="sxs-lookup"><span data-stu-id="823bf-106">Possible values for when accounts are deleted on a shared PC.</span></span>

## <a name="members"></a><span data-ttu-id="823bf-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="823bf-107">Members</span></span>
|<span data-ttu-id="823bf-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="823bf-108">Member</span></span>|<span data-ttu-id="823bf-109">値</span><span class="sxs-lookup"><span data-stu-id="823bf-109">Value</span></span>|<span data-ttu-id="823bf-110">説明</span><span class="sxs-lookup"><span data-stu-id="823bf-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="823bf-111">瞬時</span><span class="sxs-lookup"><span data-stu-id="823bf-111">immediate</span></span>|<span data-ttu-id="823bf-112">.0</span><span class="sxs-lookup"><span data-stu-id="823bf-112">0</span></span>|<span data-ttu-id="823bf-113">すぐに削除します。</span><span class="sxs-lookup"><span data-stu-id="823bf-113">Delete immediately.</span></span>|
|<span data-ttu-id="823bf-114">ディスクスペースしきい値</span><span class="sxs-lookup"><span data-stu-id="823bf-114">diskSpaceThreshold</span></span>|<span data-ttu-id="823bf-115">1-d</span><span class="sxs-lookup"><span data-stu-id="823bf-115">1</span></span>|<span data-ttu-id="823bf-116">ディスク容量のしきい値で削除します。</span><span class="sxs-lookup"><span data-stu-id="823bf-116">Delete at disk space threshold.</span></span>|
|<span data-ttu-id="823bf-117">diskSpaceThresholdOrInactiveThreshold</span><span class="sxs-lookup"><span data-stu-id="823bf-117">diskSpaceThresholdOrInactiveThreshold</span></span>|<span data-ttu-id="823bf-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="823bf-118">2</span></span>|<span data-ttu-id="823bf-119">ディスク容量のしきい値または非アクティブなしきい値での削除。</span><span class="sxs-lookup"><span data-stu-id="823bf-119">Delete at disk space threshold or inactive threshold.</span></span>|



