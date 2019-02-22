---
title: devicemanagementのトラブルシューティング errorresource リソースの種類
description: 'オブジェクト: トラブルシューティング情報へのリンクを表すオブジェクトは、Azure Portal または Microsoft doc にリンクします。'
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 25d97a6d085b9f1b7e0b1ab73361be3ac7ae74d2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30155560"
---
# <a name="devicemanagementtroubleshootingerrorresource-resource-type"></a><span data-ttu-id="fa9ab-103">devicemanagementのトラブルシューティング errorresource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fa9ab-103">deviceManagementTroubleshootingErrorResource resource type</span></span>

> <span data-ttu-id="fa9ab-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fa9ab-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fa9ab-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="fa9ab-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa9ab-106">オブジェクト: トラブルシューティング情報へのリンクを表すオブジェクトは、Azure Portal または Microsoft doc にリンクします。</span><span class="sxs-lookup"><span data-stu-id="fa9ab-106">Object representing a link to troubleshooting information, the link could be to the Azure Portal or a Microsoft doc.</span></span>

## <a name="properties"></a><span data-ttu-id="fa9ab-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fa9ab-107">Properties</span></span>
|<span data-ttu-id="fa9ab-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fa9ab-108">Property</span></span>|<span data-ttu-id="fa9ab-109">型</span><span class="sxs-lookup"><span data-stu-id="fa9ab-109">Type</span></span>|<span data-ttu-id="fa9ab-110">説明</span><span class="sxs-lookup"><span data-stu-id="fa9ab-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa9ab-111">text</span><span class="sxs-lookup"><span data-stu-id="fa9ab-111">text</span></span>|<span data-ttu-id="fa9ab-112">String</span><span class="sxs-lookup"><span data-stu-id="fa9ab-112">String</span></span>|<span data-ttu-id="fa9ab-113">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="fa9ab-113">Not yet documented</span></span>|
|<span data-ttu-id="fa9ab-114">link</span><span class="sxs-lookup"><span data-stu-id="fa9ab-114">link</span></span>|<span data-ttu-id="fa9ab-115">String</span><span class="sxs-lookup"><span data-stu-id="fa9ab-115">String</span></span>|<span data-ttu-id="fa9ab-116">web リソースへのリンク。</span><span class="sxs-lookup"><span data-stu-id="fa9ab-116">The link to the web resource.</span></span> <span data-ttu-id="fa9ab-117">次のいずれかのフォーマッタを含めることができます。 {{UPN}}、{{deviceguid}}、{{userguid}}</span><span class="sxs-lookup"><span data-stu-id="fa9ab-117">Can contain any of the following formatters: {{UPN}}, {{DeviceGUID}}, {{UserGUID}}</span></span>|

## <a name="relationships"></a><span data-ttu-id="fa9ab-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fa9ab-118">Relationships</span></span>
<span data-ttu-id="fa9ab-119">なし</span><span class="sxs-lookup"><span data-stu-id="fa9ab-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fa9ab-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fa9ab-120">JSON Representation</span></span>
<span data-ttu-id="fa9ab-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="fa9ab-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingErrorResource",
  "text": "String",
  "link": "String"
}
```




