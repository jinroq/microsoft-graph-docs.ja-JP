---
title: deviceManagementExchangeConnectorType 列挙型
description: Exchange Connector の種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8742a146f1183376424678f070b902eb052df5ac
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30150436"
---
# <a name="devicemanagementexchangeconnectortype-enum-type"></a><span data-ttu-id="8a6e2-103">deviceManagementExchangeConnectorType 列挙型</span><span class="sxs-lookup"><span data-stu-id="8a6e2-103">deviceManagementExchangeConnectorType enum type</span></span>

> <span data-ttu-id="8a6e2-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8a6e2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8a6e2-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8a6e2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8a6e2-106">Exchange Connector の種類。</span><span class="sxs-lookup"><span data-stu-id="8a6e2-106">The type of Exchange Connector.</span></span>

## <a name="members"></a><span data-ttu-id="8a6e2-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="8a6e2-107">Members</span></span>
|<span data-ttu-id="8a6e2-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="8a6e2-108">Member</span></span>|<span data-ttu-id="8a6e2-109">値</span><span class="sxs-lookup"><span data-stu-id="8a6e2-109">Value</span></span>|<span data-ttu-id="8a6e2-110">説明</span><span class="sxs-lookup"><span data-stu-id="8a6e2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a6e2-111">onPremises</span><span class="sxs-lookup"><span data-stu-id="8a6e2-111">onPremises</span></span>|<span data-ttu-id="8a6e2-112">.0</span><span class="sxs-lookup"><span data-stu-id="8a6e2-112">0</span></span>|<span data-ttu-id="8a6e2-113">オンプレミスの Exchange 環境に接続します。</span><span class="sxs-lookup"><span data-stu-id="8a6e2-113">Connects to on-premises Exchange Environment.</span></span>|
|<span data-ttu-id="8a6e2-114">さ</span><span class="sxs-lookup"><span data-stu-id="8a6e2-114">hosted</span></span>|<span data-ttu-id="8a6e2-115">1-d</span><span class="sxs-lookup"><span data-stu-id="8a6e2-115">1</span></span>|<span data-ttu-id="8a6e2-116">O365 マルチテナントの Exchange 環境に接続します。</span><span class="sxs-lookup"><span data-stu-id="8a6e2-116">Connects to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="8a6e2-117">servicetoservice</span><span class="sxs-lookup"><span data-stu-id="8a6e2-117">serviceToService</span></span>|<span data-ttu-id="8a6e2-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="8a6e2-118">2</span></span>|<span data-ttu-id="8a6e2-119">Intune サービスが O365 マルチテナントの Exchange 環境に直接接続される</span><span class="sxs-lookup"><span data-stu-id="8a6e2-119">Intune Service connects directly to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="8a6e2-120">集中的</span><span class="sxs-lookup"><span data-stu-id="8a6e2-120">dedicated</span></span>|<span data-ttu-id="8a6e2-121">1/3</span><span class="sxs-lookup"><span data-stu-id="8a6e2-121">3</span></span>|<span data-ttu-id="8a6e2-122">O365 専用 Exchange 環境に接続します。</span><span class="sxs-lookup"><span data-stu-id="8a6e2-122">Connects to O365 Dedicated Exchange environment.</span></span>|




