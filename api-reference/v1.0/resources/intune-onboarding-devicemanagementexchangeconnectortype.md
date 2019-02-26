---
title: deviceManagementExchangeConnectorType 列挙型
description: Exchange Connector の種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c358832db83e5f5b3e1fb0f5457f480d21ded996
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30263561"
---
# <a name="devicemanagementexchangeconnectortype-enum-type"></a><span data-ttu-id="4a6b7-103">deviceManagementExchangeConnectorType 列挙型</span><span class="sxs-lookup"><span data-stu-id="4a6b7-103">deviceManagementExchangeConnectorType enum type</span></span>

> <span data-ttu-id="4a6b7-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4a6b7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a6b7-105">Exchange Connector の種類。</span><span class="sxs-lookup"><span data-stu-id="4a6b7-105">The type of Exchange Connector.</span></span>

## <a name="members"></a><span data-ttu-id="4a6b7-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="4a6b7-106">Members</span></span>
|<span data-ttu-id="4a6b7-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="4a6b7-107">Member</span></span>|<span data-ttu-id="4a6b7-108">値</span><span class="sxs-lookup"><span data-stu-id="4a6b7-108">Value</span></span>|<span data-ttu-id="4a6b7-109">説明</span><span class="sxs-lookup"><span data-stu-id="4a6b7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a6b7-110">onPremises</span><span class="sxs-lookup"><span data-stu-id="4a6b7-110">onPremises</span></span>|<span data-ttu-id="4a6b7-111">.0</span><span class="sxs-lookup"><span data-stu-id="4a6b7-111">0</span></span>|<span data-ttu-id="4a6b7-112">オンプレミスの Exchange 環境に接続します。</span><span class="sxs-lookup"><span data-stu-id="4a6b7-112">Connects to on-premises Exchange Environment.</span></span>|
|<span data-ttu-id="4a6b7-113">さ</span><span class="sxs-lookup"><span data-stu-id="4a6b7-113">hosted</span></span>|<span data-ttu-id="4a6b7-114">1-d</span><span class="sxs-lookup"><span data-stu-id="4a6b7-114">1</span></span>|<span data-ttu-id="4a6b7-115">O365 マルチテナントの Exchange 環境に接続します。</span><span class="sxs-lookup"><span data-stu-id="4a6b7-115">Connects to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="4a6b7-116">servicetoservice</span><span class="sxs-lookup"><span data-stu-id="4a6b7-116">serviceToService</span></span>|<span data-ttu-id="4a6b7-117">pbm-2</span><span class="sxs-lookup"><span data-stu-id="4a6b7-117">2</span></span>|<span data-ttu-id="4a6b7-118">Intune サービスが O365 マルチテナントの Exchange 環境に直接接続される</span><span class="sxs-lookup"><span data-stu-id="4a6b7-118">Intune Service connects directly to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="4a6b7-119">集中的</span><span class="sxs-lookup"><span data-stu-id="4a6b7-119">dedicated</span></span>|<span data-ttu-id="4a6b7-120">1/3</span><span class="sxs-lookup"><span data-stu-id="4a6b7-120">3</span></span>|<span data-ttu-id="4a6b7-121">O365 専用 Exchange 環境に接続します。</span><span class="sxs-lookup"><span data-stu-id="4a6b7-121">Connects to O365 Dedicated Exchange environment.</span></span>|



