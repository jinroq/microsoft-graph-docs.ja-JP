---
title: deviceManagementExchangeConnectorStatus 列挙型
description: Exchange Connector の現在の状態。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e6ba563f451a7b5dacf938411912e3623fe400f7
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34993019"
---
# <a name="devicemanagementexchangeconnectorstatus-enum-type"></a><span data-ttu-id="8bc24-103">deviceManagementExchangeConnectorStatus 列挙型</span><span class="sxs-lookup"><span data-stu-id="8bc24-103">deviceManagementExchangeConnectorStatus enum type</span></span>

> <span data-ttu-id="8bc24-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8bc24-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8bc24-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8bc24-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8bc24-106">Exchange Connector の現在の状態。</span><span class="sxs-lookup"><span data-stu-id="8bc24-106">The current status of the Exchange Connector.</span></span>

## <a name="members"></a><span data-ttu-id="8bc24-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="8bc24-107">Members</span></span>
|<span data-ttu-id="8bc24-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="8bc24-108">Member</span></span>|<span data-ttu-id="8bc24-109">値</span><span class="sxs-lookup"><span data-stu-id="8bc24-109">Value</span></span>|<span data-ttu-id="8bc24-110">説明</span><span class="sxs-lookup"><span data-stu-id="8bc24-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8bc24-111">none</span><span class="sxs-lookup"><span data-stu-id="8bc24-111">none</span></span>|<span data-ttu-id="8bc24-112">.0</span><span class="sxs-lookup"><span data-stu-id="8bc24-112">0</span></span>|<span data-ttu-id="8bc24-113">コネクタが存在しません。</span><span class="sxs-lookup"><span data-stu-id="8bc24-113">No Connector exists.</span></span>|
|<span data-ttu-id="8bc24-114">connectionPending</span><span class="sxs-lookup"><span data-stu-id="8bc24-114">connectionPending</span></span>|<span data-ttu-id="8bc24-115">1-d</span><span class="sxs-lookup"><span data-stu-id="8bc24-115">1</span></span>|<span data-ttu-id="8bc24-116">Exchange 環境への保留中の接続。</span><span class="sxs-lookup"><span data-stu-id="8bc24-116">Pending Connection to the Exchange Environment.</span></span>|
|<span data-ttu-id="8bc24-117">まし</span><span class="sxs-lookup"><span data-stu-id="8bc24-117">connected</span></span>|<span data-ttu-id="8bc24-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="8bc24-118">2</span></span>|<span data-ttu-id="8bc24-119">Exchange 環境に接続されている</span><span class="sxs-lookup"><span data-stu-id="8bc24-119">Connected to the Exchange Environment</span></span>|
|<span data-ttu-id="8bc24-120">外す</span><span class="sxs-lookup"><span data-stu-id="8bc24-120">disconnected</span></span>|<span data-ttu-id="8bc24-121">1/3</span><span class="sxs-lookup"><span data-stu-id="8bc24-121">3</span></span>|<span data-ttu-id="8bc24-122">Exchange 環境から切断されている</span><span class="sxs-lookup"><span data-stu-id="8bc24-122">Disconnected from the Exchange Environment</span></span>|





