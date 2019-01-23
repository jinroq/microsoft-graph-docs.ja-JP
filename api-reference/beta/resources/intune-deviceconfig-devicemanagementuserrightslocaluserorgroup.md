---
title: deviceManagementUserRightsLocalUserOrGroup リソースの種類
description: ローカル ユーザーまたはグループのユーザー権利の設定の使用に関する情報を表します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8a2cc0ff5b9e054398e7878b7d99619b59d109a4
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422062"
---
# <a name="devicemanagementuserrightslocaluserorgroup-resource-type"></a><span data-ttu-id="6522f-103">deviceManagementUserRightsLocalUserOrGroup リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6522f-103">deviceManagementUserRightsLocalUserOrGroup resource type</span></span>

> <span data-ttu-id="6522f-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6522f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6522f-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6522f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6522f-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6522f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6522f-107">ローカル ユーザーまたはグループのユーザー権利の設定の使用に関する情報を表します。</span><span class="sxs-lookup"><span data-stu-id="6522f-107">Represents information for a local user or group used for user rights setting.</span></span>

## <a name="properties"></a><span data-ttu-id="6522f-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6522f-108">Properties</span></span>
|<span data-ttu-id="6522f-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6522f-109">Property</span></span>|<span data-ttu-id="6522f-110">型</span><span class="sxs-lookup"><span data-stu-id="6522f-110">Type</span></span>|<span data-ttu-id="6522f-111">説明</span><span class="sxs-lookup"><span data-stu-id="6522f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6522f-112">name</span><span class="sxs-lookup"><span data-stu-id="6522f-112">name</span></span>|<span data-ttu-id="6522f-113">String</span><span class="sxs-lookup"><span data-stu-id="6522f-113">String</span></span>|<span data-ttu-id="6522f-114">ローカル ユーザーまたはグループの名前です。</span><span class="sxs-lookup"><span data-stu-id="6522f-114">The name of this local user or group.</span></span>|
|<span data-ttu-id="6522f-115">説明</span><span class="sxs-lookup"><span data-stu-id="6522f-115">description</span></span>|<span data-ttu-id="6522f-116">String</span><span class="sxs-lookup"><span data-stu-id="6522f-116">String</span></span>|<span data-ttu-id="6522f-117">ローカル ユーザーまたはグループの管理の説明です。</span><span class="sxs-lookup"><span data-stu-id="6522f-117">Admin’s description of this local user or group.</span></span>|
|<span data-ttu-id="6522f-118">securityIdentifier</span><span class="sxs-lookup"><span data-stu-id="6522f-118">securityIdentifier</span></span>|<span data-ttu-id="6522f-119">String</span><span class="sxs-lookup"><span data-stu-id="6522f-119">String</span></span>|<span data-ttu-id="6522f-120">このローカル ユーザーまたはグループのセキュリティ識別子 (例: \* S-1-5-32-544)。</span><span class="sxs-lookup"><span data-stu-id="6522f-120">The security identifier of this local user or group (e.g. \*S-1-5-32-544).</span></span>|

## <a name="relationships"></a><span data-ttu-id="6522f-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6522f-121">Relationships</span></span>
<span data-ttu-id="6522f-122">なし</span><span class="sxs-lookup"><span data-stu-id="6522f-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6522f-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6522f-123">JSON Representation</span></span>
<span data-ttu-id="6522f-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6522f-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
  "name": "String",
  "description": "String",
  "securityIdentifier": "String"
}
```




