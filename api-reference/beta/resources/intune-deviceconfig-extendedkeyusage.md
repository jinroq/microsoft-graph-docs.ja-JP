---
title: extendedKeyUsage リソースの種類
description: カスタムの拡張キー使用法の定義
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6ed825f44923d3fe86cc410397747b50a1f2c681
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425968"
---
# <a name="extendedkeyusage-resource-type"></a><span data-ttu-id="7a90d-103">extendedKeyUsage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7a90d-103">extendedKeyUsage resource type</span></span>

> <span data-ttu-id="7a90d-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7a90d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7a90d-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7a90d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7a90d-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7a90d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a90d-107">カスタムの拡張キー使用法の定義</span><span class="sxs-lookup"><span data-stu-id="7a90d-107">Custom Extended Key Usage definition</span></span>

## <a name="properties"></a><span data-ttu-id="7a90d-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7a90d-108">Properties</span></span>
|<span data-ttu-id="7a90d-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7a90d-109">Property</span></span>|<span data-ttu-id="7a90d-110">型</span><span class="sxs-lookup"><span data-stu-id="7a90d-110">Type</span></span>|<span data-ttu-id="7a90d-111">説明</span><span class="sxs-lookup"><span data-stu-id="7a90d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a90d-112">name</span><span class="sxs-lookup"><span data-stu-id="7a90d-112">name</span></span>|<span data-ttu-id="7a90d-113">String</span><span class="sxs-lookup"><span data-stu-id="7a90d-113">String</span></span>|<span data-ttu-id="7a90d-114">拡張キー使用法の名前</span><span class="sxs-lookup"><span data-stu-id="7a90d-114">Extended Key Usage Name</span></span>|
|<span data-ttu-id="7a90d-115">objectIdentifier</span><span class="sxs-lookup"><span data-stu-id="7a90d-115">objectIdentifier</span></span>|<span data-ttu-id="7a90d-116">String</span><span class="sxs-lookup"><span data-stu-id="7a90d-116">String</span></span>|<span data-ttu-id="7a90d-117">拡張キー使用法のオブジェクト識別子</span><span class="sxs-lookup"><span data-stu-id="7a90d-117">Extended Key Usage Object Identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="7a90d-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7a90d-118">Relationships</span></span>
<span data-ttu-id="7a90d-119">なし</span><span class="sxs-lookup"><span data-stu-id="7a90d-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7a90d-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7a90d-120">JSON Representation</span></span>
<span data-ttu-id="7a90d-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7a90d-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.extendedKeyUsage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.extendedKeyUsage",
  "name": "String",
  "objectIdentifier": "String"
}
```




