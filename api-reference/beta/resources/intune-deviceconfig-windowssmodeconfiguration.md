---
title: windowsSModeConfiguration 列挙型
description: S モードを構成するのには使用可能なオプションのロックを解除します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 28106a073a6bb213fe17e80193cb32d1e6b3b9ce
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947380"
---
# <a name="windowssmodeconfiguration-enum-type"></a><span data-ttu-id="76b92-103">windowsSModeConfiguration 列挙型</span><span class="sxs-lookup"><span data-stu-id="76b92-103">windowsSModeConfiguration enum type</span></span>

> <span data-ttu-id="76b92-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="76b92-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="76b92-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="76b92-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="76b92-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="76b92-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="76b92-107">S モードを構成するのには使用可能なオプションのロックを解除します。</span><span class="sxs-lookup"><span data-stu-id="76b92-107">The possible options to configure S mode unlock</span></span>
## <a name="members"></a><span data-ttu-id="76b92-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="76b92-108">Members</span></span>
|<span data-ttu-id="76b92-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="76b92-109">Member</span></span>|<span data-ttu-id="76b92-110">値</span><span class="sxs-lookup"><span data-stu-id="76b92-110">Value</span></span>|<span data-ttu-id="76b92-111">説明</span><span class="sxs-lookup"><span data-stu-id="76b92-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76b92-112">noRestriction</span><span class="sxs-lookup"><span data-stu-id="76b92-112">noRestriction</span></span>|<span data-ttu-id="76b92-113">0</span><span class="sxs-lookup"><span data-stu-id="76b92-113">0</span></span>|<span data-ttu-id="76b92-114">このオプションでは、S モードの既定のロックを解除するすべての制限を削除します。</span><span class="sxs-lookup"><span data-stu-id="76b92-114">This option will remove all restrictions to unlock S mode - default</span></span>|
|<span data-ttu-id="76b92-115">ブロック</span><span class="sxs-lookup"><span data-stu-id="76b92-115">block</span></span>|<span data-ttu-id="76b92-116">1</span><span class="sxs-lookup"><span data-stu-id="76b92-116">1</span></span>|<span data-ttu-id="76b92-117">このオプションは S モードのデバイスのロックを解除するユーザーをブロックします。</span><span class="sxs-lookup"><span data-stu-id="76b92-117">This option will block the user to unlock the device from S mode</span></span>|
|<span data-ttu-id="76b92-118">ロックを解除します。</span><span class="sxs-lookup"><span data-stu-id="76b92-118">unlock</span></span>|<span data-ttu-id="76b92-119">2</span><span class="sxs-lookup"><span data-stu-id="76b92-119">2</span></span>|<span data-ttu-id="76b92-120">このオプションは S モードのデバイスのロックを解除します。</span><span class="sxs-lookup"><span data-stu-id="76b92-120">This option will unlock the device from S mode</span></span>|





