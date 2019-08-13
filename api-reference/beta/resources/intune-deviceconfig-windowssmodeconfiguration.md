---
title: windowsSModeConfiguration 列挙型
description: S モードのロック解除を構成するために使用可能なオプション
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: aaf6b8c36ea5d0de5628043f87db89ecc62c6490
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369620"
---
# <a name="windowssmodeconfiguration-enum-type"></a><span data-ttu-id="94b2a-103">windowsSModeConfiguration 列挙型</span><span class="sxs-lookup"><span data-stu-id="94b2a-103">windowsSModeConfiguration enum type</span></span>

> <span data-ttu-id="94b2a-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="94b2a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="94b2a-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="94b2a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="94b2a-106">S モードのロック解除を構成するために使用可能なオプション</span><span class="sxs-lookup"><span data-stu-id="94b2a-106">The possible options to configure S mode unlock</span></span>

## <a name="members"></a><span data-ttu-id="94b2a-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="94b2a-107">Members</span></span>
|<span data-ttu-id="94b2a-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="94b2a-108">Member</span></span>|<span data-ttu-id="94b2a-109">値</span><span class="sxs-lookup"><span data-stu-id="94b2a-109">Value</span></span>|<span data-ttu-id="94b2a-110">説明</span><span class="sxs-lookup"><span data-stu-id="94b2a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94b2a-111">noRestriction</span><span class="sxs-lookup"><span data-stu-id="94b2a-111">noRestriction</span></span>|<span data-ttu-id="94b2a-112">.0</span><span class="sxs-lookup"><span data-stu-id="94b2a-112">0</span></span>|<span data-ttu-id="94b2a-113">このオプションを選択すると、ロックを解除するためのすべての制限が削除されます-既定値</span><span class="sxs-lookup"><span data-stu-id="94b2a-113">This option will remove all restrictions to unlock S mode - default</span></span>|
|<span data-ttu-id="94b2a-114">拒否</span><span class="sxs-lookup"><span data-stu-id="94b2a-114">block</span></span>|<span data-ttu-id="94b2a-115">1-d</span><span class="sxs-lookup"><span data-stu-id="94b2a-115">1</span></span>|<span data-ttu-id="94b2a-116">このオプションは、ユーザーが S モードからデバイスのロックを解除するのをブロックします。</span><span class="sxs-lookup"><span data-stu-id="94b2a-116">This option will block the user to unlock the device from S mode</span></span>|
|<span data-ttu-id="94b2a-117">外す</span><span class="sxs-lookup"><span data-stu-id="94b2a-117">unlock</span></span>|<span data-ttu-id="94b2a-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="94b2a-118">2</span></span>|<span data-ttu-id="94b2a-119">このオプションでは、デバイスを S モードからロック解除します。</span><span class="sxs-lookup"><span data-stu-id="94b2a-119">This option will unlock the device from S mode</span></span>|



