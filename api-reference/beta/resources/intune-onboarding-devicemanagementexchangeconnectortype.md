---
title: deviceManagementExchangeConnectorType 列挙型
description: Exchange Connector の種類。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 36cdb3ff0490ea1b2d446beb587ef3a828e638ed
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34993054"
---
# <a name="devicemanagementexchangeconnectortype-enum-type"></a><span data-ttu-id="a4051-103">deviceManagementExchangeConnectorType 列挙型</span><span class="sxs-lookup"><span data-stu-id="a4051-103">deviceManagementExchangeConnectorType enum type</span></span>

> <span data-ttu-id="a4051-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a4051-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a4051-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a4051-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4051-106">Exchange Connector の種類。</span><span class="sxs-lookup"><span data-stu-id="a4051-106">The type of Exchange Connector.</span></span>

## <a name="members"></a><span data-ttu-id="a4051-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="a4051-107">Members</span></span>
|<span data-ttu-id="a4051-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="a4051-108">Member</span></span>|<span data-ttu-id="a4051-109">値</span><span class="sxs-lookup"><span data-stu-id="a4051-109">Value</span></span>|<span data-ttu-id="a4051-110">説明</span><span class="sxs-lookup"><span data-stu-id="a4051-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4051-111">onPremises</span><span class="sxs-lookup"><span data-stu-id="a4051-111">onPremises</span></span>|<span data-ttu-id="a4051-112">.0</span><span class="sxs-lookup"><span data-stu-id="a4051-112">0</span></span>|<span data-ttu-id="a4051-113">オンプレミスの Exchange 環境に接続します。</span><span class="sxs-lookup"><span data-stu-id="a4051-113">Connects to on-premises Exchange Environment.</span></span>|
|<span data-ttu-id="a4051-114">さ</span><span class="sxs-lookup"><span data-stu-id="a4051-114">hosted</span></span>|<span data-ttu-id="a4051-115">1-d</span><span class="sxs-lookup"><span data-stu-id="a4051-115">1</span></span>|<span data-ttu-id="a4051-116">O365 マルチテナントの Exchange 環境に接続します。</span><span class="sxs-lookup"><span data-stu-id="a4051-116">Connects to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="a4051-117">serviceToService</span><span class="sxs-lookup"><span data-stu-id="a4051-117">serviceToService</span></span>|<span data-ttu-id="a4051-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="a4051-118">2</span></span>|<span data-ttu-id="a4051-119">Intune サービスが O365 マルチテナントの Exchange 環境に直接接続される</span><span class="sxs-lookup"><span data-stu-id="a4051-119">Intune Service connects directly to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="a4051-120">集中的</span><span class="sxs-lookup"><span data-stu-id="a4051-120">dedicated</span></span>|<span data-ttu-id="a4051-121">1/3</span><span class="sxs-lookup"><span data-stu-id="a4051-121">3</span></span>|<span data-ttu-id="a4051-122">O365 専用 Exchange 環境に接続します。</span><span class="sxs-lookup"><span data-stu-id="a4051-122">Connects to O365 Dedicated Exchange environment.</span></span>|





