---
title: adminConsent リソースの種類
description: 同意の情報を管理します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c76ac169bb15792afec908f62b9740e81a4d7e5b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415881"
---
# <a name="adminconsent-resource-type"></a><span data-ttu-id="dde70-103">adminConsent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="dde70-103">adminConsent resource type</span></span>

> <span data-ttu-id="dde70-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="dde70-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="dde70-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dde70-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dde70-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="dde70-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dde70-107">同意の情報を管理します。</span><span class="sxs-lookup"><span data-stu-id="dde70-107">Admin consent information.</span></span>

## <a name="properties"></a><span data-ttu-id="dde70-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dde70-108">Properties</span></span>
|<span data-ttu-id="dde70-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dde70-109">Property</span></span>|<span data-ttu-id="dde70-110">型</span><span class="sxs-lookup"><span data-stu-id="dde70-110">Type</span></span>|<span data-ttu-id="dde70-111">説明</span><span class="sxs-lookup"><span data-stu-id="dde70-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dde70-112">shareAPNSData</span><span class="sxs-lookup"><span data-stu-id="dde70-112">shareAPNSData</span></span>|[<span data-ttu-id="dde70-113">adminConsentState</span><span class="sxs-lookup"><span data-stu-id="dde70-113">adminConsentState</span></span>](../resources/intune-devices-adminconsentstate.md)|<span data-ttu-id="dde70-114">ユーザーと apple のデバイスのデータを共有するための管理者の同意の状態です。</span><span class="sxs-lookup"><span data-stu-id="dde70-114">The admin consent state of sharing user and device data to Apple.</span></span> <span data-ttu-id="dde70-115">可能な値は、`notConfigured`、`granted`、`notGranted` です。</span><span class="sxs-lookup"><span data-stu-id="dde70-115">Possible values are: `notConfigured`, `granted`, `notGranted`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dde70-116">関係</span><span class="sxs-lookup"><span data-stu-id="dde70-116">Relationships</span></span>
<span data-ttu-id="dde70-117">なし</span><span class="sxs-lookup"><span data-stu-id="dde70-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dde70-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dde70-118">JSON Representation</span></span>
<span data-ttu-id="dde70-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="dde70-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.adminConsent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.adminConsent",
  "shareAPNSData": "String"
}
```




