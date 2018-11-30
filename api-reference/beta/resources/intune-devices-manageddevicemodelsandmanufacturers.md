---
title: managedDeviceModelsAndManufacturers リソースの種類
description: モデルと、アカウントで管理されているデバイスのメーカーの meatadata
ms.openlocfilehash: c61026a6caa097e01e09a4343dd54f769c743460
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074277"
---
# <a name="manageddevicemodelsandmanufacturers-resource-type"></a><span data-ttu-id="a4ca3-103">managedDeviceModelsAndManufacturers リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a4ca3-103">managedDeviceModelsAndManufacturers resource type</span></span>

> <span data-ttu-id="a4ca3-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a4ca3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a4ca3-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a4ca3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a4ca3-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a4ca3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a4ca3-107">モデルと、アカウントで管理されているデバイスのメーカーの meatadata</span><span class="sxs-lookup"><span data-stu-id="a4ca3-107">Models and Manufactures meatadata for managed devices in the account</span></span>
## <a name="properties"></a><span data-ttu-id="a4ca3-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a4ca3-108">Properties</span></span>
|<span data-ttu-id="a4ca3-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a4ca3-109">Property</span></span>|<span data-ttu-id="a4ca3-110">型</span><span class="sxs-lookup"><span data-stu-id="a4ca3-110">Type</span></span>|<span data-ttu-id="a4ca3-111">説明</span><span class="sxs-lookup"><span data-stu-id="a4ca3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4ca3-112">deviceModels</span><span class="sxs-lookup"><span data-stu-id="a4ca3-112">deviceModels</span></span>|<span data-ttu-id="a4ca3-113">String コレクション</span><span class="sxs-lookup"><span data-stu-id="a4ca3-113">String collection</span></span>|<span data-ttu-id="a4ca3-114">アカウントで管理されているデバイスのモデルの一覧</span><span class="sxs-lookup"><span data-stu-id="a4ca3-114">List of Models for managed devices in the account</span></span>|
|<span data-ttu-id="a4ca3-115">deviceManufacturers</span><span class="sxs-lookup"><span data-stu-id="a4ca3-115">deviceManufacturers</span></span>|<span data-ttu-id="a4ca3-116">String コレクション</span><span class="sxs-lookup"><span data-stu-id="a4ca3-116">String collection</span></span>|<span data-ttu-id="a4ca3-117">アカウントで管理されているデバイスの製造元の一覧</span><span class="sxs-lookup"><span data-stu-id="a4ca3-117">List of Manufactures for managed devices in the account</span></span>|

## <a name="relationships"></a><span data-ttu-id="a4ca3-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a4ca3-118">Relationships</span></span>
<span data-ttu-id="a4ca3-119">なし</span><span class="sxs-lookup"><span data-stu-id="a4ca3-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a4ca3-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a4ca3-120">JSON Representation</span></span>
<span data-ttu-id="a4ca3-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a4ca3-121">Here is a JSON representation of the resource.</span></span>
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





