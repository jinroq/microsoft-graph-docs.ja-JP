---
title: windowsSModeConfiguration 列挙型
description: S モードを構成するのには使用可能なオプションのロックを解除します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 858be5b3a55fbbf4454aa576785ba793f501079c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415468"
---
# <a name="windowssmodeconfiguration-enum-type"></a><span data-ttu-id="eebe6-103">windowsSModeConfiguration 列挙型</span><span class="sxs-lookup"><span data-stu-id="eebe6-103">windowsSModeConfiguration enum type</span></span>

> <span data-ttu-id="eebe6-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="eebe6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="eebe6-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eebe6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="eebe6-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="eebe6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eebe6-107">S モードを構成するのには使用可能なオプションのロックを解除します。</span><span class="sxs-lookup"><span data-stu-id="eebe6-107">The possible options to configure S mode unlock</span></span>

## <a name="members"></a><span data-ttu-id="eebe6-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="eebe6-108">Members</span></span>
|<span data-ttu-id="eebe6-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="eebe6-109">Member</span></span>|<span data-ttu-id="eebe6-110">値</span><span class="sxs-lookup"><span data-stu-id="eebe6-110">Value</span></span>|<span data-ttu-id="eebe6-111">説明</span><span class="sxs-lookup"><span data-stu-id="eebe6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eebe6-112">noRestriction</span><span class="sxs-lookup"><span data-stu-id="eebe6-112">noRestriction</span></span>|<span data-ttu-id="eebe6-113">0</span><span class="sxs-lookup"><span data-stu-id="eebe6-113">0</span></span>|<span data-ttu-id="eebe6-114">このオプションでは、S モードの既定のロックを解除するすべての制限を削除します。</span><span class="sxs-lookup"><span data-stu-id="eebe6-114">This option will remove all restrictions to unlock S mode - default</span></span>|
|<span data-ttu-id="eebe6-115">ブロック</span><span class="sxs-lookup"><span data-stu-id="eebe6-115">block</span></span>|<span data-ttu-id="eebe6-116">1</span><span class="sxs-lookup"><span data-stu-id="eebe6-116">1</span></span>|<span data-ttu-id="eebe6-117">このオプションは S モードのデバイスのロックを解除するユーザーをブロックします。</span><span class="sxs-lookup"><span data-stu-id="eebe6-117">This option will block the user to unlock the device from S mode</span></span>|
|<span data-ttu-id="eebe6-118">ロックを解除します。</span><span class="sxs-lookup"><span data-stu-id="eebe6-118">unlock</span></span>|<span data-ttu-id="eebe6-119">2</span><span class="sxs-lookup"><span data-stu-id="eebe6-119">2</span></span>|<span data-ttu-id="eebe6-120">このオプションは S モードのデバイスのロックを解除します。</span><span class="sxs-lookup"><span data-stu-id="eebe6-120">This option will unlock the device from S mode</span></span>|




