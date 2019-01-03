---
title: managedDeviceModelsAndManufacturers リソースの種類
description: モデルと、アカウントで管理されているデバイスのメーカーの meatadata
author: tfitzmac
ms.openlocfilehash: 42611b0c14aa583d2871d97b66ce116a0b835268
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27352935"
---
# <a name="manageddevicemodelsandmanufacturers-resource-type"></a><span data-ttu-id="8910d-103">managedDeviceModelsAndManufacturers リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8910d-103">managedDeviceModelsAndManufacturers resource type</span></span>

> <span data-ttu-id="8910d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8910d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8910d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8910d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8910d-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8910d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8910d-107">モデルと、アカウントで管理されているデバイスのメーカーの meatadata</span><span class="sxs-lookup"><span data-stu-id="8910d-107">Models and Manufactures meatadata for managed devices in the account</span></span>
## <a name="properties"></a><span data-ttu-id="8910d-108">Properties</span><span class="sxs-lookup"><span data-stu-id="8910d-108">Properties</span></span>
|<span data-ttu-id="8910d-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8910d-109">Property</span></span>|<span data-ttu-id="8910d-110">種類</span><span class="sxs-lookup"><span data-stu-id="8910d-110">Type</span></span>|<span data-ttu-id="8910d-111">説明</span><span class="sxs-lookup"><span data-stu-id="8910d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8910d-112">deviceModels</span><span class="sxs-lookup"><span data-stu-id="8910d-112">deviceModels</span></span>|<span data-ttu-id="8910d-113">String コレクション</span><span class="sxs-lookup"><span data-stu-id="8910d-113">String collection</span></span>|<span data-ttu-id="8910d-114">アカウントで管理されているデバイスのモデルの一覧</span><span class="sxs-lookup"><span data-stu-id="8910d-114">List of Models for managed devices in the account</span></span>|
|<span data-ttu-id="8910d-115">deviceManufacturers</span><span class="sxs-lookup"><span data-stu-id="8910d-115">deviceManufacturers</span></span>|<span data-ttu-id="8910d-116">String コレクション</span><span class="sxs-lookup"><span data-stu-id="8910d-116">String collection</span></span>|<span data-ttu-id="8910d-117">アカウントで管理されているデバイスの製造元の一覧</span><span class="sxs-lookup"><span data-stu-id="8910d-117">List of Manufactures for managed devices in the account</span></span>|

## <a name="relationships"></a><span data-ttu-id="8910d-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8910d-118">Relationships</span></span>
<span data-ttu-id="8910d-119">なし</span><span class="sxs-lookup"><span data-stu-id="8910d-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8910d-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8910d-120">JSON Representation</span></span>
<span data-ttu-id="8910d-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8910d-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedDeviceModelsAndManufacturers"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceModelsAndManufacturers",
  "deviceModels": [
    "String"
  ],
  "deviceManufacturers": [
    "String"
  ]
}
```




