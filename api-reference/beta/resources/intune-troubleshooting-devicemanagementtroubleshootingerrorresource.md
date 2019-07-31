---
title: Devicemanagementのトラブルシューティング Errorresource リソースの種類
description: 'オブジェクト: トラブルシューティング情報へのリンクを表すオブジェクトは、Azure Portal または Microsoft doc にリンクします。'
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6454bad98938bc73d4cde8d48229f6146d07c0bb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010309"
---
# <a name="devicemanagementtroubleshootingerrorresource-resource-type"></a><span data-ttu-id="2c44d-103">Devicemanagementのトラブルシューティング Errorresource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2c44d-103">deviceManagementTroubleshootingErrorResource resource type</span></span>

> <span data-ttu-id="2c44d-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2c44d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2c44d-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2c44d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c44d-106">オブジェクト: トラブルシューティング情報へのリンクを表すオブジェクトは、Azure Portal または Microsoft doc にリンクします。</span><span class="sxs-lookup"><span data-stu-id="2c44d-106">Object representing a link to troubleshooting information, the link could be to the Azure Portal or a Microsoft doc.</span></span>

## <a name="properties"></a><span data-ttu-id="2c44d-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2c44d-107">Properties</span></span>
|<span data-ttu-id="2c44d-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2c44d-108">Property</span></span>|<span data-ttu-id="2c44d-109">型</span><span class="sxs-lookup"><span data-stu-id="2c44d-109">Type</span></span>|<span data-ttu-id="2c44d-110">説明</span><span class="sxs-lookup"><span data-stu-id="2c44d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c44d-111">text</span><span class="sxs-lookup"><span data-stu-id="2c44d-111">text</span></span>|<span data-ttu-id="2c44d-112">String</span><span class="sxs-lookup"><span data-stu-id="2c44d-112">String</span></span>|<span data-ttu-id="2c44d-113">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="2c44d-113">Not yet documented</span></span>|
|<span data-ttu-id="2c44d-114">link</span><span class="sxs-lookup"><span data-stu-id="2c44d-114">link</span></span>|<span data-ttu-id="2c44d-115">String</span><span class="sxs-lookup"><span data-stu-id="2c44d-115">String</span></span>|<span data-ttu-id="2c44d-116">Web リソースへのリンク。</span><span class="sxs-lookup"><span data-stu-id="2c44d-116">The link to the web resource.</span></span> <span data-ttu-id="2c44d-117">次のいずれかのフォーマッタを含めることができます。 {{UPN}}、{{DeviceGUID}}、{{UserGUID}}</span><span class="sxs-lookup"><span data-stu-id="2c44d-117">Can contain any of the following formatters: {{UPN}}, {{DeviceGUID}}, {{UserGUID}}</span></span>|

## <a name="relationships"></a><span data-ttu-id="2c44d-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2c44d-118">Relationships</span></span>
<span data-ttu-id="2c44d-119">なし</span><span class="sxs-lookup"><span data-stu-id="2c44d-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2c44d-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2c44d-120">JSON Representation</span></span>
<span data-ttu-id="2c44d-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2c44d-121">Here is a JSON representation of the resource.</span></span>
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





