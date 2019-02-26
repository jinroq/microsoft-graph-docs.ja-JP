---
title: deviceManagementExchangeConnectorSyncType 列挙型
description: 要求された Exchange Connector の同期の種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 47021a0a071995261f218cd4080026ababa33e0f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166599"
---
# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a><span data-ttu-id="26700-103">deviceManagementExchangeConnectorSyncType 列挙型</span><span class="sxs-lookup"><span data-stu-id="26700-103">deviceManagementExchangeConnectorSyncType enum type</span></span>

> <span data-ttu-id="26700-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="26700-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="26700-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="26700-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26700-106">要求された Exchange Connector の同期の種類。</span><span class="sxs-lookup"><span data-stu-id="26700-106">The type of Exchange Connector sync requested.</span></span>

## <a name="members"></a><span data-ttu-id="26700-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="26700-107">Members</span></span>
|<span data-ttu-id="26700-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="26700-108">Member</span></span>|<span data-ttu-id="26700-109">値</span><span class="sxs-lookup"><span data-stu-id="26700-109">Value</span></span>|<span data-ttu-id="26700-110">説明</span><span class="sxs-lookup"><span data-stu-id="26700-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26700-111">fullSync</span><span class="sxs-lookup"><span data-stu-id="26700-111">fullSync</span></span>|<span data-ttu-id="26700-112">.0</span><span class="sxs-lookup"><span data-stu-id="26700-112">0</span></span>|<span data-ttu-id="26700-113">Exchange のすべてのデバイスを検出します。</span><span class="sxs-lookup"><span data-stu-id="26700-113">Discover all the device in Exchange.</span></span>|
|<span data-ttu-id="26700-114">deltasync]</span><span class="sxs-lookup"><span data-stu-id="26700-114">deltaSync</span></span>|<span data-ttu-id="26700-115">1-d</span><span class="sxs-lookup"><span data-stu-id="26700-115">1</span></span>|<span data-ttu-id="26700-116">[差分同期] ウィンドウで更新された Exchange のデバイスのみを検出します。</span><span class="sxs-lookup"><span data-stu-id="26700-116">Discover only the device in Exchange which have updated during the delta sync window.</span></span>|




