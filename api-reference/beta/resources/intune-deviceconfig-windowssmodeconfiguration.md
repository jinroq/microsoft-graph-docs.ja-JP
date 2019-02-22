---
title: windowsSModeConfiguration 列挙型
description: S モードのロック解除を構成するために使用可能なオプション
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6a451108c6e55f8587317dfc43caf8bc84cca673
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30144717"
---
# <a name="windowssmodeconfiguration-enum-type"></a><span data-ttu-id="d90e4-103">windowsSModeConfiguration 列挙型</span><span class="sxs-lookup"><span data-stu-id="d90e4-103">windowsSModeConfiguration enum type</span></span>

> <span data-ttu-id="d90e4-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d90e4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d90e4-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d90e4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d90e4-106">S モードのロック解除を構成するために使用可能なオプション</span><span class="sxs-lookup"><span data-stu-id="d90e4-106">The possible options to configure S mode unlock</span></span>

## <a name="members"></a><span data-ttu-id="d90e4-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="d90e4-107">Members</span></span>
|<span data-ttu-id="d90e4-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="d90e4-108">Member</span></span>|<span data-ttu-id="d90e4-109">値</span><span class="sxs-lookup"><span data-stu-id="d90e4-109">Value</span></span>|<span data-ttu-id="d90e4-110">説明</span><span class="sxs-lookup"><span data-stu-id="d90e4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d90e4-111">noRestriction</span><span class="sxs-lookup"><span data-stu-id="d90e4-111">noRestriction</span></span>|<span data-ttu-id="d90e4-112">.0</span><span class="sxs-lookup"><span data-stu-id="d90e4-112">0</span></span>|<span data-ttu-id="d90e4-113">このオプションを選択すると、ロックを解除するためのすべての制限が削除されます-既定値</span><span class="sxs-lookup"><span data-stu-id="d90e4-113">This option will remove all restrictions to unlock S mode - default</span></span>|
|<span data-ttu-id="d90e4-114">拒否</span><span class="sxs-lookup"><span data-stu-id="d90e4-114">block</span></span>|<span data-ttu-id="d90e4-115">1-d</span><span class="sxs-lookup"><span data-stu-id="d90e4-115">1</span></span>|<span data-ttu-id="d90e4-116">このオプションは、ユーザーが S モードからデバイスのロックを解除するのをブロックします。</span><span class="sxs-lookup"><span data-stu-id="d90e4-116">This option will block the user to unlock the device from S mode</span></span>|
|<span data-ttu-id="d90e4-117">外す</span><span class="sxs-lookup"><span data-stu-id="d90e4-117">unlock</span></span>|<span data-ttu-id="d90e4-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="d90e4-118">2</span></span>|<span data-ttu-id="d90e4-119">このオプションでは、デバイスを S モードからロック解除します。</span><span class="sxs-lookup"><span data-stu-id="d90e4-119">This option will unlock the device from S mode</span></span>|




