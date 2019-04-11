---
title: deviceManagementExchangeConnectorSyncType 列挙型
description: 要求された Exchange Connector の同期の種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: abb2a74c27df76a75971a2e2205698002bc3d8ab
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31798461"
---
# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a><span data-ttu-id="bcc65-103">deviceManagementExchangeConnectorSyncType 列挙型</span><span class="sxs-lookup"><span data-stu-id="bcc65-103">deviceManagementExchangeConnectorSyncType enum type</span></span>

> <span data-ttu-id="bcc65-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bcc65-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bcc65-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bcc65-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bcc65-106">要求された Exchange Connector の同期の種類。</span><span class="sxs-lookup"><span data-stu-id="bcc65-106">The type of Exchange Connector sync requested.</span></span>

## <a name="members"></a><span data-ttu-id="bcc65-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="bcc65-107">Members</span></span>
|<span data-ttu-id="bcc65-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="bcc65-108">Member</span></span>|<span data-ttu-id="bcc65-109">値</span><span class="sxs-lookup"><span data-stu-id="bcc65-109">Value</span></span>|<span data-ttu-id="bcc65-110">説明</span><span class="sxs-lookup"><span data-stu-id="bcc65-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bcc65-111">fullSync</span><span class="sxs-lookup"><span data-stu-id="bcc65-111">fullSync</span></span>|<span data-ttu-id="bcc65-112">.0</span><span class="sxs-lookup"><span data-stu-id="bcc65-112">0</span></span>|<span data-ttu-id="bcc65-113">Exchange のすべてのデバイスを検出します。</span><span class="sxs-lookup"><span data-stu-id="bcc65-113">Discover all the device in Exchange.</span></span>|
|<span data-ttu-id="bcc65-114">deltasync]</span><span class="sxs-lookup"><span data-stu-id="bcc65-114">deltaSync</span></span>|<span data-ttu-id="bcc65-115">1-d</span><span class="sxs-lookup"><span data-stu-id="bcc65-115">1</span></span>|<span data-ttu-id="bcc65-116">[差分同期] ウィンドウで更新された Exchange のデバイスのみを検出します。</span><span class="sxs-lookup"><span data-stu-id="bcc65-116">Discover only the device in Exchange which have updated during the delta sync window.</span></span>|





