---
title: windowsSModeConfiguration 列挙型
description: S モードを構成するのには使用可能なオプションのロックを解除します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 9e37bd51be1b5476e8b4590b92b3caeeed92ac45
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830738"
---
# <a name="windowssmodeconfiguration-enum-type"></a><span data-ttu-id="ecfa6-103">windowsSModeConfiguration 列挙型</span><span class="sxs-lookup"><span data-stu-id="ecfa6-103">windowsSModeConfiguration enum type</span></span>

> <span data-ttu-id="ecfa6-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ecfa6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ecfa6-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ecfa6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ecfa6-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ecfa6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ecfa6-107">S モードを構成するのには使用可能なオプションのロックを解除します。</span><span class="sxs-lookup"><span data-stu-id="ecfa6-107">The possible options to configure S mode unlock</span></span>
## <a name="members"></a><span data-ttu-id="ecfa6-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="ecfa6-108">Members</span></span>
|<span data-ttu-id="ecfa6-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="ecfa6-109">Member</span></span>|<span data-ttu-id="ecfa6-110">値</span><span class="sxs-lookup"><span data-stu-id="ecfa6-110">Value</span></span>|<span data-ttu-id="ecfa6-111">説明</span><span class="sxs-lookup"><span data-stu-id="ecfa6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ecfa6-112">noRestriction</span><span class="sxs-lookup"><span data-stu-id="ecfa6-112">noRestriction</span></span>|<span data-ttu-id="ecfa6-113">0</span><span class="sxs-lookup"><span data-stu-id="ecfa6-113">0</span></span>|<span data-ttu-id="ecfa6-114">このオプションでは、S モードの既定のロックを解除するすべての制限を削除します。</span><span class="sxs-lookup"><span data-stu-id="ecfa6-114">This option will remove all restrictions to unlock S mode - default</span></span>|
|<span data-ttu-id="ecfa6-115">ブロック</span><span class="sxs-lookup"><span data-stu-id="ecfa6-115">block</span></span>|<span data-ttu-id="ecfa6-116">1</span><span class="sxs-lookup"><span data-stu-id="ecfa6-116">1</span></span>|<span data-ttu-id="ecfa6-117">このオプションは S モードのデバイスのロックを解除するユーザーをブロックします。</span><span class="sxs-lookup"><span data-stu-id="ecfa6-117">This option will block the user to unlock the device from S mode</span></span>|
|<span data-ttu-id="ecfa6-118">ロックを解除します。</span><span class="sxs-lookup"><span data-stu-id="ecfa6-118">unlock</span></span>|<span data-ttu-id="ecfa6-119">2</span><span class="sxs-lookup"><span data-stu-id="ecfa6-119">2</span></span>|<span data-ttu-id="ecfa6-120">このオプションは S モードのデバイスのロックを解除します。</span><span class="sxs-lookup"><span data-stu-id="ecfa6-120">This option will unlock the device from S mode</span></span>|





