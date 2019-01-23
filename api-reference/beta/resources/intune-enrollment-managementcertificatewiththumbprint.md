---
title: managementCertificateWithThumbprint リソースの種類
description: まだ文書化されていません
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 765d3b9370e4b0f5eda481883956c72bf261e65a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418856"
---
# <a name="managementcertificatewiththumbprint-resource-type"></a><span data-ttu-id="960fb-103">managementCertificateWithThumbprint リソースの種類</span><span class="sxs-lookup"><span data-stu-id="960fb-103">managementCertificateWithThumbprint resource type</span></span>

> <span data-ttu-id="960fb-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="960fb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="960fb-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="960fb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="960fb-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="960fb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="960fb-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="960fb-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="960fb-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="960fb-108">Properties</span></span>
|<span data-ttu-id="960fb-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="960fb-109">Property</span></span>|<span data-ttu-id="960fb-110">型</span><span class="sxs-lookup"><span data-stu-id="960fb-110">Type</span></span>|<span data-ttu-id="960fb-111">説明</span><span class="sxs-lookup"><span data-stu-id="960fb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="960fb-112">拇印</span><span class="sxs-lookup"><span data-stu-id="960fb-112">thumbprint</span></span>|<span data-ttu-id="960fb-113">String</span><span class="sxs-lookup"><span data-stu-id="960fb-113">String</span></span>|<span data-ttu-id="960fb-114">管理証明書の拇印</span><span class="sxs-lookup"><span data-stu-id="960fb-114">The thumbprint of the management certificate</span></span>|
|<span data-ttu-id="960fb-115">証明書</span><span class="sxs-lookup"><span data-stu-id="960fb-115">certificate</span></span>|<span data-ttu-id="960fb-116">String</span><span class="sxs-lookup"><span data-stu-id="960fb-116">String</span></span>|<span data-ttu-id="960fb-117">Base 64 にエンコードされた証明書の管理</span><span class="sxs-lookup"><span data-stu-id="960fb-117">The Base 64 encoded management certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="960fb-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="960fb-118">Relationships</span></span>
<span data-ttu-id="960fb-119">なし</span><span class="sxs-lookup"><span data-stu-id="960fb-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="960fb-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="960fb-120">JSON Representation</span></span>
<span data-ttu-id="960fb-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="960fb-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managementCertificateWithThumbprint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managementCertificateWithThumbprint",
  "thumbprint": "String",
  "certificate": "String"
}
```




