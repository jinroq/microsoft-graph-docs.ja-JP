---
title: devicemanagementのトラブルシューティング errorresource リソースの種類
description: 'オブジェクト: トラブルシューティング情報へのリンクを表すオブジェクトは、Azure Portal または Microsoft doc にリンクします。'
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5905f62a1da0329db1b311ae586cdb64517a2b5d
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31796543"
---
# <a name="devicemanagementtroubleshootingerrorresource-resource-type"></a><span data-ttu-id="c377e-103">devicemanagementのトラブルシューティング errorresource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c377e-103">deviceManagementTroubleshootingErrorResource resource type</span></span>

> <span data-ttu-id="c377e-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c377e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c377e-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c377e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c377e-106">オブジェクト: トラブルシューティング情報へのリンクを表すオブジェクトは、Azure Portal または Microsoft doc にリンクします。</span><span class="sxs-lookup"><span data-stu-id="c377e-106">Object representing a link to troubleshooting information, the link could be to the Azure Portal or a Microsoft doc.</span></span>

## <a name="properties"></a><span data-ttu-id="c377e-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c377e-107">Properties</span></span>
|<span data-ttu-id="c377e-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c377e-108">Property</span></span>|<span data-ttu-id="c377e-109">型</span><span class="sxs-lookup"><span data-stu-id="c377e-109">Type</span></span>|<span data-ttu-id="c377e-110">説明</span><span class="sxs-lookup"><span data-stu-id="c377e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c377e-111">text</span><span class="sxs-lookup"><span data-stu-id="c377e-111">text</span></span>|<span data-ttu-id="c377e-112">String</span><span class="sxs-lookup"><span data-stu-id="c377e-112">String</span></span>|<span data-ttu-id="c377e-113">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="c377e-113">Not yet documented</span></span>|
|<span data-ttu-id="c377e-114">link</span><span class="sxs-lookup"><span data-stu-id="c377e-114">link</span></span>|<span data-ttu-id="c377e-115">文字列</span><span class="sxs-lookup"><span data-stu-id="c377e-115">String</span></span>|<span data-ttu-id="c377e-116">web リソースへのリンク。</span><span class="sxs-lookup"><span data-stu-id="c377e-116">The link to the web resource.</span></span> <span data-ttu-id="c377e-117">次のいずれかのフォーマッタを含めることができます。 {{UPN}}、{{deviceguid}}、{{userguid}}</span><span class="sxs-lookup"><span data-stu-id="c377e-117">Can contain any of the following formatters: {{UPN}}, {{DeviceGUID}}, {{UserGUID}}</span></span>|

## <a name="relationships"></a><span data-ttu-id="c377e-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c377e-118">Relationships</span></span>
<span data-ttu-id="c377e-119">なし</span><span class="sxs-lookup"><span data-stu-id="c377e-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c377e-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c377e-120">JSON Representation</span></span>
<span data-ttu-id="c377e-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c377e-121">Here is a JSON representation of the resource.</span></span>
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



