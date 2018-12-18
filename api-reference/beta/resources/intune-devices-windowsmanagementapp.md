---
title: windowsManagementApp リソースの種類
description: Windows 管理アプリケーションのエンティティです。
author: tfitzmac
ms.openlocfilehash: 641538644dc313234e27b0f518a26d8a38c612b7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27346425"
---
# <a name="windowsmanagementapp-resource-type"></a><span data-ttu-id="8074a-103">windowsManagementApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8074a-103">windowsManagementApp resource type</span></span>

> <span data-ttu-id="8074a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8074a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8074a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8074a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8074a-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8074a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8074a-107">Windows 管理アプリケーションのエンティティです。</span><span class="sxs-lookup"><span data-stu-id="8074a-107">Windows management app entity.</span></span>
## <a name="methods"></a><span data-ttu-id="8074a-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="8074a-108">Methods</span></span>
|<span data-ttu-id="8074a-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="8074a-109">Method</span></span>|<span data-ttu-id="8074a-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="8074a-110">Return Type</span></span>|<span data-ttu-id="8074a-111">説明</span><span class="sxs-lookup"><span data-stu-id="8074a-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8074a-112">WindowsManagementApp を取得します。</span><span class="sxs-lookup"><span data-stu-id="8074a-112">Get windowsManagementApp</span></span>](../api/intune-devices-windowsmanagementapp-get.md)|[<span data-ttu-id="8074a-113">windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="8074a-113">windowsManagementApp</span></span>](../resources/intune-devices-windowsmanagementapp.md)|<span data-ttu-id="8074a-114">[WindowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8074a-114">Read properties and relationships of the [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>|
|[<span data-ttu-id="8074a-115">WindowsManagementApp を更新します。</span><span class="sxs-lookup"><span data-stu-id="8074a-115">Update windowsManagementApp</span></span>](../api/intune-devices-windowsmanagementapp-update.md)|[<span data-ttu-id="8074a-116">windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="8074a-116">windowsManagementApp</span></span>](../resources/intune-devices-windowsmanagementapp.md)|<span data-ttu-id="8074a-117">[WindowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="8074a-117">Update the properties of a [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8074a-118">Properties</span><span class="sxs-lookup"><span data-stu-id="8074a-118">Properties</span></span>
|<span data-ttu-id="8074a-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8074a-119">Property</span></span>|<span data-ttu-id="8074a-120">種類</span><span class="sxs-lookup"><span data-stu-id="8074a-120">Type</span></span>|<span data-ttu-id="8074a-121">説明</span><span class="sxs-lookup"><span data-stu-id="8074a-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8074a-122">ID</span><span class="sxs-lookup"><span data-stu-id="8074a-122">id</span></span>|<span data-ttu-id="8074a-123">String</span><span class="sxs-lookup"><span data-stu-id="8074a-123">String</span></span>|<span data-ttu-id="8074a-124">Windows 管理アプリケーションの一意の識別子</span><span class="sxs-lookup"><span data-stu-id="8074a-124">Unique Identifier for the Windows management app</span></span>|
|<span data-ttu-id="8074a-125">availableVersion</span><span class="sxs-lookup"><span data-stu-id="8074a-125">availableVersion</span></span>|<span data-ttu-id="8074a-126">String</span><span class="sxs-lookup"><span data-stu-id="8074a-126">String</span></span>|<span data-ttu-id="8074a-127">Windows 管理アプリケーションの使用可能なバージョンです。</span><span class="sxs-lookup"><span data-stu-id="8074a-127">Windows management app available version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8074a-128">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8074a-128">Relationships</span></span>
|<span data-ttu-id="8074a-129">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8074a-129">Relationship</span></span>|<span data-ttu-id="8074a-130">型</span><span class="sxs-lookup"><span data-stu-id="8074a-130">Type</span></span>|<span data-ttu-id="8074a-131">説明</span><span class="sxs-lookup"><span data-stu-id="8074a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8074a-132">healthSummary</span><span class="sxs-lookup"><span data-stu-id="8074a-132">healthSummary</span></span>|[<span data-ttu-id="8074a-133">windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="8074a-133">windowsManagementAppHealthSummary</span></span>](../resources/intune-devices-windowsmanagementapphealthsummary.md)|<span data-ttu-id="8074a-134">Windows 管理アプリケーションの概要の状態です。</span><span class="sxs-lookup"><span data-stu-id="8074a-134">Health summary for Windows management app.</span></span>|
|<span data-ttu-id="8074a-135">healthStates</span><span class="sxs-lookup"><span data-stu-id="8074a-135">healthStates</span></span>|<span data-ttu-id="8074a-136">[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="8074a-136">[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) collection</span></span>|<span data-ttu-id="8074a-137">インストールされている Windows の管理アプリケーションの稼働状態の一覧です。</span><span class="sxs-lookup"><span data-stu-id="8074a-137">The list of health states for installed Windows management app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8074a-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8074a-138">JSON Representation</span></span>
<span data-ttu-id="8074a-139">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8074a-139">Here is a JSON representation of the resource.</span></span>
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





