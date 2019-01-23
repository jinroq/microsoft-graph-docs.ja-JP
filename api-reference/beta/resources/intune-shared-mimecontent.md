---
title: mimeContent リソースの種類
description: 汎用 MIME コンテンツのプロパティが含まれています。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 62132b9e55b8130f82fc8414cbb6e90ba34bb70f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413459"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="3ae7d-103">mimeContent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3ae7d-103">mimeContent resource type</span></span>

> <span data-ttu-id="3ae7d-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3ae7d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3ae7d-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3ae7d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3ae7d-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3ae7d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ae7d-107">汎用 MIME コンテンツのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="3ae7d-107">Contains properties for a generic mime content.</span></span>

## <a name="properties"></a><span data-ttu-id="3ae7d-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3ae7d-108">Properties</span></span>
|<span data-ttu-id="3ae7d-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3ae7d-109">Property</span></span>|<span data-ttu-id="3ae7d-110">型</span><span class="sxs-lookup"><span data-stu-id="3ae7d-110">Type</span></span>|<span data-ttu-id="3ae7d-111">説明</span><span class="sxs-lookup"><span data-stu-id="3ae7d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ae7d-112">type</span><span class="sxs-lookup"><span data-stu-id="3ae7d-112">type</span></span>|<span data-ttu-id="3ae7d-113">String</span><span class="sxs-lookup"><span data-stu-id="3ae7d-113">String</span></span>|<span data-ttu-id="3ae7d-114">コンテンツ MIME の種類を示します。</span><span class="sxs-lookup"><span data-stu-id="3ae7d-114">Indicates the content mime type.</span></span>|
|<span data-ttu-id="3ae7d-115">value</span><span class="sxs-lookup"><span data-stu-id="3ae7d-115">value</span></span>|<span data-ttu-id="3ae7d-116">バイナリ</span><span class="sxs-lookup"><span data-stu-id="3ae7d-116">Binary</span></span>|<span data-ttu-id="3ae7d-117">実際のコンテンツを含むバイト配列です。</span><span class="sxs-lookup"><span data-stu-id="3ae7d-117">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3ae7d-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3ae7d-118">Relationships</span></span>
<span data-ttu-id="3ae7d-119">なし</span><span class="sxs-lookup"><span data-stu-id="3ae7d-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3ae7d-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3ae7d-120">JSON Representation</span></span>
<span data-ttu-id="3ae7d-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3ae7d-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mimeContent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mimeContent",
  "type": "String",
  "value": "binary"
}
```




