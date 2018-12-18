---
title: windowsSModeConfiguration 列挙型
description: S モードを構成するのには使用可能なオプションのロックを解除します。
author: tfitzmac
ms.openlocfilehash: 592eb58a13d1f78caadb5b46acac5b43e6c97384
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344703"
---
# <a name="windowssmodeconfiguration-enum-type"></a><span data-ttu-id="c270e-103">windowsSModeConfiguration 列挙型</span><span class="sxs-lookup"><span data-stu-id="c270e-103">windowsSModeConfiguration enum type</span></span>

> <span data-ttu-id="c270e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c270e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c270e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c270e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c270e-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c270e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c270e-107">S モードを構成するのには使用可能なオプションのロックを解除します。</span><span class="sxs-lookup"><span data-stu-id="c270e-107">The possible options to configure S mode unlock</span></span>
## <a name="members"></a><span data-ttu-id="c270e-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="c270e-108">Members</span></span>
|<span data-ttu-id="c270e-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="c270e-109">Member</span></span>|<span data-ttu-id="c270e-110">値</span><span class="sxs-lookup"><span data-stu-id="c270e-110">Value</span></span>|<span data-ttu-id="c270e-111">説明</span><span class="sxs-lookup"><span data-stu-id="c270e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c270e-112">noRestriction</span><span class="sxs-lookup"><span data-stu-id="c270e-112">noRestriction</span></span>|<span data-ttu-id="c270e-113">0</span><span class="sxs-lookup"><span data-stu-id="c270e-113">0</span></span>|<span data-ttu-id="c270e-114">このオプションでは、S モードの既定のロックを解除するすべての制限を削除します。</span><span class="sxs-lookup"><span data-stu-id="c270e-114">This option will remove all restrictions to unlock S mode - default</span></span>|
|<span data-ttu-id="c270e-115">ブロック</span><span class="sxs-lookup"><span data-stu-id="c270e-115">block</span></span>|<span data-ttu-id="c270e-116">1</span><span class="sxs-lookup"><span data-stu-id="c270e-116">1</span></span>|<span data-ttu-id="c270e-117">このオプションは S モードのデバイスのロックを解除するユーザーをブロックします。</span><span class="sxs-lookup"><span data-stu-id="c270e-117">This option will block the user to unlock the device from S mode</span></span>|
|<span data-ttu-id="c270e-118">ロックを解除します。</span><span class="sxs-lookup"><span data-stu-id="c270e-118">unlock</span></span>|<span data-ttu-id="c270e-119">2</span><span class="sxs-lookup"><span data-stu-id="c270e-119">2</span></span>|<span data-ttu-id="c270e-120">このオプションは S モードのデバイスのロックを解除します。</span><span class="sxs-lookup"><span data-stu-id="c270e-120">This option will unlock the device from S mode</span></span>|





