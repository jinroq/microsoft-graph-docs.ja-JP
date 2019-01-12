---
title: windowsManagementApp リソースの種類
description: Windows 管理アプリケーションのエンティティです。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 395148d4c870193d75f418d7dc30d2b2241bad01
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27913500"
---
# <a name="windowsmanagementapp-resource-type"></a><span data-ttu-id="3b5b3-103">windowsManagementApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3b5b3-103">windowsManagementApp resource type</span></span>

> <span data-ttu-id="3b5b3-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3b5b3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3b5b3-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3b5b3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3b5b3-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="3b5b3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3b5b3-107">Windows 管理アプリケーションのエンティティです。</span><span class="sxs-lookup"><span data-stu-id="3b5b3-107">Windows management app entity.</span></span>
## <a name="methods"></a><span data-ttu-id="3b5b3-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="3b5b3-108">Methods</span></span>
|<span data-ttu-id="3b5b3-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="3b5b3-109">Method</span></span>|<span data-ttu-id="3b5b3-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="3b5b3-110">Return Type</span></span>|<span data-ttu-id="3b5b3-111">説明</span><span class="sxs-lookup"><span data-stu-id="3b5b3-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3b5b3-112">WindowsManagementApp を取得します。</span><span class="sxs-lookup"><span data-stu-id="3b5b3-112">Get windowsManagementApp</span></span>](../api/intune-devices-windowsmanagementapp-get.md)|[<span data-ttu-id="3b5b3-113">windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="3b5b3-113">windowsManagementApp</span></span>](../resources/intune-devices-windowsmanagementapp.md)|<span data-ttu-id="3b5b3-114">[WindowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3b5b3-114">Read properties and relationships of the [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>|
|[<span data-ttu-id="3b5b3-115">WindowsManagementApp を更新します。</span><span class="sxs-lookup"><span data-stu-id="3b5b3-115">Update windowsManagementApp</span></span>](../api/intune-devices-windowsmanagementapp-update.md)|[<span data-ttu-id="3b5b3-116">windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="3b5b3-116">windowsManagementApp</span></span>](../resources/intune-devices-windowsmanagementapp.md)|<span data-ttu-id="3b5b3-117">[WindowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="3b5b3-117">Update the properties of a [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3b5b3-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3b5b3-118">Properties</span></span>
|<span data-ttu-id="3b5b3-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3b5b3-119">Property</span></span>|<span data-ttu-id="3b5b3-120">型</span><span class="sxs-lookup"><span data-stu-id="3b5b3-120">Type</span></span>|<span data-ttu-id="3b5b3-121">説明</span><span class="sxs-lookup"><span data-stu-id="3b5b3-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b5b3-122">ID</span><span class="sxs-lookup"><span data-stu-id="3b5b3-122">id</span></span>|<span data-ttu-id="3b5b3-123">String</span><span class="sxs-lookup"><span data-stu-id="3b5b3-123">String</span></span>|<span data-ttu-id="3b5b3-124">Windows 管理アプリケーションの一意の識別子</span><span class="sxs-lookup"><span data-stu-id="3b5b3-124">Unique Identifier for the Windows management app</span></span>|
|<span data-ttu-id="3b5b3-125">availableVersion</span><span class="sxs-lookup"><span data-stu-id="3b5b3-125">availableVersion</span></span>|<span data-ttu-id="3b5b3-126">String</span><span class="sxs-lookup"><span data-stu-id="3b5b3-126">String</span></span>|<span data-ttu-id="3b5b3-127">Windows 管理アプリケーションの使用可能なバージョンです。</span><span class="sxs-lookup"><span data-stu-id="3b5b3-127">Windows management app available version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3b5b3-128">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3b5b3-128">Relationships</span></span>
|<span data-ttu-id="3b5b3-129">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3b5b3-129">Relationship</span></span>|<span data-ttu-id="3b5b3-130">型</span><span class="sxs-lookup"><span data-stu-id="3b5b3-130">Type</span></span>|<span data-ttu-id="3b5b3-131">説明</span><span class="sxs-lookup"><span data-stu-id="3b5b3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b5b3-132">healthSummary</span><span class="sxs-lookup"><span data-stu-id="3b5b3-132">healthSummary</span></span>|[<span data-ttu-id="3b5b3-133">windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="3b5b3-133">windowsManagementAppHealthSummary</span></span>](../resources/intune-devices-windowsmanagementapphealthsummary.md)|<span data-ttu-id="3b5b3-134">Windows 管理アプリケーションの概要の状態です。</span><span class="sxs-lookup"><span data-stu-id="3b5b3-134">Health summary for Windows management app.</span></span>|
|<span data-ttu-id="3b5b3-135">healthStates</span><span class="sxs-lookup"><span data-stu-id="3b5b3-135">healthStates</span></span>|<span data-ttu-id="3b5b3-136">[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="3b5b3-136">[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) collection</span></span>|<span data-ttu-id="3b5b3-137">インストールされている Windows の管理アプリケーションの稼働状態の一覧です。</span><span class="sxs-lookup"><span data-stu-id="3b5b3-137">The list of health states for installed Windows management app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3b5b3-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3b5b3-138">JSON Representation</span></span>
<span data-ttu-id="3b5b3-139">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3b5b3-139">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsManagementApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsManagementApp",
  "id": "String (identifier)",
  "availableVersion": "String"
}
```





