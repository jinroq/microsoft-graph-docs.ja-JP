---
title: Devicemanagementのトラブルシューティング Errorresource リソースの種類
description: 'オブジェクト: トラブルシューティング情報へのリンクを表すオブジェクトは、Azure Portal または Microsoft doc にリンクします。'
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 712832420b556517be8ef053cc6cd292acfeed86
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33939848"
---
# <a name="devicemanagementtroubleshootingerrorresource-resource-type"></a><span data-ttu-id="0f0da-103">Devicemanagementのトラブルシューティング Errorresource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0f0da-103">deviceManagementTroubleshootingErrorResource resource type</span></span>

> <span data-ttu-id="0f0da-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0f0da-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0f0da-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0f0da-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f0da-106">オブジェクト: トラブルシューティング情報へのリンクを表すオブジェクトは、Azure Portal または Microsoft doc にリンクします。</span><span class="sxs-lookup"><span data-stu-id="0f0da-106">Object representing a link to troubleshooting information, the link could be to the Azure Portal or a Microsoft doc.</span></span>

## <a name="properties"></a><span data-ttu-id="0f0da-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0f0da-107">Properties</span></span>
|<span data-ttu-id="0f0da-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0f0da-108">Property</span></span>|<span data-ttu-id="0f0da-109">型</span><span class="sxs-lookup"><span data-stu-id="0f0da-109">Type</span></span>|<span data-ttu-id="0f0da-110">説明</span><span class="sxs-lookup"><span data-stu-id="0f0da-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f0da-111">text</span><span class="sxs-lookup"><span data-stu-id="0f0da-111">text</span></span>|<span data-ttu-id="0f0da-112">String</span><span class="sxs-lookup"><span data-stu-id="0f0da-112">String</span></span>|<span data-ttu-id="0f0da-113">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0f0da-113">Not yet documented</span></span>|
|<span data-ttu-id="0f0da-114">link</span><span class="sxs-lookup"><span data-stu-id="0f0da-114">link</span></span>|<span data-ttu-id="0f0da-115">String</span><span class="sxs-lookup"><span data-stu-id="0f0da-115">String</span></span>|<span data-ttu-id="0f0da-116">Web リソースへのリンク。</span><span class="sxs-lookup"><span data-stu-id="0f0da-116">The link to the web resource.</span></span> <span data-ttu-id="0f0da-117">次のいずれかのフォーマッタを含めることができます。 {{UPN}}、{{DeviceGUID}}、{{UserGUID}}</span><span class="sxs-lookup"><span data-stu-id="0f0da-117">Can contain any of the following formatters: {{UPN}}, {{DeviceGUID}}, {{UserGUID}}</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f0da-118">関係</span><span class="sxs-lookup"><span data-stu-id="0f0da-118">Relationships</span></span>
<span data-ttu-id="0f0da-119">なし</span><span class="sxs-lookup"><span data-stu-id="0f0da-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0f0da-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0f0da-120">JSON Representation</span></span>
<span data-ttu-id="0f0da-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0f0da-121">Here is a JSON representation of the resource.</span></span>
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




