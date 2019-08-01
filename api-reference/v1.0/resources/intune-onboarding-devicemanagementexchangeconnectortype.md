---
title: deviceManagementExchangeConnectorType 列挙型
description: Exchange Connector の種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: cff16857b9cd646db2da18c662447527173673e3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037437"
---
# <a name="devicemanagementexchangeconnectortype-enum-type"></a><span data-ttu-id="37f99-103">deviceManagementExchangeConnectorType 列挙型</span><span class="sxs-lookup"><span data-stu-id="37f99-103">deviceManagementExchangeConnectorType enum type</span></span>

> <span data-ttu-id="37f99-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="37f99-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37f99-105">Exchange Connector の種類。</span><span class="sxs-lookup"><span data-stu-id="37f99-105">The type of Exchange Connector.</span></span>

## <a name="members"></a><span data-ttu-id="37f99-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="37f99-106">Members</span></span>
|<span data-ttu-id="37f99-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="37f99-107">Member</span></span>|<span data-ttu-id="37f99-108">値</span><span class="sxs-lookup"><span data-stu-id="37f99-108">Value</span></span>|<span data-ttu-id="37f99-109">説明</span><span class="sxs-lookup"><span data-stu-id="37f99-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37f99-110">onPremises</span><span class="sxs-lookup"><span data-stu-id="37f99-110">onPremises</span></span>|<span data-ttu-id="37f99-111">.0</span><span class="sxs-lookup"><span data-stu-id="37f99-111">0</span></span>|<span data-ttu-id="37f99-112">オンプレミスの Exchange 環境に接続します。</span><span class="sxs-lookup"><span data-stu-id="37f99-112">Connects to on-premises Exchange Environment.</span></span>|
|<span data-ttu-id="37f99-113">さ</span><span class="sxs-lookup"><span data-stu-id="37f99-113">hosted</span></span>|<span data-ttu-id="37f99-114">1-d</span><span class="sxs-lookup"><span data-stu-id="37f99-114">1</span></span>|<span data-ttu-id="37f99-115">O365 マルチテナントの Exchange 環境に接続します。</span><span class="sxs-lookup"><span data-stu-id="37f99-115">Connects to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="37f99-116">serviceToService</span><span class="sxs-lookup"><span data-stu-id="37f99-116">serviceToService</span></span>|<span data-ttu-id="37f99-117">pbm-2</span><span class="sxs-lookup"><span data-stu-id="37f99-117">2</span></span>|<span data-ttu-id="37f99-118">Intune サービスが O365 マルチテナントの Exchange 環境に直接接続される</span><span class="sxs-lookup"><span data-stu-id="37f99-118">Intune Service connects directly to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="37f99-119">集中的</span><span class="sxs-lookup"><span data-stu-id="37f99-119">dedicated</span></span>|<span data-ttu-id="37f99-120">1/3</span><span class="sxs-lookup"><span data-stu-id="37f99-120">3</span></span>|<span data-ttu-id="37f99-121">O365 専用 Exchange 環境に接続します。</span><span class="sxs-lookup"><span data-stu-id="37f99-121">Connects to O365 Dedicated Exchange environment.</span></span>|



