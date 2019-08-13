---
title: deviceManagementExchangeConnectorSyncType 列挙型
description: 要求された Exchange Connector の同期の種類。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: f68277b2eeb7aea123ee843a0b602d11123cbd04
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369452"
---
# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a><span data-ttu-id="f960b-103">deviceManagementExchangeConnectorSyncType 列挙型</span><span class="sxs-lookup"><span data-stu-id="f960b-103">deviceManagementExchangeConnectorSyncType enum type</span></span>

> <span data-ttu-id="f960b-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f960b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f960b-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f960b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f960b-106">要求された Exchange Connector の同期の種類。</span><span class="sxs-lookup"><span data-stu-id="f960b-106">The type of Exchange Connector sync requested.</span></span>

## <a name="members"></a><span data-ttu-id="f960b-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="f960b-107">Members</span></span>
|<span data-ttu-id="f960b-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="f960b-108">Member</span></span>|<span data-ttu-id="f960b-109">値</span><span class="sxs-lookup"><span data-stu-id="f960b-109">Value</span></span>|<span data-ttu-id="f960b-110">説明</span><span class="sxs-lookup"><span data-stu-id="f960b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f960b-111">fullSync</span><span class="sxs-lookup"><span data-stu-id="f960b-111">fullSync</span></span>|<span data-ttu-id="f960b-112">.0</span><span class="sxs-lookup"><span data-stu-id="f960b-112">0</span></span>|<span data-ttu-id="f960b-113">Exchange のすべてのデバイスを検出します。</span><span class="sxs-lookup"><span data-stu-id="f960b-113">Discover all the device in Exchange.</span></span>|
|<span data-ttu-id="f960b-114">Deltasync]</span><span class="sxs-lookup"><span data-stu-id="f960b-114">deltaSync</span></span>|<span data-ttu-id="f960b-115">1-d</span><span class="sxs-lookup"><span data-stu-id="f960b-115">1</span></span>|<span data-ttu-id="f960b-116">[差分同期] ウィンドウで更新された Exchange のデバイスのみを検出します。</span><span class="sxs-lookup"><span data-stu-id="f960b-116">Discover only the device in Exchange which have updated during the delta sync window.</span></span>|



