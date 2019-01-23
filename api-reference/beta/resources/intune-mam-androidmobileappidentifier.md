---
title: androidMobileAppIdentifier リソースの種類
description: Android アプリの識別子。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f6c26c41ffcb36ee325f5e0fae907916a418fb8b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410281"
---
# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="1a1f7-103">androidMobileAppIdentifier リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1a1f7-103">androidMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="1a1f7-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1a1f7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1a1f7-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1a1f7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1a1f7-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1a1f7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a1f7-107">Android アプリの識別子。</span><span class="sxs-lookup"><span data-stu-id="1a1f7-107">The identifier for an Android app.</span></span>


<span data-ttu-id="1a1f7-108">[mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="1a1f7-108">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1a1f7-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1a1f7-109">Properties</span></span>
|<span data-ttu-id="1a1f7-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1a1f7-110">Property</span></span>|<span data-ttu-id="1a1f7-111">型</span><span class="sxs-lookup"><span data-stu-id="1a1f7-111">Type</span></span>|<span data-ttu-id="1a1f7-112">説明</span><span class="sxs-lookup"><span data-stu-id="1a1f7-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a1f7-113">packageId</span><span class="sxs-lookup"><span data-stu-id="1a1f7-113">packageId</span></span>|<span data-ttu-id="1a1f7-114">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="1a1f7-114">String</span></span>|<span data-ttu-id="1a1f7-115">Play ストアで指定されている、アプリの識別子。</span><span class="sxs-lookup"><span data-stu-id="1a1f7-115">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1a1f7-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1a1f7-116">Relationships</span></span>
<span data-ttu-id="1a1f7-117">なし</span><span class="sxs-lookup"><span data-stu-id="1a1f7-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1a1f7-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1a1f7-118">JSON Representation</span></span>
<span data-ttu-id="1a1f7-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1a1f7-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidMobileAppIdentifier"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidMobileAppIdentifier",
  "packageId": "String"
}
```




