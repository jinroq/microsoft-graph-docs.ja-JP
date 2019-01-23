---
title: groupPolicyConfigurationType 列挙型
description: グループ ポリシーの構成の種類
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 372a5bd5656510c43b388bac128cba4bc46c0988
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430382"
---
# <a name="grouppolicyconfigurationtype-enum-type"></a><span data-ttu-id="1cbb6-103">groupPolicyConfigurationType 列挙型</span><span class="sxs-lookup"><span data-stu-id="1cbb6-103">groupPolicyConfigurationType enum type</span></span>

> <span data-ttu-id="1cbb6-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1cbb6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1cbb6-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1cbb6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1cbb6-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1cbb6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1cbb6-107">グループ ポリシーの構成の種類</span><span class="sxs-lookup"><span data-stu-id="1cbb6-107">Group Policy Configuration Type</span></span>

## <a name="members"></a><span data-ttu-id="1cbb6-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="1cbb6-108">Members</span></span>
|<span data-ttu-id="1cbb6-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="1cbb6-109">Member</span></span>|<span data-ttu-id="1cbb6-110">値</span><span class="sxs-lookup"><span data-stu-id="1cbb6-110">Value</span></span>|<span data-ttu-id="1cbb6-111">説明</span><span class="sxs-lookup"><span data-stu-id="1cbb6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1cbb6-112">役割</span><span class="sxs-lookup"><span data-stu-id="1cbb6-112">policy</span></span>|<span data-ttu-id="1cbb6-113">0</span><span class="sxs-lookup"><span data-stu-id="1cbb6-113">0</span></span>|<span data-ttu-id="1cbb6-114">ポリシーの種類には、値、値が削除される場合は、使用する元の設定値を許可することを意味する tattoo ないです。</span><span class="sxs-lookup"><span data-stu-id="1cbb6-114">The policy type does not tattoo the value, which means the value is removed allowing the original configuration value to be used.</span></span> <span data-ttu-id="1cbb6-115">ポリシーの種類は、アプリケーションの値の対応は常にアプリケーションの構成設定より優先されます。</span><span class="sxs-lookup"><span data-stu-id="1cbb6-115">The policy type supercedes application configuration setting so the application is always aware of the value.</span></span> <span data-ttu-id="1cbb6-116">ポリシーの種類では、ユーザーがアプリケーションのユーザー インターフェイスを使用して値を変更できなくなります。</span><span class="sxs-lookup"><span data-stu-id="1cbb6-116">The policy type prevents the user from modifying the value through the application's user interface.</span></span>|
|<span data-ttu-id="1cbb6-117">preference</span><span class="sxs-lookup"><span data-stu-id="1cbb6-117">preference</span></span>|<span data-ttu-id="1cbb6-118">1</span><span class="sxs-lookup"><span data-stu-id="1cbb6-118">1</span></span>|<span data-ttu-id="1cbb6-119">優先タイプは、値は、値がレジストリから削除されないことを意味を tattoo は。</span><span class="sxs-lookup"><span data-stu-id="1cbb6-119">The preference type does tattoo the value, which means the value is not removed from the registry.</span></span> <span data-ttu-id="1cbb6-120">優先型では、ユーザー設定の値が上書きされ、以前の値は保持されません。</span><span class="sxs-lookup"><span data-stu-id="1cbb6-120">The preference type will overwrite the user configured-value and does not retain the previous value.</span></span> <span data-ttu-id="1cbb6-121">優先型に、アプリケーションのユーザー インターフェイスを使用して値を変更することから、ユーザーができません。</span><span class="sxs-lookup"><span data-stu-id="1cbb6-121">The preference type does not prevent the user from modifying the value through the application's user interface.</span></span>|




