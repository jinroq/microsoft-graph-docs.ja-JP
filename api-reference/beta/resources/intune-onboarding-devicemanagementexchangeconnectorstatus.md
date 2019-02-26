---
title: deviceManagementExchangeConnectorStatus 列挙型
description: Exchange Connector の現在の状態。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: acfb4bccf0cbf9a2fc7b1074c119ac2f9c74855f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30149813"
---
# <a name="devicemanagementexchangeconnectorstatus-enum-type"></a><span data-ttu-id="8cc7c-103">deviceManagementExchangeConnectorStatus 列挙型</span><span class="sxs-lookup"><span data-stu-id="8cc7c-103">deviceManagementExchangeConnectorStatus enum type</span></span>

> <span data-ttu-id="8cc7c-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8cc7c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8cc7c-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8cc7c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8cc7c-106">Exchange Connector の現在の状態。</span><span class="sxs-lookup"><span data-stu-id="8cc7c-106">The current status of the Exchange Connector.</span></span>

## <a name="members"></a><span data-ttu-id="8cc7c-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="8cc7c-107">Members</span></span>
|<span data-ttu-id="8cc7c-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="8cc7c-108">Member</span></span>|<span data-ttu-id="8cc7c-109">値</span><span class="sxs-lookup"><span data-stu-id="8cc7c-109">Value</span></span>|<span data-ttu-id="8cc7c-110">説明</span><span class="sxs-lookup"><span data-stu-id="8cc7c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8cc7c-111">none</span><span class="sxs-lookup"><span data-stu-id="8cc7c-111">none</span></span>|<span data-ttu-id="8cc7c-112">.0</span><span class="sxs-lookup"><span data-stu-id="8cc7c-112">0</span></span>|<span data-ttu-id="8cc7c-113">コネクタが存在しません。</span><span class="sxs-lookup"><span data-stu-id="8cc7c-113">No Connector exists.</span></span>|
|<span data-ttu-id="8cc7c-114">connectionpending</span><span class="sxs-lookup"><span data-stu-id="8cc7c-114">connectionPending</span></span>|<span data-ttu-id="8cc7c-115">1-d</span><span class="sxs-lookup"><span data-stu-id="8cc7c-115">1</span></span>|<span data-ttu-id="8cc7c-116">Exchange 環境への保留中の接続。</span><span class="sxs-lookup"><span data-stu-id="8cc7c-116">Pending Connection to the Exchange Environment.</span></span>|
|<span data-ttu-id="8cc7c-117">まし</span><span class="sxs-lookup"><span data-stu-id="8cc7c-117">connected</span></span>|<span data-ttu-id="8cc7c-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="8cc7c-118">2</span></span>|<span data-ttu-id="8cc7c-119">Exchange 環境に接続されている</span><span class="sxs-lookup"><span data-stu-id="8cc7c-119">Connected to the Exchange Environment</span></span>|
|<span data-ttu-id="8cc7c-120">外す</span><span class="sxs-lookup"><span data-stu-id="8cc7c-120">disconnected</span></span>|<span data-ttu-id="8cc7c-121">1/3</span><span class="sxs-lookup"><span data-stu-id="8cc7c-121">3</span></span>|<span data-ttu-id="8cc7c-122">Exchange 環境から切断されている</span><span class="sxs-lookup"><span data-stu-id="8cc7c-122">Disconnected from the Exchange Environment</span></span>|




