---
title: sharedPCAllowedAccountType 列挙型
description: PC の共有が許可されているアカウントの種類。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 093b695e6ae5fad885f393e7690dd26f4300c59e
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34964228"
---
# <a name="sharedpcallowedaccounttype-enum-type"></a><span data-ttu-id="c6c4f-103">sharedPCAllowedAccountType 列挙型</span><span class="sxs-lookup"><span data-stu-id="c6c4f-103">sharedPCAllowedAccountType enum type</span></span>

> <span data-ttu-id="c6c4f-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c6c4f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c6c4f-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c6c4f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c6c4f-106">PC の共有が許可されているアカウントの種類。</span><span class="sxs-lookup"><span data-stu-id="c6c4f-106">Type of accounts that are allowed to share the PC.</span></span>

## <a name="members"></a><span data-ttu-id="c6c4f-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="c6c4f-107">Members</span></span>
|<span data-ttu-id="c6c4f-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="c6c4f-108">Member</span></span>|<span data-ttu-id="c6c4f-109">値</span><span class="sxs-lookup"><span data-stu-id="c6c4f-109">Value</span></span>|<span data-ttu-id="c6c4f-110">説明</span><span class="sxs-lookup"><span data-stu-id="c6c4f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6c4f-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="c6c4f-111">notConfigured</span></span>|<span data-ttu-id="c6c4f-112">.0</span><span class="sxs-lookup"><span data-stu-id="c6c4f-112">0</span></span>|<span data-ttu-id="c6c4f-113">構成されていません。</span><span class="sxs-lookup"><span data-stu-id="c6c4f-113">Not configured.</span></span> <span data-ttu-id="c6c4f-114">既定値です。</span><span class="sxs-lookup"><span data-stu-id="c6c4f-114">Default value.</span></span>|
|<span data-ttu-id="c6c4f-115">しあわせ</span><span class="sxs-lookup"><span data-stu-id="c6c4f-115">guest</span></span>|<span data-ttu-id="c6c4f-116">1-d</span><span class="sxs-lookup"><span data-stu-id="c6c4f-116">1</span></span>|<span data-ttu-id="c6c4f-117">Guest アカウントのみ。</span><span class="sxs-lookup"><span data-stu-id="c6c4f-117">Only guest accounts.</span></span>|
|<span data-ttu-id="c6c4f-118">domain</span><span class="sxs-lookup"><span data-stu-id="c6c4f-118">domain</span></span>|<span data-ttu-id="c6c4f-119">pbm-2</span><span class="sxs-lookup"><span data-stu-id="c6c4f-119">2</span></span>|<span data-ttu-id="c6c4f-120">ドメインに参加しているアカウントのみ</span><span class="sxs-lookup"><span data-stu-id="c6c4f-120">Only domain-joined accounts.</span></span>|





