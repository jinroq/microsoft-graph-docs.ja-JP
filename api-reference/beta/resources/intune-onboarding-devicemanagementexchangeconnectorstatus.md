---
title: deviceManagementExchangeConnectorStatus 列挙型
description: Exchange Connector の現在の状態。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 87b45805c7beb15147cf90f8c2f6bef1b82ecb7f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566620"
---
# <a name="devicemanagementexchangeconnectorstatus-enum-type"></a><span data-ttu-id="817c4-103">deviceManagementExchangeConnectorStatus 列挙型</span><span class="sxs-lookup"><span data-stu-id="817c4-103">deviceManagementExchangeConnectorStatus enum type</span></span>

> <span data-ttu-id="817c4-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="817c4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="817c4-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="817c4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="817c4-106">Exchange Connector の現在の状態。</span><span class="sxs-lookup"><span data-stu-id="817c4-106">The current status of the Exchange Connector.</span></span>

## <a name="members"></a><span data-ttu-id="817c4-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="817c4-107">Members</span></span>
|<span data-ttu-id="817c4-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="817c4-108">Member</span></span>|<span data-ttu-id="817c4-109">値</span><span class="sxs-lookup"><span data-stu-id="817c4-109">Value</span></span>|<span data-ttu-id="817c4-110">説明</span><span class="sxs-lookup"><span data-stu-id="817c4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="817c4-111">なし</span><span class="sxs-lookup"><span data-stu-id="817c4-111">none</span></span>|<span data-ttu-id="817c4-112">.0</span><span class="sxs-lookup"><span data-stu-id="817c4-112">0</span></span>|<span data-ttu-id="817c4-113">コネクタが存在しません。</span><span class="sxs-lookup"><span data-stu-id="817c4-113">No Connector exists.</span></span>|
|<span data-ttu-id="817c4-114">connectionpending</span><span class="sxs-lookup"><span data-stu-id="817c4-114">connectionPending</span></span>|<span data-ttu-id="817c4-115">1 </span><span class="sxs-lookup"><span data-stu-id="817c4-115">1</span></span>|<span data-ttu-id="817c4-116">Exchange 環境への保留中の接続。</span><span class="sxs-lookup"><span data-stu-id="817c4-116">Pending Connection to the Exchange Environment.</span></span>|
|<span data-ttu-id="817c4-117">まし</span><span class="sxs-lookup"><span data-stu-id="817c4-117">connected</span></span>|<span data-ttu-id="817c4-118">2 </span><span class="sxs-lookup"><span data-stu-id="817c4-118">2</span></span>|<span data-ttu-id="817c4-119">Exchange 環境に接続されている</span><span class="sxs-lookup"><span data-stu-id="817c4-119">Connected to the Exchange Environment</span></span>|
|<span data-ttu-id="817c4-120">外す</span><span class="sxs-lookup"><span data-stu-id="817c4-120">disconnected</span></span>|<span data-ttu-id="817c4-121">3 </span><span class="sxs-lookup"><span data-stu-id="817c4-121">3</span></span>|<span data-ttu-id="817c4-122">Exchange 環境から切断されている</span><span class="sxs-lookup"><span data-stu-id="817c4-122">Disconnected from the Exchange Environment</span></span>|





